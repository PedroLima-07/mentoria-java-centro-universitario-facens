# 🏋️‍♂️ Exercícios: Dominando o Do-While

Agora que você aprendeu a usar o `do-while` e o `Scanner`, seus programas vão ganhar vida! Crie os arquivos `.java` e prepare-se para digitar bastante no terminal.

---

### 🔐 Exercício 1: O Cofre

**Arquivo:** `Senha.java`

**Cenário:** Você está programando o bloqueio de tela de um celular. O celular deve pedir a senha repetidas vezes até que o usuário acerte.

**O que você deve fazer:**

1. Importe o `Scanner` para ler o teclado.
2. Defina uma variável com a senha correta (ex: `int senhaCerta = 1234;`).
3. Crie uma variável `int senhaDigitada;` (sem valor inicial).
4. Use o `do-while` para pedir: _"Digite a senha:"_ e ler o número que o usuário digitar.
5. O laço deve repetir **enquanto** a `senhaDigitada` for **diferente** da `senhaCerta`.
6. Quando o laço terminar, imprima: _"Acesso Permitido!"_

---

### 🎲 Exercício 2: Jogo de Adivinhação

**Arquivo:** `Adivinhacao.java`

**Cenário:** O computador pensou em um número de 1 a 10 e você precisa adivinhar.

**O que você deve fazer:**

1. Defina um número secreto (ex: `int numeroSecreto = 7;`).
2. Crie uma variável `int palpite;`.
3. Use um `do-while` para perguntar o palpite do usuário e ler o teclado.
4. Dentro do laço, se o palpite for errado, dê uma dica usando `if/else` ("Tente um número maior" ou "Tente um número menor").
5. O laço repete **enquanto** o palpite for diferente do número secreto.
6. Fora do laço, imprima: _"Parabéns, você acertou!"_

---

### 🍕 Desafio: Pedido de Lanchonete

**Arquivo:** `Lanchonete.java`

**Cenário:** Crie um sistema de pedidos onde o cliente pode escolher vários itens.

**O que você deve fazer:**

1. Mostre um menu simples:
   - 1. Hamburguer (R$ 20.0)
   - 2. Refri (R$ 5.0)
   - 0. Finalizar Pedido
2. Crie uma variável `double totalConta = 0.0;` e `int escolha;`.
3. Use o `do-while` para ler a escolha do usuário.
4. Se ele escolher 1, some 20.0 na conta. Se escolher 2, some 5.0.
5. Repita o menu **enquanto** a escolha for diferente de 0.
6. No final, mostre o valor total do pedido.

---

### 💬 Precisa de ajuda com este módulo?

Ficou confuso ou o código deu erro? Lembre-se de que a mentoria está aqui exatamente para isso! Consulte os nossos canais de contato disponíveis lá no **Canvas** e mande sua dúvida. Estou aqui para te ajudar a avançar! 💪
