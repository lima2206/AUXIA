# API 5º Semestre ADS 
# DomRock AI - Auxia

<p align="center">
      <img src="Documentação/Img/Logo/logo-BuzzTech.png" alt="logo da Buzz Tech" width="200">
      <h2 align="center"> Buzz Tech</h2>
</p>

<hr>

<p align="center">
  <a href ="#desafio"> Desafio </a>  |   
  <a href ="#metodologia"> Metodologia </a>  |
  <a href ="#mvp"> MVP </a>  |
  <a href ="#sprint"> Sprints </a>  |
  <a href ="#backlog"> Backlog do Produto </a>  | 
  <a href ="#equipe"> Equipe </a> |
</p>

<h4 align="center">
 <a href="https://www.figma.com/"><img src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white"/></a>
 <a href="https://github.com/"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white"/></a>
 <a href="https://fastapi.tiangolo.com/"><img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/></a>
 <a href="https://www.atlassian.com/software/jira"><img src="https://img.shields.io/badge/Jira-0052CC?style=for-the-badge&logo=jira&logoColor=white"/></a>
 <a href="https://vuejs.org/"><img src="https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vue.js&logoColor=4FC08D"/></a>
 <a href="https://miro.com/"><img src="https://img.shields.io/badge/Miro-1A1A1A?style=for-the-badge&logo=miro&logoColor=white"/></a>
</h4>

> Status do Projeto: Em andamento

## :medal_sports: Desafio <a id="desafio"></a>

O desafio consiste em criar uma aplicação web de avaliação de respostas de LLM. A aplicação deve permitir enviar um prompt para 2 (dois) LLMs via API simultaneamente. A seguir, a aplicação deve apresentar as 2 (duas) respostas obtidas. Para cada resposta, a aplicação apresenta os itens de avaliação das respostas e, ao final, a aplicação apresenta uma escala de comparação das duas respostas para que o usuário possa definir qual das duas respostas foi a melhor e justificar. Todas essas informações devem ser gravadas em um banco de dados que servirá para futuros retreinamentos dos LLMs.

## 🚀 MVP <a id="mvp"></a>

Criar o primeiro entregável de valor ao Cliente, consistindo em uma aplicação Local que tenha em sua lógica a técnica do RLHF.

## 📅 Sprints <a id="sprint"></a>

🔖 **SPRINT 1:** Concluído! ✅

🔖 **SPRINT 2:** 27/04

🔖 **SPRINT 3:** 25/05

## :books: Metodologia <a id="metodologia"></a>

O framework de Metodologia Ágil utilizado foi o Scrum, que possui os seguintes princípios norteadores:

1. Controle empírico
2. Auto-organização
3. Colaboração
4. Priorização da criação de valor
5. Time-boxing
6. Desenvolvimento iterativo

O projeto foi dividido em Sprints, onde priorizamos tarefas que trouxessem maior valor ao cliente. Utilizamos a construção de Personas para guiar nossas Histórias de Usuários e o Planning Poker para definir o tempo necessário para cada tarefa.

## 📋 Backlog do Produto <a id="backlog"></a>

- **Inserção de Prompt**: Como usuário, quero uma interface para inserir um prompt, para que eu possa enviá-lo às LLMs e obter suas respostas.
- **Envio para Múltiplos Modelos**: Como usuário, eu quero enviar um prompt para dois modelos de IA simultaneamente, para que eu possa avaliar suas respostas posteriormente.
- **Avaliação Individual**: Como usuário, eu quero uma interface para poder avaliar cada resposta individualmente através de critérios definidos, para que eu possa analisar a qualidade das respostas geradas.
- **Escolha da Melhor Resposta**: Como usuário, eu quero uma interface para poder escolher a melhor resposta entre as duas geradas pelas LLMs, para que o sistema registre minha decisão e justificativa.
- **Visualização Clara das Respostas**: Como usuário, eu quero visualizar as respostas das LLMs de forma clara e acessível, para que eu possa analisá-las em critérios.
- **Armazenamento das Avaliações**: Como Administrador, eu quero que as avaliações dos usuários sobre as LLMs sejam armazenadas em um BD, para que possam ser utilizadas em processos de fine-tuning futuramente.
- **Usuário Inicial Pré-Definido**: Como Administrador, eu gostaria de ser o primeiro usuário do sistema, já devidamente pré-inserido no banco de dados, para que possa acessar a aplicação.

## :mortar_board: Equipe <a id="equipe"></a>

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
      <td>Nilber Siqueira</td>
      <td>Scrum Master</td>
      <td><a href="https://github.com/NilberSiqueira"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/nilber-siqueira-b3404a176"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Isaque da Silva</td>
      <td>Product Owner</td>
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
      <td>Vitor Lima</td>
      <td>Desenvolvedor</td>
      <td><a href="https://github.com/lima2206"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/vitor-spricigo-lima-84a377184"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Rafael Motta</td>
      <td>Desenvolvedor</td>
      <td><a href="https://github.com/Rafael-Motta"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/rafaelmotta97"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
  </table>
</div>
