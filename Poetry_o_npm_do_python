Poetry - Project setup

# iniciar um projeto com poetry
$ poetry new [projeto]

# Estrutura de pastas e arquivos
poetry-demo
├── pyproject.toml
├── README.md
├── poetry_demo
│   └── __init__.py
└── tests
    └── __init__.py
    

# pyproject.toml Base

[tool.poetry]
name = "poetry-demo"
version = "0.1.0"
description = ""
authors = ["Sébastien Eustace <sebastien@eustace.io>"]
readme = "README.md"
packages = [{include = "poetry_demo"}]

[tool.poetry.dependencies]
python = "^3.7"


[build-system]
requires = ["poetry-core"]
build-backend = "poetry.core.masonry.api"

# Ativando a virtualenv do poetry
$ poetry shell

# Desativando e mantendo o shell
$ deactivate

#desativando e saindo do shell
$ exit

# Atualização das dependencias
$ poetry update

# Poetry run - Poetry vai ser igual o npm e o yarn da pra executar os scripts deles com Poetry run [nome_do_script.py]

# Iniciando um projeto pre-existente
$ cd pre-existente-project
$ poetry init

# Instalando/ adicionando blibiotecas e pacotes
$ poetry add httpx

# adicionando apenas a dependencia em dev
$ poetry add --dev httpx

# para remover a biblioteca ou o pacote
$ poetry remove httpx
obs: lembrando se a biblioteca estiver em dev usar o --dev

# Instalando dependencias - quando já definidas no projeto:
$ poetry install

## se deseja instalar apenas as dependencias execute:
$ poetry install --no-root

# Poetry Scripts - criação de scripts
## No pyproject.toml 

[tool.poetry.scripts]
# name do script     pacote.modulo:função
bagulho-cli =       'bagulho.cli:cli'

# Poetry build-buildar o projeto
$ poetry build

#Publicar o Modulo no PyPi
$ poetry publish

# Exportar as dependencias caso necessario 
$ poetry export > requirements.txt





