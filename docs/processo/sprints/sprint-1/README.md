
# API 6º Semestre ADS

# DomRock AI - Auxia

# Documentação - Sprint 1

<p align="center">
      <img src="../../../img/logo-BuzzTech.png" alt="logo da Buzz Tech" width="200">
      <h2 align="center"> Buzz Tech</h2>
</p>

<p align="center">
  | <a href ="#desafio"> Desafio</a>  |
  <a href ="#us"> User Stories</a>  |   
  <a href ="#dor">DoR</a>  |
  <a href ="#dod">DoD</a>  |
  <a href ="#equipe"> Equipe</a> |
</p>

> Status da Sprint: Concluída ✅

## 🏅 Desafio <a id="desafio"></a>

Implementar a base do sistema de RLHF, permitindo que os usuários interajam com dois modelos LLMs de forma simultânea, avaliem as respostas com critérios definidos e escolham a melhor com justificativa. Foi necessário garantir uma interface clara, armazenamento eficiente das avaliações e estrutura adequada para suportar futuras etapas da implementação do RAG, consolidando o fluxo inicial de aprendizado com reforço baseado em feedback humano.

## 📋 User Stories <a id="us"></a>

| Rank | Prioridade | User Story                                                                                                                                                                         | Story Points | Sprint | Requisito do Cliente | Status |
| :--: | :--------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :----: | :------------------: | :----: |
|  1   |    Alta    | Como usuário, quero uma interface para inserir um prompt, para que eu possa enviá-lo às LLMs e obter suas respostas                                                                |      14      |   1    |         R02          |   ✅   |
|  2   |    Alta    | Como usuário, eu quero enviar um prompt para dois modelos de IA simultaneamente, para que eu possa avaliar suas respostas posteriormente.                                          |      47      |   1    |       R01/R09        |   ✅   |
|  3   |    Alta    | Como usuário, eu quero visualizar as respostas das LLMs de forma clara e acessível, para que eu possa analisá-las em critérios.                                                    |      28      |   1    |         R03          |   ✅   |
|  4   |    Alta    | Como usuário, eu quero uma interface para poder avaliar cada resposta individualmente através de critérios definidos, para que eu possa analisar a qualidade das respostas geradas |      22      |   1    |         R03          |   ✅   |
|  5   |    Alta    | Como usuário, eu quero uma interface para poder escolher a melhor resposta entre as duas geradas pelas LLMs, para que o sistema registre minha decisão e justificativa.            |      29      |   1    |         R04          |   ✅   |
|  6   |    Alta    | Como Administrador, eu quero que as avaliações dos usuários sobre as LLMs sejam armazenadas em um BD, para que possam ser utilizadas em processos de fine-tunning futuramente.     |      41      |   1    |         R05          |   ✅   |
|  10  |    Alta    | Como Administrador, eu gostaria de ser o primeiro usuário do sistema, já devidamente pré inserido no banco de dados, para que possa acessar a aplicação.                           |      44      |   1    |         R06          |   ✅   |

## 🏅 DoR - Definition of Ready <a id="dor"></a>

|             Critério             | Descrição                                                                                         |
| :------------------------------: | ------------------------------------------------------------------------------------------------- |
|       Clareza na Descrição       | A User Story está escrita no formato “Como [persona], quero [ação] para que [objetivo]”           |
| Critérios de Aceitação Definidos | A história possui critérios objetivos que indicam o que é necessário para considerá-la concluída. |
| Cenários de Teste Especificados  | A história tem pelo menos 1 cenário de teste estruturado (Dado, Quando, Então).                   |
|           Independente           | A história pode ser implementada sem depender de outra tarefa da mesma Sprint.                    |
|    Compreensão Compartilhada     | Toda a equipe (incluindo PO e devs) compreende o propósito da história.                           |
|            Estímável             | A história foi pontuada no Planning Poker ou tem uma estimativa clara.                            |
|       Documentos de Apoio        | Se necessário, mockups, fluxos ou modelos de dados estão anexados ou referenciados.               |
|   Critérios técnicos acordados   | As necessidades de Frontend e Backend foram claramente separadas (quando aplicável).              |

## 🏅 DoD - Definition of Done <a id="dod"></a>

|                 Critério                 | Descrição                                                                            |
| :--------------------------------------: | ------------------------------------------------------------------------------------ |
|     Critérios de Aceitação atendidos     | Todos os cenários de teste da história foram executados e aprovados.                 |
|        Testes manuais realizados         | Onde aplicável (ex: US07), os dados são corretamente armazenados e recuperáveis.     |
|             Código revisado              | O código foi revisado por pelo menos um colega de equipe.                            |
|     Documentação interna atualizada      | Foi atualizado o que for necessário: API, estrutura de dados, endpoints, etc.        |
|  Integração com outras partes testadas   | As interfaces entre Frontend e Backend foram validadas.                              |
| Build/Testes automatiados (se aplicável) | A funcionalidade não quebra a aplicação e passa nos testes automatizados existentes. |
|             Validação do PO              | O Product Owner validou a entrega com base nos critérios definidos.                  |
|            Pronto para deploy            | O item está testado, validado e pode ser integrado ao produto final.                 |

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
      <td>Nilber Siqueira</td>
      <td>Scrum Master</td>
      <td><a href="https://github.com/NilberSiqueira"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"></a></td>
      <td><a href="https://www.linkedin.com/in/nilber-siqueira-b3404a176"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a></td>
    </tr>
    <tr>
      <td>Vitor Spricigo Lima</td>
      <td>Desenvolvedor</td>
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
