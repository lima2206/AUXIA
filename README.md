# API 6º Semestre ADS

# DomRock AI - Auxia

<p align="center">
      <img src="docs/Img/logo-BuzzTech.png" alt="logo da Buzz Tech" width="200">
      <h2 align="center"> Buzz Tech</h2>
</p>

<p align="center">
  | <a href ="#desafio"> Desafio</a>  |
  <a href ="#solucao"> Solução</a>  |   
  <a href ="#backlog"> Backlog do Produto</a>  |
  <a href ="#dor">DoR</a>  |
  <a href ="#dod">DoD</a>  |
  <a href ="#sprint"> Cronograma de Sprints</a>  |
  <a href ="#tecnologias">Tecnologias</a> |
  <a href ="#manual">Manual de Instalação</a>  | 
  <a href ="#equipe"> Equipe</a> |
</p>

> Status do Projeto: Em andamento 🛠️

## 🏅 Desafio <a id="desafio"></a>

O desafio consiste em criar uma aplicação web de avaliação de respostas de LLM. A aplicação deve permitir enviar um prompt para 2 (dois) LLMs via API simultaneamente. A seguir, a aplicação deve apresentar as 2 (duas) respostas obtidas. Para cada resposta, a aplicação apresenta os itens de avaliação das respostas e, ao final, a aplicação apresenta uma escala de comparação das duas respostas para que o usuário possa definir qual das duas respostas foi a melhor e justificar. Todas essas informações devem ser gravadas em um banco de dados que servirá para futuros retreinamentos dos LLMs.

## 🏅 Solução <a id="solucao"></a>

O AUXIA - Auxiliary AI Training, permitirá que os usuários enviem prompts para múltiplos modelos de IA, comparem suas respostas, avaliem cada uma segundo critérios objetivos, escolham a melhor resposta e justifiquem suas decisões. Esse processo garantirá um aprendizado por reforço eficiente, possibilitando o aprimoramento contínuo dos modelos utilizados através dos dados persistidos de cada avaliação.

## 📋 Backlog do Produto <a id="backlog"></a>

