# 📦 Módulo 01: Variáveis e Tipos de Dados em Java

Agora que seu ambiente está configurado e você já fez o computador dizer "Olá, Mundo!", vamos entender como os programas guardam informações.

---

## 🎯 O que você vai aprender

- O que são variáveis
- Como criar variáveis em Java
- Tipos de dados básicos
- Boas práticas de nomeação
- Como juntar textos e variáveis (Concatenação)

---

## 🧠 Conceito: O que é uma variável?

Pense na memória do seu computador como um grande armazém. Uma **variável** é como uma **caixa** dentro desse armazém onde você guarda um dado.

Toda caixa precisa de três coisas:

1. **Tipo:** O formato da caixa (é para guardar números? textos?).
2. **Nome (Etiqueta):** Para você achar a caixa depois.
3. **Valor:** O que tem dentro da caixa.

---

## ✍️ Como declarar uma variável

A "fórmula" para criar essa caixa em Java é sempre a mesma:

```java
tipo nome = valor;
Exemplo na prática:

Java
int idade = 20;
String nome = "Pedro";
double altura = 1.75;

🔢 Tipos de dados mais usados no dia a dia
Existem vários tipos de caixas, mas no início vamos focar nos "Quatro Fantásticos":

🔹 Números inteiros (int)
Serve para idades, quantidades, anos.

int idade = 20;

🔹 Números com casas decimais (double)
Serve para dinheiro, altura, peso. (Atenção: em Java usamos ponto ., não vírgula ,)

double altura = 1.75;

🔹 Texto (String)
Serve para nomes, frases, senhas. O texto deve estar sempre entre aspas duplas "".
(Dica de Ouro: Note que String começa com a letra 'S' MAIÚSCULA, enquanto os outros são minúsculos!)

String nome = "Pedro";

🔹 Booleano (boolean)
Só aceita dois valores: true (verdadeiro) ou false (falso).

boolean estudante = true;

🔄 Variáveis podem... variar!
O legal das variáveis é que você pode trocar o que tem dentro da caixa a qualquer momento no seu código:

Java
int pontuacao = 10;

// ops, ganhei mais pontos!
pontuacao = 15;

// Agora a caixa 'pontuacao' não vale mais 10, vale 15.

-----

📏 Regras e Boas Práticas para Nomes
Para dar nome às suas caixas, existem regras:

❌ Não pode começar com número: 1idade

❌ Não usar espaços: nome completo

✅ Use nomes claros: idade, valorTotal

✅ Use o padrão camelCase: Quando juntar duas palavras, a primeira começa minúscula e a segunda maiúscula. Ex: valorDaCompra, nomeDoAluno.

------

🧩 O "Pulo do Gato": Juntando Texto e Variável (Concatenação)
E se você quiser que o comando System.out.println imprima uma frase bonitinha usando suas variáveis? Usamos o símbolo de soma + para "colar" as coisas!

Java
String nome = "Pedro";
int idade = 20;

// O símbolo + serve como uma "cola" juntando o texto com o valor da variável
System.out.println("Olá, meu nome é " + nome + " e eu tenho " + idade + " anos.");
💻 Exemplo completo
Se você copiar e colar este código no seu VS Code, vai ver a mágica acontecer:

Java
public class Variaveis {
    public static void main(String[] args) {
        String nome = "Maria";
        int idade = 25;
        double altura = 1.68;
        boolean gostaDeCafe = true;

        System.out.println("Ficha de Cadastro:");
        System.out.println("Nome: " + nome);
        System.out.println("Idade: " + idade);
        System.out.println("Altura: " + altura + "m");
    }
}

------

🧪 Hora de Praticar!
Chegou a sua vez de colocar a mão na massa. Crie um arquivo chamado MeusDados.java e resolva os exercícios abaixo.

Exercício 1
Crie variáveis com os tipos corretos para armazenar:

O seu nome

A sua idade

A sua altura

Se você gosta de programar (Verdadeiro ou Falso)

Mostre os valores no console usando System.out.println().

🚀 Desafio Final
Usando o que você aprendeu sobre concatenação (juntar textos e variáveis com o +), crie um programa que imprima exatamente esta frase no terminal, substituindo as letras pelas suas variáveis:

"Meu nome é X, tenho Y anos e minha altura é Z."

(💡 Se travar, não tem problema! Dá uma espiada na pasta resolucoes/ para ver como o código foi construído).
```
