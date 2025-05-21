# Padrão de Commits

Os commits devem seguir o padrão **"Padrão de Commits – por Renato Adorno"** para manter a consistência e a clareza no repositório.

## Formato do Commit:
```
<tipo>: <descrição em tom de ação direta>
<informações adicionais (opcional)>
```

## Tipos de Commit:
- **fix** – Soluciona um problema (bug fix). Relacionado ao PATCH no versionamento semântico.
- **feat** – Inclui um novo recurso. Relacionado ao MINOR no versionamento semântico.
- **docs** – Mudanças na documentação (como Readme). Não inclui alterações em código.
- **style** – Alterações de formatação de código (ex: semicolons, trailing spaces, lint). Não inclui alterações em código.
- **refactor** – Refatorações que não alteram funcionalidades, como melhoria de performance ou ajustes no código sem mudar o comportamento.
- **build** – Modificações em arquivos de build e dependências.
- **test** – Alterações em testes (criação, modificação ou remoção de testes unitários).
- **chore** – Atualizações de tarefas administrativas ou configuração, como adição de pacotes no gitignore.

## Exemplos:
- **feat**: Adiciona botão de login na tela inicial
- **fix**: Corrige bug no redirecionamento após login
- **refactor**: Refatora lógica de autenticação para usar hooks
- **docs**: Documenta processo de deploy no README
- **style**: Remove espaços em branco desnecessários
