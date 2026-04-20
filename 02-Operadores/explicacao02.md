# 🧮 Módulo 02: Operadores em Java

No módulo anterior, aprendemos a criar variáveis (nossas caixas) e guardar informações nelas. Mas um programa de verdade precisa fazer cálculos, comparar valores e tomar decisões. É aqui que entram os **Operadores**!

Pense nos operadores como as "ações" que acontecem entre as nossas variáveis.

---

## 🎯 O que você vai aprender

- Operadores Aritméticos (Matemática básica)
- O perigoso (mas útil) operador de Resto (`%`)
- Operadores de Atribuição (Atalhos)
- Operadores Relacionais (Fazendo perguntas de Sim/Não)
- Operadores Lógicos (Juntando condições)

---

## ➕ 1. Operadores Aritméticos (Matemática)

Esses são os que você já conhece da escola. Eles pegam números, fazem uma conta e devolvem um novo número.

- `+` : Soma
- `-` : Subtração
- `*` : Multiplicação (usamos o asterisco, e não o "x")
- `/` : Divisão
- `%` : Módulo (Resto da divisão)

**Exemplo prático:**

```java
int a = 10;
int b = 3;

System.out.println(a + b); // Imprime 13
System.out.println(a - b); // Imprime 7
System.out.println(a * b); // Imprime 30
System.out.println(a / b); // Imprime 3 (Como são inteiros, ele ignora os decimais)
```

💡 Atenção ao Módulo (%)!
Ele não é porcentagem! Ele pega o resto da divisão.
Exemplo: Se você tem 10 fatias de pizza e divide para 3 pessoas, cada um come 3 fatias e sobra 1.
Logo, 10 % 3 é igual a 1. É muito usado para descobrir se um número é par ou ímpar!

---

## 🔄 2. Operadores de Atribuição (Os Atalhos)

Lembra que o sinal de igual = significa "recebe"? Ele pega o que está na direita e guarda na variável da esquerda.
Mas na programação, muitas vezes queremos atualizar o valor de uma variável baseada nela mesma (ex: ganhar mais pontos num jogo).

Em vez de escrever:
pontos = pontos + 5;

Nós usamos os atalhos:

+= : Soma e guarda (Ex: pontos += 5;)

-= : Subtrai e guarda

\*= : Multiplica e guarda

/= : Divide e guarda

---

## ⚖️ 3. Operadores Relacionais (As Comparações)

Aqui as coisas ficam interessantes. Esses operadores comparam dois valores e a resposta SEMPRE será um valor Booleano (true ou false). É como se você estivesse fazendo uma pergunta ao Java.

== : É igual a? (Atenção: são DOIS sinais de igual!)

!= : É diferente de?

" > : É maior que?

< : É menor que?

" >= : É maior ou igual a?

<= : É menor ou igual a?

Exemplo prático:

```java
int idade = 18;
boolean maiorDeIdade = idade >= 18; // Pergunta: 18 é maior ou igual a 18? SIM (true).

System.out.println("É maior de idade? " + maiorDeIdade); // Imprime true
```

### 🛑 DICA DE OURO DO MENTOR:

Nunca confunda = com ==.
idade = 18 significa "A variável idade AGORA VALE 18".
idade == 18 significa "A variável idade É IGUAL A 18?".

---

## 🧠 4. Operadores Lógicos (Juntando Regras)

Às vezes, uma comparação só não basta. Imagina que para entrar em uma festa você precisa ter ingresso E ser maior de idade. Os operadores lógicos juntam perguntas.

&& (E lógico): Tudo tem que ser verdade.

|| (OU lógico): Basta um ser verdade para tudo ser verdade. (O símbolo é formado por duas barras retas, geralmente perto da tecla Shift/Z).

! (NÃO lógico): Inverte o resultado (se era true, vira false).

Exemplo prático:

```java
boolean temIngresso = true;
int idade = 20;

// Só entra se TIVER ingresso E a idade for MAIOR OU IGUAL a 18
boolean podeEntrar = temIngresso && (idade >= 18);

System.out.println("Pode entrar na festa? " + podeEntrar); // Imprime true
💻 Exemplo Completo
Copie e rode no seu VS Code para ver como tudo se encaixa:

Java
public class Loja {
    public static void main(String[] args) {
        double valorProduto = 100.0;
        int quantidade = 2;

        // 1. Aritmético: Calculando o total
        double total = valorProduto * quantidade; // 200.0

        // 2. Relacional e Lógico: Regra para frete grátis (Acima de 150 reais OU cliente VIP)
        boolean clienteVip = false;
        boolean temFreteGratis = (total > 150.0) || clienteVip;

        System.out.println("Valor total da compra: R$ " + total);
        System.out.println("Tem frete grátis? " + temFreteGratis);
    }
}
```

---

## 🧪 Hora de Praticar!

Chegou a sua vez! Vá para a pasta exercicios e abra o arquivo exercicios.md.
Lá você encontrará os desafios para testar se a lógica dos operadores.

---

### 💬 Precisa de ajuda com este módulo?

Ficou confuso ou o código deu erro? Lembre-se de que a mentoria está aqui exatamente para isso! Consulte os nossos canais de contato disponíveis lá no **Canvas** e mande sua dúvida. Estou aqui para te ajudar a avançar! 💪

```

```
