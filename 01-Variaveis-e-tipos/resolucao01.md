# ✅ Gabarito: Módulo 01 - Variáveis e Tipos

Se você chegou até aqui, **parabéns por ter tentado!** É super normal travar no começo. A programação é como aprender um novo idioma: no início, a gente tropeça nas palavras (ou nas chaves e pontos e vírgulas rs), mas com a prática tudo fica natural.

Lembre-se: na programação, muitas vezes existe mais de uma maneira de chegar ao mesmo resultado. Se o seu código funcionou e exibiu os dados corretamente, você acertou! Abaixo estão as nossas sugestões de resolução.

---

## 🛠️ Resolução: Exercício 1 (MeusDados.java)

**O objetivo:** Criar variáveis com os tipos corretos para nome, idade, altura e se gosta de programar, e depois imprimir tudo.

**Como resolvemos:**

```java
public class MeusDados {
    public static void main(String[] args) {

        // 1. O seu nome é um TEXTO, então usamos a caixa do tipo String.
        // Lembre-se: String começa com 'S' maiúsculo e o texto fica entre aspas duplas!
        String nome = "Carlos";

        // 2. A sua idade é um número INTEIRO (ninguém tem 20.5 anos), então usamos int.
        int idade = 28;

        // 3. A sua altura tem casas decimais, então usamos double.
        // Lembre-se: no Java usamos ponto (.) ao invés de vírgula (,).
        double altura = 1.82;

        // 4. Se gosta de programar é uma pergunta de SIM ou NÃO (Verdadeiro ou Falso).
        // Para isso, a caixa perfeita é a boolean.
        boolean gostaDeProgramar = true;

        // Agora, usamos o comando System.out.println para mostrar tudo na tela:
        System.out.println("--- Meus Dados ---");
        System.out.println(nome);
        System.out.println(idade);
        System.out.println(altura);
        System.out.println(gostaDeProgramar);
    }
}
```

## 🚀 Resolução: Desafio Final

O objetivo: Usar a concatenação (o sinal de +) para montar a frase: "Meu nome é X, tenho Y anos e minha altura é Z."

Como resolvemos:

```java
public class DesafioFinal {
    public static void main(String[] args) {

        // Primeiro, criamos as nossas variáveis (as nossas caixas com os dados)
        String nome = "Ana";
        int idade = 22;
        double altura = 1.65;

        // Agora vem a mágica da concatenação!
        // Note que deixamos um espaço em branco antes de fechar as aspas em "Meu nome é "
        // para que o nome não fique grudado na palavra. O mesmo vale para o resto da frase.

        System.out.println("Meu nome é " + nome + ", tenho " + idade + " anos e minha altura é " + altura + ".");

    }
}
```

💡 Dica do Mentor: O Erro do "Texto Grudado"
Um erro muito comum no começo é esquecer os espaços dentro das aspas.
Se você fizer isso: "Meu nome é" + nome
O resultado será: Meu nome éAna (Tudo junto!).

Sempre confira se você deixou um espaço vazio dentro das aspas para dar um respiro entre as palavras!
