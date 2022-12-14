# Projeto Desafio

Desenvolvedor: Joedson Gabriel | json.gbriel@gmail.com
#

# Requisitos para executar o projeto

* Docker Compose https://docs.docker.com/compose/install/

    *OBS: Também é possível executar o projeto usando apenas Python e Node.js  (Instruções no final deste documento)*

#

# Como executar o projeto?

Utilize o docker compose

* Comandos para inicialização
   * ```docker compose build --no-cache```
   * ```docker compose run api-desafio python manage.py migrate```
   * ```docker compose up -d```

*Obs: Verifique a versão do docker instalada: **docker-compose** ou **docker compose (v2)***

Após a inicialização o sistema estará disponível conforme abaixo

* API
    * http://localhost:8000/api

* Front
    * http://localhost:8080


#

## Esta aplicação também foi disponibilizada em nuvem para poupar a necessidade de executar localmente.

- API (http): http://34.125.118.24:8000/api/

- Front (http): http://34.125.118.24:8080/#/

#

# Sobre o projeto
Este projeto foi desenvolvido utilizando as seguintes tecnologias

* Back-end: Django (Python)
* API: Django Rest Framework
* Banco de dados: SQLite (local)
* Infraestrutura em Docker
* Front-end: Vue.js (Node.js)
* Biblioteca visual frontend: Bootstrap Vue
* Deploy: Google Cloud

#
# Especificações da API Rest
 
## Endpoint de usuários

* Cadastro (Método POST)
    * Endpoint
        * ```/api/user/```
    * Formato do dado a ser enviado
        * {
            "name":"",
            "email":"",
            "born_date":"YYYY-MM-DD",
            "password":"########"
        }

* Listagem (Método GET)
    * Endpoint
        * ```/api/user/```

* Edição (Método PUT)
    * Endpoint
        * ```/api/user/<pk:register>/```
    * Formato do dado a ser enviado
        * {
            "name":"",
            "email":"",
            "born_date":"YYYY-MM-DD",
            "password":"########"
        }
* Exclusão (Método DELETE)
    * Endpoint
        * ```/api/user/<pk:register>/```

#

# Alternativa para executar o projeto (sem o Docker)

### Requisitos: 

Python 3 https://www.python.org/

Node.js https://nodejs.org

## Passo a passo (API):

* Acesse o diretório **api-desafio**:
    * ```cd api-desafio```

* Crie um **virtual environment** com o Python: (Opcional)
    * ```python3 -m venv .venv```

* Ative o **virtual environment**: (Opcional)
    * Linux: ```source .venv/bin/active```
    * Windows: ```.venv\Scripts\activate.bat```

* Instale os **requirements.txt**:
    * ```pip install -r requirements.txt```

* Aplique as migrações:
    * ```python manage.py migrate```

* Execute o servidor:
    * ```python manage.py runserver 0.0.0.0:8000```
#

## Passo a passo (Front)

* Acesse o diretório **front-desafio**:
    * ```cd front-desafio```

* Instale as dependências usando **npm**:
    * ```npm install```

* Inicie o servidor front:

    * ```npm run serve```