| Rank | Prioridade | User Story                                                                                                                                                                                                     | Story Points | Sprint | Requisito do Cliente | Status |
| :--: | :--------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :----: | :------------------: | :----: |
|  -   |    Alta    | Como usuário, eu quero ter as respostas das duas LLMs, para poder avaliá-las em critérios.                                                                                                                     |     N/D      |   1    |         R03          |   🗑️   |
|  1   |    Alta    | Como usuário, quero uma interface para inserir um prompt, para que eu possa enviá-lo às LLMs e obter suas respostas                                                                                            |      14      |   1    |         R02          |   ✅   |
|  2   |    Alta    | Como usuário, eu quero enviar um prompt para dois modelos de IA simultaneamente, para que eu possa avaliar suas respostas posteriormente.                                                                      |      47      |   1    |       R01/R09        |   ✅   |
|  3   |    Alta    | Como usuário, eu quero visualizar as respostas das LLMs de forma clara e acessível, para que eu possa analisá-las em critérios.                                                                                |      28      |   1    |         R03          |   ✅   |
|  4   |    Alta    | Como usuário, eu quero uma interface para poder avaliar cada resposta individualmente através de critérios definidos, para que eu possa analisar a qualidade das respostas geradas                             |      22      |   1    |         R03          |   ✅   |
|  5   |    Alta    | Como usuário, eu quero uma interface para poder escolher a melhor resposta entre as duas geradas pelas LLMs, para que o sistema registre minha decisão e justificativa.                                        |      29      |   1    |         R04          |   ✅   |
|  6   |    Alta    | Como Administrador, eu quero que as avaliações dos usuários sobre as LLMs sejam armazenadas em um BD, para que possam ser utilizadas em processos de fine-tunning futuramente.                                 |      41      |   1    |         R05          |   ✅   |
|  7   |    Alta    | Como usuário, eu quero ser alertado caso minha escolha entre LLM1 e LLM2 não esteja coerente com minha avaliação, para que eu possa revisar minha decisão antes de finalizar.                                  |      3       |   2    |         R04          |   🛠️   |
|  8   |    Alta    | Como usuário, eu quero que as respostas das LLMs sejam enriquecidas com informações relevantes da base de dados (vetorizada), para que sejam mais precisas                                                     |      5       |   2    |         R07          |   🛠️   |
|  9   |    Alta    | Como usuário, eu quero que a LLM utilize apenas o contexto recuperado para responder ao meu prompt, para que a resposta seja mais precisa e baseada em informações verificadas.                                |     N/D      |   2    |         R07          |   🗑️   |
|  10  |    Alta    | Como Administrador, eu gostaria de ser o primeiro usuário do sistema, já devidamente pré inserido no banco de dados, para que possa acessar a aplicação.                                                       |      44      |   1    |         R06          |   ✅   |
|  11  |   Média    | Como Administrador, eu quero cadastrar novos usuários na plataforma, para que somente pessoas autorizadas possam acessá-la.                                                                                    |     N/D      |   3    |         R06          |   -    |
|  12  |   Média    | Como usuário, eu quero acessar a aplicação através de uma interface de login, para que somente usuários autorizados possam utilizar o sistema.                                                                 |     N/D      |   3    |         R06          |   -    |
|  13  |   Média    | Como usuário autorizado, eu quero acessar o sistema através de um login, para utilizar a aplicação.                                                                                                            |     N/D      |   3    |         R06          |   -    |
|  14  |   Média    | Como usuário autenticado, eu quero poder fazer o logout da aplicação de forma segura, para que meus dados não fiquem acessíveis a terceiros.                                                                   |     N/D      |   3    |         R06          |   -    |
|  15  |   Média    | Como usuário, eu quero poder revisar minha escolha antes de submetê-la, para que eu tenha certeza de que minha decisão está correta.                                                                           |      2       |   2    |         R04          |   🛠️   |
|  16  |   Média    | Como Administrador, eu quero visualizar a lista de usuários cadastrados, para que eu possa gerenciar quem tem acesso ao sistema.                                                                               |     N/D      |   3    |         R06          |   -    |
|  17  |   Média    | Como Administrador, eu quero redefinir a senha de um usuário, para que eu possa ajudá-lo caso ele não consiga acessar a conta.                                                                                 |     N/D      |   3    |         R06          |   -    |
|  18  |   Média    | Como Administrador, eu quero excluir usuários do sistema, para que possa revogar o acesso de usuários a aplicação.                                                                                             |     N/D      |   3    |         R06          |   -    |
|  19  |   Baixa    | Como usuário, eu quero ser informado com mensagens de erro caso ocorra demora excessiva no envio do prompt ou na resposta das LLMs, ou outros erros, para que eu possa entender o problema e tentar novamente. |      2       |   2    |         R03          |   🛠️   |
|  20  |   Baixa    | Como usuário, eu quero ser informado com mensagens de erro caso haja falha na obtenção das respostas, para que eu possa entender o problema e tentar novamente.                                                |     N/D      |   2    |         R03          |   🗑️   |
|  21  |   Baixa    | Como usuário, eu quero poder receber mensagens claras sobre o status das avaliações, para ter certeza de que minha avaliação foi registrada corretamente.                                                      |      2       |   2    |         R03          |   🛠️   |
|  22  |   Baixa    | Como usuário, eu quero poder voltar para telas anteriores durante o processo de avaliação, para que eu possa corrigir informações antes de enviar a decisão final.                                             |      1       |   2    |       R03/R04        |   🛠️   |
|  23  |   Baixa    | Como usuário, eu não quero perder meu progresso de avaliação ao voltar para telas anteriores, para que eu possa visualizar o que escolhi e verificar se errei em alguma avaliação.                             |     N/D      |   2    |       R03/R04        |   🗑️   |
|  24  |   Baixa    | Como usuário, eu quero editar meus dados pessoais, para que eu possa manter minhas informações atualizadas.                                                                                                    |     N/D      |   3    |         R06          |   -    |

## 🏃‍ DoR - Definition of Ready <a id="dor"></a>

- User Stories com **Critérios de Aceitação**
- Subtarefas divididas **a partir das US**
- Design no **Figma**
- Modelagem do **Banco de Dados**
- Diagrama de **Rotas**
- Banco de Dados **Vetorizado** do Cliente

## 🏆 DoD - Definition of Done <a id="dod"></a>

- Manual de Usuário
- Manual da Aplicação
- Documentação da API (Application Programming Interface)
- Código completo
- Vídeos de cada etapa de entrega

## 📅 Cronograma de Sprints <a id="sprint"></a>

