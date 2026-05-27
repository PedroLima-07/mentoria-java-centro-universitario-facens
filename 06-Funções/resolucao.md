# ✅ Gabarito: Funções em Java

Parabéns por chegar até aqui! 🎉

Funções são um dos conceitos mais importantes da programação. Elas ajudam a dividir o problema em pequenas partes e deixam o código muito mais organizado.

Confira as resoluções abaixo:

---

# 📝 Resolução: Exercício 1 (BoasVindas.java)

## Como resolvemos:

Criamos uma função do tipo `void`, porque ela apenas mostra uma mensagem e não precisa devolver nenhum valor.

```java
public class BoasVindas {

    public static void mostrarMensagem() {
        System.out.println("Bem-vindo ao sistema escolar!");
    }

    public static void main(String[] args) {

        mostrarMensagem();

    }
}
```

---

# 📊 Resolução: Exercício 2 (Calculadora.java)

## Como resolvemos:

Criamos uma função que recebe dois números como parâmetros e devolve a soma usando `return`.

```java
public class Calculadora {

    public static int somar(int a, int b) {

        int resultado = a + b;

        return resultado;
    }

    public static void main(String[] args) {

        int total = somar(10, 5);

        System.out.println("Resultado: " + total);

    }
}
```

---

# 🎓 Resolução: Exercício 3 (MediaAluno.java)

## Como resolvemos:

A função recebe duas notas do tipo `double` e retorna a média delas.

```java
public class MediaAluno {

    public static double calcularMedia(double nota1, double nota2) {

        double media = (nota1 + nota2) / 2;

        return media;
    }

    public static void main(String[] args) {

        double nota1 = 8.5;
        double nota2 = 7.0;

        double resultado = calcularMedia(nota1, nota2);

        System.out.println("Nota 1: " + nota1);
        System.out.println("Nota 2: " + nota2);
        System.out.println("Média final: " + resultado);

    }
}
```

---

# 🚀 Resolução: Desafio (NumeroPar.java)

## Como resolvemos:

Usamos o operador `%` para descobrir o resto da divisão.

Se o resto da divisão por 2 for igual a 0, o número é par.

```java
public class NumeroPar {

    public static void verificarPar(int numero) {

        if (numero % 2 == 0) {

            System.out.println(numero + " é um número par");

        } else {

            System.out.println(numero + " é um número ímpar");

        }
    }

    public static void main(String[] args) {

        verificarPar(10);
        verificarPar(7);
        verificarPar(24);

    }
}
```

---

# 🏆 Conclusão

Agora você já consegue:
- criar funções,
- usar parâmetros,
- retornar valores,
- e organizar melhor seus programas.

Esses conceitos serão usados praticamente em TODOS os sistemas reais 😄