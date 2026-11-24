# 📘 Assignment: Criando APIs REST com FastAPI

## 🎯 Objetivo

Construir uma API REST com FastAPI, criando rotas GET e POST, validando dados com Pydantic e retornando erros HTTP adequados.

## 📝 Tarefas

### 🛠️ Criar a Primeira Rota

#### Descrição
Instale o FastAPI e o Uvicorn, depois crie as rotas `GET /` e `GET /health` no arquivo `main.py`.

#### Requisitos
O programa concluído deve:

- Iniciar com `uvicorn main:app --reload` sem erros
- Responder `GET /` com o JSON `{"message": "Bem-vindo à API"}`
- Responder `GET /health` com o JSON `{"status": "ok"}`


### 🛠️ Receber Dados com Pydantic

#### Descrição
Crie um modelo `Tarefa` com Pydantic e uma lista em memória para armazenar as tarefas recebidas pela API.

#### Requisitos
O programa concluído deve:

- Definir o modelo `Tarefa` com os campos `id` (int), `titulo` (str) e `concluida` (bool, com padrão `False`)
- Responder `POST /tarefas` com status `201` e a tarefa criada
- Responder `GET /tarefas` com a lista de todas as tarefas
- Retornar erro `422` automaticamente quando o `titulo` for enviado sem texto ou com tipo incorreto


### 🛠️ Buscar, Atualizar e Tratar Erros

#### Descrição
Implemente as rotas para buscar e remover uma tarefa pelo `id`, tratando os casos em que ela não existe.

#### Requisitos
O programa concluído deve:

- Responder `GET /tarefas/{id}` com status `200` quando a tarefa existir
- Responder com status `404` e a mensagem `"Tarefa não encontrada"` quando o `id` não existir
- Responder `DELETE /tarefas/{id}` com status `204` ao remover uma tarefa existente
- Verificar a documentação interativa em `/docs` e testar todas as rotas por ela

#### Exemplo de Saída
```text
POST /tarefas  {"id": 1, "titulo": "Estudar FastAPI"}
→ 201 {"id": 1, "titulo": "Estudar FastAPI", "concluida": false}

GET /tarefas/2
→ 404 {"detail": "Tarefa não encontrada"}
```