| Sprint          |    Período    | Documentação                                     |
| --------------- | :-----------: | ------------------------------------------------ |
| 🔖 **SPRINT 1** | 10/03 - 30/03 | [Sprint 1 Docs](docs\sprints\sprint-1\README.md) |
| 🔖 **SPRINT 2** | 07/04 - 27/04 | [Sprint 2 Docs](docs\sprints\sprint-2\README.md) |
| 🔖 **SPRINT 3** | 05/05 - 25/05 | [Sprint 2 Docs](docs\sprints\sprint-3\README.md) |

## 💻 Tecnologias <a id="tecnologias"></a>

<h4 align="center">
 <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"></a>
 <a href="https://fastapi.tiangolo.com/"><img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/></a>
 <a href="https://www.typescriptlang.org/"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white"></a>
 <a href="https://vuejs.org/"><img src="https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vue.js&logoColor=4FC08D"/></a>
 <a href="https://www.mongodb.com/"><img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white"></a>
 <a href="https://www.trychroma.com/"><img src="https://img.shields.io/badge/ChromaDB-FF6B00?style=for-the-badge&logo=chroma&logoColor=white"></a>
 <a href="https://www.atlassian.com/software/jira"><img src="https://img.shields.io/badge/Jira-0052CC?style=for-the-badge&logo=jira&logoColor=white"/></a>
 <a href="https://miro.com/"><img src="https://img.shields.io/badge/Miro-1A1A1A?style=for-the-badge&logo=miro&logoColor=white"/></a>
 <a href="https://github.com/"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white"/></a>
 <a href="https://www.figma.com/"><img src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white"/></a>
</h4>

## 📖 Manual de Instalação <a id="manual"></a>

### 🛠 Pré-requisitos

- Git ([Download](https://git-scm.com/downloads))

- Python 3.9+ ([Download](https://www.python.org/downloads/))

- Node.js 16+ ([Download](https://nodejs.org/en/download))

- Poetry (opcional para o backend) ([Download](https://python-poetry.org/))

---

### 1. Clonar o Repositório Principal

```bash
git clone --recurse-submodules https://github.com/BuzzTech-API/API_ADS_6SEMESTE_2025.1.git
cd API_ADS_6SEMESTE_2025.1
```

> **Observação:** Se já tiver clonado sem os submódulos, execute:

```
git submodule update --init --recursive
```

---

### 2. Configuração do Backend (auxia-backend)

**1° Adicione as variáveis no .env**

**2° Instale e Inicie a aplicação:**

**Opção A: Com Poetry**

```bash
cd ./auxia-backend
poetry shell
poetry install
make run
```

**Opção B: Com Ambiente Virtual Python**

```bash
cd ./auxia-backend
python3 -m venv venv
source venv/bin/activate # se você usa linux
venv/Scripts/activate 	 # se você usa windows
pip install -r requirements.txt
fastapi dev ./auxia/main.py
```

**Saída Esperada:**
<br>
Servidor rodando em `http://localhost:8000` (acesse `http://localhost:8000/docs` para a UI do Swagger).

---

### 3. Configuração do Frontend (auxia-frontend)

```bash
cd ../auxia-frontend/auxia
npm install
npm run dev
```

**Saída Esperada:**
<br>
Frontend rodando em `http://localhost:5173`.

## 🎓 Equipe <a id="equipe"></a>

<div align="center">
  <table>
    <tr>
      <th>Membro</th>
      <th>Função</th>
      <th>Github</th>
      <th>Linkedin</th>
    </tr>
    <tr>
      <td>Ivan Duarte</td>
      <td>Product Owner</td>
      <td><a href="https://github.com/Ivan-Duarte"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/ivan-duarte-982532217"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Vitor Lima</td>
      <td>Scrum Master</td>
      <td><a href="https://github.com/lima2206"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/vitor-spricigo-lima-84a377184"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Isaque da Silva</td>
      <td>Desenvolvedor</td>
      <td><a href="https://github.com/KhovetS2"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/isaque-elis-da-silva-2a4087226/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Joice Araujo</td>
      <td>Desenvolvedor</td>
      <td><a href="https://github.com/Joice-Araujo"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/joice-aparecida-581226250/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Jonas Alves</td>
      <td>Desenvolvedor</td>
      <td><a href="https://github.com/dodekafonos"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="http://linkedin.com/in/jonas-alves"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Pedro Davi</td>
      <td>Desenvolvedor</td>
      <td><a href="https://github.com/PedrohDavi"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/pedro-davi-jobs/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Rafael Motta</td>
      <td>Desenvolvedor</td>
      <td><a href="https://github.com/Rafael-Motta"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/rafaelmotta97"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
  </table>
</div>
