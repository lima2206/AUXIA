# API 6º Semestre ADS

# DomRock AI - Auxia

# Documentação - Sprint 2

<p align="center">
      <img src="../../../img/logo-BuzzTech.png" alt="logo da Buzz Tech" width="200">
      <h2 align="center"> Buzz Tech</h2>
</p>

<p align="center">
  | <a href ="#desafio"> Desafio</a>  |
  <a href ="#us"> User Stories</a>  |   
  <a href ="#dor">DoR</a>  |
  <a href ="#dod">DoD</a>  |
  <a href ="#burndown">Burndown</a>  | 
  <a href ="#equipe"> Equipe</a> |
</p>

> Status da Sprint: Concluído ✅

## 🏅 Desafio <a id="desafio"></a>

Implementar funcionalidades que aprimorem a experiência do usuário durante o processo de avaliação das respostas geradas por LLMs, garantindo maior confiabilidade, interatividade e controle nas decisões. Nesta sprint, será feita a integração da base vetorizada com as LLMs por meio da técnica de RAG (Retrieval-Augmented Generation), permitindo que as respostas sejam enriquecidas com informações relevantes e atualizadas. Além disso, serão implementadas melhorias no fluxo de avaliação, como alertas de inconsistência, mensagens de status e erro mais claras, e navegação mais flexível para revisão e correção de decisões.

## 📋 User Stories <a id="us"></a>

| Rank | Prioridade | User Story                                                                                                                                                                                                     | Story Points | Sprint | Requisito do Cliente | Status |
| :--: | :--------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------: | :----: | :------------------: | :----: |
|  7   |    Alta    | Como usuário, eu quero ser alertado caso minha escolha entre LLM1 e LLM2 não esteja coerente com minha avaliação, para que eu possa revisar minha decisão antes de finalizar.                                  |      3       |   2    |         R04          |   ✅   |
|  8   |    Alta    | Como usuário, eu quero que as respostas das LLMs sejam enriquecidas com informações relevantes da base de dados (vetorizada), para que sejam mais precisas                                                     |      5       |   2    |         R07          |   ✅   |
|  15  |   Média    | Como usuário, eu quero poder revisar minha escolha antes de submetê-la, para que eu tenha certeza de que minha decisão está correta.                                                                           |      2       |   2    |         R04          |   ✅   |
|  19  |   Baixa    | Como usuário, eu quero ser informado com mensagens de erro caso ocorra demora excessiva no envio do prompt ou na resposta das LLMs, ou outros erros, para que eu possa entender o problema e tentar novamente. |      2       |   2    |         R03          |   ✅   |
|  21  |   Baixa    | Como usuário, eu quero poder receber mensagens claras sobre o status das avaliações, para ter certeza de que minha avaliação foi registrada corretamente.                                                      |      2       |   2    |         R03          |   ✅   |
|  22  |   Baixa    | Como usuário, eu quero poder voltar para telas anteriores durante o processo de avaliação, para que eu possa corrigir informações antes de enviar a decisão final.                                             |      1       |   2    |       R03/R04        |   ✅   |

## 🏅 DoR - Definition of Ready <a id="dor"></a>

|              Critério              | Descrição                                                                                          |
| :--------------------------------: | -------------------------------------------------------------------------------------------------- |
|        Clareza na Descrição        | A User Story está escrita no formato “Como [persona], quero [ação] para que [objetivo]”            |
|  Critérios de Aceitação Definidos  | A história possui critérios objetivos que indicam o que é necessário para considerá-la concluída.  |
|  Cenários de Teste Especificados   | A história tem pelo menos 1 cenário de teste estruturado (Dado, Quando, Então).                    |
|            Independente            | A história pode ser implementada sem depender de outra tarefa da mesma Sprint.                     |
|      Escopo Técnico Validado       | Há clareza se a história envolve frontend, backend ou ambos — com pontos de integração definidos.  |
|             Estímável              | A história foi pontuada no Planning Poker ou tem uma estimativa clara.                             |
| Referências ou Documentos de Apoio | Onde necessário, foram fornecidos arquivos, links (ex: base vetorizada), ou instruções adicionais. |
|     Validação com PO e equipe      | A história foi discutida em refinamento ou planning e validada com o time técnico.                 |
| Alinhamento com arquitetura atual  | A funcionalidade proposta está coerente com o funcionamento já entregue na Sprint 1.               |

## 🏅 DoD - Definition of Done <a id="dod"></a>

|                 Critério                 | Descrição                                                                                                        |
| :--------------------------------------: | ---------------------------------------------------------------------------------------------------------------- |
|     Critérios de Aceitação atendidos     | Todos os critérios definidos na US foram implementados e validados com sucesso.                                  |
| Cenários de Teste executados e aprovados | Todos os cenários descritos foram validados manualmente ou por teste automatizado.                               |
|      Dados persistidos corretamente      | Informações sensíveis como prompt, resposta, avaliação ou contexto vetorizado foram salvos conforme esperado.    |
|       Feedback visual implementado       | Funcionalidades como pop-ups, mensagens de erro ou barras de progresso estão claras e acessíveis ao usuário.     |
|        Fluxo seguro e controlado         | Não há caminhos quebrados nem submissões incoerentes no fluxo de avaliação ou navegação.                         |
|      Código revisado (Code Review)       | A US passou por revisão entre pares antes da integração.                                                         |
|  Integrado com o restante da aplicação   | A funcionalidade foi testada junto com o fluxo completo do sistema (Ex: Envio → Resposta → Avaliação → Escolha). |
|     Documentação Técnica atualizada      | Se aplicável, a lógica de RAG, manipulação da base vetorizada ou instruções de uso estão registradas.            |
|         Validação final com o PO         | O PO testou e confirmou que a funcionalidade atende ao esperado.                                                 |
|            Pronta para Deploy            | A funcionalidade pode ser entregue ao ambiente de produção/testes finais sem pendências.                         |

## 🏅 Sprint Burndown <a id="burndown"></a>

<p align="center">
      <img src="../../../img/Burndown_Sprint2.jpg" alt="Burndown Sprint 2" width="500">
</p>

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
      <td>Vitor Spricigo Lima</td>
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
