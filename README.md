# Projeto Desafio

Desenvolvedor: Joedson Gabriel | json.gbriel@gmail.com

#

## Requisitos para executar o projeto

* Docker Compose https://docs.docker.com/desktop/

    *OBS: Também é possível executar o projeto usando apenas Python e Node.js  (Instruções no final deste arquivo)*

#

## Como executar o projeto?

Utilize o docker compose

    docker compose up

*Obs: O alias do docker compose pode mudar dependendo da versão: **docker-compose** ou **docker compose (v2)***

Após a inicialização o sistema estará disponível conforme abaixo

* API
    * http://localhost:8000

* Front
    * http://localhost:8080

#
## Sobre o projeto

Este projeto foi desenvolvido utilizando as seguintes tecnologias

* Back-end: Django (Python)
* API: Django Rest Framework
* Banco de dados: SQLite (local)
* Infraestrutura em Docker
* Front-end: Vue.js (Node.js)
* Biblioteca visual frontend: Bootstrap Vue


#

## Alternativa para executar o projeto (sem o Docker)

Requisitos: Python 3 e Node.js

Link do python: https://www.python.org/

Link do Node.js: https://nodejs.org
* **Passo a passo (API)**:

    * Entre no diretório **api-desafio**:
        * ```cd api-desafio```

    * Crie uma **virtual env** com o Python:
        * ```python3 -m venv .venv```

    * Ative a **virtual env**:
        * Linux: ```source .venv/bin/active```
        * Windows: ```.venv\Scripts\activate.bat```

    * Instale os **requirements.txt**:
        * ```pip install -r requirements.txt```

    * Aplique as migrações:
        * ```python manage.py migrate```

    * Execute o servidor:
        * ```python manage.py runserver 0.0.0.0:8000```


### Passo a passo (Front)

* Entre no diretório **front-desafio**:
    * ```cd front-desafio```
* Instale as dependências usando **npm** ou **yarn**:
    * ```npm install```
    
        ou

    * ```yarn install```

* Inicie o servidor front:

    * ```npm run serve```
    
        ou

    * ```yarn serve```
