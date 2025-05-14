# API_ADS_6SEMESTE_2025.1

# Guia de instalação do projeto

## Descrição

Este repositório contém a aplicação desenvolvida para o 6º semestre do curso de Análise e Desenvolvimento de Sistemas da FATEC São José dos Campos - Prof. Jessen Vidal. A aplicação é composta por múltiplos componentes organizados como submódulos Git.

## Pré-requisitos

Git instalado na máquina - [Download](https://git-scm.com/downloads)

Node.js e npm instalados - [Download](https://nodejs.org/pt/download)

Python 3+ instalado - [Download](https://www.python.org/downloads/)

## Clonando o Repositório

Para clonar o repositório principal e todos os seus submódulos, execute o seguinte comando:
```bash
git clone --recurse-submodules https://github.com/BuzzTech-API/API_ADS_6SEMESTE_2025.1.git
```

Caso já tenha clonado o repositório sem a opção --recurse-submodules, inicialize e atualize os submódulos manualmente:

```bash
cd ./API_ADS_6SEMESTE_2025.1
git submodule update --init --recursive
```

## Inicializando a Aplicação

#### Instale as dependências

Após clonar o repositório e os submódulos, siga os passos abaixo para iniciar a aplicação:

Instale as dependências necessárias para cada submódulo:

``` bash
# Entre no repositório
cd ./auxia-frontend/auxia

# Instale as dependências
npm install
```

Logo após:
``` bash
# Entre no repositório
cd ../../auxia-backend

# Crie o ambiente virtual python (caso já tenha, pule esse comando)
python -m venv venv

# inicie o ambiente virtual
.\venv\Scripts\activate

# Instale as dependências
pip install -r .\requirements.txt
```

Configure as **variáveis de ambiente** conforme necessário. Crie o arquivo **.env** no diretório ./auxia-backend com as configurações exigidas.
Todas as informações estão no arquivo
>.env.example

#### Inicie os serviços.

Servidor Backend:

```bash
# Entre no repositório (caso ainda não esteja)
cd ./auxia-backend

# inicie o ambiente virtual
.\venv\Scripts\activate

# Inicie o Servidor Backend
fastapi dev ./auxia/main.py
```

Em outro Terminal, Servidor Frontend:

```bash
# Entre no repositório
cd ./auxia-frontend/auxia

# Inicie o servidor Frontend
npm run dev
```


