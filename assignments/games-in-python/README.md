
# 📘 Assignment: Jogo da Forca

## 🎯 Objetivo

Construir o clássico jogo de adivinhar palavras usando strings, loops, condicionais, seleção aleatória e entrada de dados do usuário em Python.

## 📝 Tarefas

### 🛠️ Sortear Palavra e Mostrar o Progresso

#### Descrição
Crie uma lista com pelo menos 5 palavras, sorteie uma delas a cada partida com `random.choice()` e mostre o progresso da palavra oculta.

#### Requisitos
O programa concluído deve:

- Sortear uma palavra diferente da lista a cada nova partida
- Exibir a palavra oculta com um `_` por letra, por exemplo `_ _ _ _ _` para `PYTHON`
- Substituir o `_` pela letra sempre que o palpite estiver correto


### 🛠️ Receber Palpites e Controlar Tentativas

#### Descrição
Peça ao jogador uma letra por vez e controle quantos erros ainda são permitidos (sugestão: 6 tentativas).

#### Requisitos
O programa concluído deve:

- Aceitar apenas uma letra por palpite e rejeitar entradas inválidas com uma mensagem
- Reduzir em 1 o número de tentativas restantes a cada letra errada
- Exibir as tentativas restantes após cada palpite
- Não descontar tentativas por letras já digitadas antes


### 🛠️ Encerrar a Partida com Vitória ou Derrota

#### Descrição
Finalize o jogo quando a palavra for totalmente revelada ou quando as tentativas chegarem a zero, mostrando a mensagem correspondente.

#### Requisitos
O programa concluído deve:

- Exibir a mensagem de vitória quando todas as letras forem reveladas
- Exibir a mensagem de derrota com a palavra correta quando as tentativas chegarem a zero
- Encerrar o programa logo após a mensagem final

#### Exemplo de Saída
```text
Palavra: _ _ _ _ _ _
Letra: p
Palavra: P _ _ _ _ _
Tentativas restantes: 6
```