# 📘 API Auxia – Documentação de Rotas

---

## 🧠 AI – LLM Endpoints

---

### `POST /ai/generate`
**Descrição:** Executa um prompt utilizando dois modelos LLM distintos simultaneamente. Retorna as respostas de ambos os modelos e as respectivas identificações. Ideal para comparações e análises paralelas entre modelos.   
**Corpo da requisição:**

```
json
{
  "prompt": "string"
}
```

**Resposta `200`:**
```
json
{
  "response1": "string",
  "response2": "string",
  "modelLlm1": "string",
  "modelLlm2": "string"
}
```

---

### `POST /ai/generatenorag`
**Descrição:** Semelhante à rota /ai/generate, mas executa os modelos sem mecanismos auxiliares de RAG (Retrieval-Augmented Generation). Retorna apenas a resposta bruta de cada LLM, útil para testes em "modo puro" dos modelos.  
**Corpo da requisição:**

```
json
{
  "prompt": "string"
}
```

**Resposta `200`:**
```
json
{
  "response1": "string",
  "response2": "string",
  "modelLlm1": "string",
  "modelLlm2": "string"
}
```

---

### `POST /ai/llm1`
**Descrição:** Executa o prompt exclusivamente no modelo LLM 1. Esta rota é útil para debug, validações ou testes isolados de comportamento do modelo 1, sem envolvimento de outros modelos ou comparações.
**Corpo da requisição:**

```
json
{
  "prompt": "string"
}
```

**Resposta `200`:**
```
json
{ 
  "response": "string"
}
```

---

### `POST /ai/llm2`
**Descrição:** Executa o prompt exclusivamente no modelo LLM 2. Esta rota é útil para debug, validações ou testes isolados de comportamento do modelo 2, sem envolvimento de outros modelos ou comparações.
**Corpo da requisição:**

```
json
{
  "prompt": "string"
}
```

**Resposta `200`:**
```
json
{ 
  "response": "string"
}
```

---

## 📝 Avaliação de Respostas

---

### `POST /answer`
**Descrição:**  
Salva uma avaliação detalhada da resposta de uma LLM (modelo de linguagem). Essa rota registra o prompt utilizado, a resposta gerada, o modelo que respondeu e as **justificativas e pontuações** para diferentes critérios de qualidade, como relevância, clareza, confiabilidade, entre outros.

**Segurança:** `OAuth2PasswordBearer (awnsers, me)`

**Corpo da requisição (exemplo resumido):**
```
json
{
  "usr_email": "user@example.com",
  "ans_prompt": "prompt usado",
  "ans_llm_answer": "resposta gerada",
  "ans_llm_model": "modelo usado",
  "ans_relevancia_resposta_justify": "texto justificando",
  "ans_relevancia_resposta_pontuation": 5,
  "...": "demais critérios de avaliação",
  "ans_prefered_answer": "LLM 1",
  "ans_prefered_answer_justify": "justificativa da escolha"
}
```

**Resposta `201`:**
```
json
{}
```

---

## 👤 Usuário

---

### `GET /user`
**Descrição:**  
Retorna a lista completa de usuários registrados no sistema. Inclui nome, e-mail, status ativo e se o usuário é administrador.

**Segurança:** `OAuth2PasswordBearer (users, me)`

**Resposta `200`:**
```
json
[
  {
    "usr_name": "string",
    "usr_email": "string",
    "usr_is_adm": true,
    "usr_is_active": true,
    "created_at": "datetime"
  }
]
```

---

### `POST /user`
**Descrição:**  
Cria um novo usuário no sistema com as informações obrigatórias, incluindo senha e permissões.

**Segurança:** `OAuth2PasswordBearer (users, me)`

**Corpo da requisição:**
```
json
{
  "usr_name": "string",
  "usr_email": "string",
  "usr_is_adm": true,
  "usr_is_active": true,
  "usr_password": "string"
}
```

**Resposta `200`:**
```
json
{
  "usr_name": "string",
  "usr_email": "string",
  "usr_is_adm": true,
  "usr_is_active": true,
  "created_at": "datetime"
}
```

---

### `GET /user/me/`
**Descrição:**  
Retorna os dados do usuário atualmente autenticado. Essa rota é útil para exibir as próprias informações de perfil.

**Segurança:** `OAuth2PasswordBearer (me)`

**Resposta `200`:**
```
json
{
  "usr_name": "string",
  "usr_email": "string",
  "usr_is_adm": true,
  "usr_is_active": true,
  "created_at": "datetime"
}
```

---

### `PUT /user/{usr_email}`
**Descrição:**  
Atualiza os dados de um usuário específico identificado pelo seu e-mail. Pode alterar nome, e-mail, status, senha e privilégios administrativos.

**Segurança:** `OAuth2PasswordBearer (users, me)`

**Parâmetro na URL:**
- `usr_email`: string (obrigatório)

**Corpo da requisição:**
```
json
{
  "usr_name": "string | null",
  "usr_email": "string | null",
  "usr_password": "string | null",
  "usr_is_adm": true,
  "usr_is_active": true
}
```

**Resposta `200`:**
```
json
{
  "usr_name": "string",
  "usr_email": "string",
  "usr_is_adm": true,
  "usr_is_active": true,
  "created_at": "datetime"
}
```

---

### `PATCH /user/`
**Descrição:**  
Atualiza os dados do próprio usuário autenticado. Permite mudanças parciais como nome ou senha.

**Segurança:** `OAuth2PasswordBearer (me)`

**Corpo da requisição:**
```
json
{
  "usr_name": "string | null",
  "usr_password": "string | null"
}
```

**Resposta `200`:**
```
json
{
  "usr_name": "string",
  "usr_email": "string",
  "usr_is_adm": true,
  "usr_is_active": true,
  "created_at": "datetime"
}
```

---

## 🔐 Autenticação

---

### `POST /token`
**Descrição:**  
Realiza a autenticação de um usuário utilizando `username` e `password`, conforme o padrão OAuth2 com grant type `password`. Retorna um token JWT (JSON Web Token) que pode ser usado para acessar rotas protegidas da API.

**Corpo da requisição (form-urlencoded):**
```
text
grant_type=password  
username=string  
password=string  
scope=  
client_id=  
client_secret=
```

**Resposta `200`:**
```
json
{
  "access_token": "string",
  "token_type": "bearer"
}
```

---

## 🌱 Root

---

### `GET /`
**Descrição:**  
Endpoint raiz da API, geralmente utilizado como teste de disponibilidade. Pode retornar uma mensagem simples ou objeto vazio.

**Resposta `200`:**
```
json
{}
```
