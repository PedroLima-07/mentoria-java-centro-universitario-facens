# 🏋️‍♂️ Exercícios: Dominando o Laço While

Agora é a sua vez! Lembre-se da regra de ouro do `while`: **sempre modifique a variável dentro do laço para não criar um loop infinito!**

Crie os arquivos `.java` no seu VS Code e resolva os desafios abaixo.

---

### ⏱️ Exercício 1: O Cronômetro de Bomba

**Arquivo:** `BombaRelogio.java`

**Cenário:** Você precisa criar um contador regressivo para desarmar uma bomba simulada. O `for` seria fácil, mas o desafio aqui é usar o `while`.

**O que você deve fazer:**

1. Crie uma variável `int tempo = 10;`.
2. Crie um laço `while` que continue rodando **enquanto** o tempo for maior ou igual a zero.
3. Dentro do laço, imprima o tempo restante.
4. Lembre-se de diminuir o tempo (`tempo--`) a cada volta.
5. Quando o laço acabar, imprima "Bomba desarmada com sucesso!".

---

### 💰 Exercício 2: Meta de Economia

**Arquivo:** `Poupanca.java`

**Cenário:** Você quer comprar um videogame que custa R$ 3.000,00. Todo mês você consegue guardar R$ 450,00. Quantos meses você vai levar para conseguir o dinheiro?

**O que você deve fazer:**

1. Crie as variáveis `double saldo = 0;`, `double meta = 3000.0;` e `int meses = 0;`.
2. Crie um `while` que repita o código **enquanto** o saldo for **menor** que a meta.
3. Dentro do laço:
   - Adicione R$ 450.00 ao saldo.
   - Adicione 1 à variável meses (para contar que passou um mês).
4. No final, **fora do laço**, imprima quantos meses demorou e qual foi o saldo final (que vai passar um pouquinho de 3000).

---

### 🐉 Desafio: Batalha de RPG

**Arquivo:** `BatalhaRPG.java`

**Cenário:** Você está programando o combate de um jogo. O herói ataca um dragão repetidas vezes até o monstro ser derrotado.

**Dados:**

- O Dragão tem 500 de HP (Vida).
- O Herói causa 45 de dano por ataque.
- Queremos saber quantos ataques o herói precisou para vencer.

**O que você deve fazer:**

1. Crie `int hpDragao = 500;` e `int ataques = 0;`.
2. O combate continua **enquanto** o HP do dragão for maior que 0.
3. A cada rodada (dentro do `while`):
   - Subtraia 45 do HP do dragão.
   - Aumente a contagem de ataques em 1.
   - Imprima algo como: "Herói atacou! HP do Dragão: X".
4. Fora do laço, imprima: "Dragão derrotado em X ataques!".

---

### 💬 Precisa de ajuda com este módulo?

Ficou confuso ou o código deu erro? Lembre-se de que a mentoria está aqui exatamente para isso! Consulte os nossos canais de contato disponíveis lá no **Canvas** e mande sua dúvida. Estou aqui para te ajudar a avançar! 💪
