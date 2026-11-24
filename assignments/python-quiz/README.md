# 📘 Assignment: Quiz Interativo em Python

## 🎯 Objetivo

Construir um quiz interativo usando funções, listas e dicionários para organizar perguntas, verificar respostas e calcular a pontuação.

## 📝 Tarefas

### 🛠️ Exibir uma Pergunta

#### Descrição
Complete a função `exibir_pergunta` para mostrar o texto de uma pergunta e suas opções numeradas, lidas de um dicionário.

#### Requisitos
O programa concluído deve:

- Receber um dicionário com as chaves `"pergunta"` e `"opcoes"`
- Mostrar a pergunta seguida de cada opção numerada a partir de 1
- Ler a escolha do aluno e retornar o número digitado


### 🛠️ Verificar a Resposta

#### Descrição
Complete a função `verificar_resposta` para comparar a escolha do aluno com a resposta correta guardada no dicionário.

#### Requisitos
O programa concluído deve:

- Receber o dicionário da pergunta e a escolha do aluno
- Retornar `True` quando a escolha corresponder à chave `"resposta"` e `False` caso contrário
- Considerar que `"resposta"` é o índice da opção na lista, começando em 0
- Mostrar `"Correto!"` ou `"Errado!"` após cada resposta


### 🛠️ Executar o Quiz Completo

#### Descrição
Complete a função `main` para percorrer a lista de perguntas, contar os acertos e mostrar o resultado final.

#### Requisitos
O programa concluído deve:

- Percorrer todas as perguntas da lista `perguntas` usando as funções já criadas
- Contar a quantidade de acertos
- Exibir ao final a mensagem `"Você acertou X de Y perguntas"`

#### Exemplo de Saída
```text
Qual palavra-chave define uma função em Python?
1. func
2. def
3. function
4. define
Escolha: 2
Correto!

Você acertou 1 de 1 perguntas
```
