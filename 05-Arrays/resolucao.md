# ✅ Gabarito: Arrays em Java

Parabéns por chegar até aqui! Trabalhar com Arrays exige muita atenção aos detalhes, principalmente para não tentar acessar uma "gaveta" que não existe (o famoso erro `ArrayIndexOutOfBoundsException`).

Confira as soluções passo a passo:

---

## 📝 Resolução: Exercício 1 (Chamada.java)

**Como resolvemos:**
Usamos a criação direta com chaves `{}` e o `.length` no `for` para garantir que o Java leia todos os nomes, independente de quantos sejam.

```java
public class Chamada {
    public static void main(String[] args) {

        // 1. Criando o array já com os valores
        String[] alunos = {"Lucas", "Mariana", "Roberto", "Fernanda", "Diego"};

        System.out.println("--- Lista de Presença ---");

        // 2. O laço for começando do índice 0
        for (int i = 0; i < alunos.length; i++) {
            System.out.println("Bem-vindo(a), " + alunos[i] + "!");
        }
    }
}
```

## 📊 Resolução: Exercício 2 (Boletim.java)

Como resolvemos:
O segredo aqui é usar a variável soma como um acumulador dentro do laço for, exatamente como fizemos no módulo passado, mas agora pegando os valores de dentro do Array.

```java
public class Boletim {
    public static void main(String[] args) {

        double[] notas = {8.5, 7.0, 9.0, 5.5};
        double soma = 0;

        // Percorre o array e soma cada nota
        for (int i = 0; i < notas.length; i++) {
            soma = soma + notas[i]; // Ou soma += notas[i];
        }

        // Calcula a média usando o tamanho dinâmico do array
        double media = soma / notas.length;

        System.out.println("Soma das notas: " + soma);
        System.out.println("Média final: " + media);
    }
}
```

## 🚀 Resolução: Desafio (MaiorNumero.java)

Como resolvemos:
Esta é uma lógica clássica de programação! Assumimos que o primeiro número (índice 0) é o maior. Depois, olhamos para os outros. Se algum for maior do que o que temos guardado, nós atualizamos o título de "maior".

```java
public class MaiorNumero {
    public static void main(String[] args) {

        int[] pontuacoes = {45, 89, 32, 104, 77};

        // Assumimos que o recorde inicial é o primeiro valor do array
        int maior = pontuacoes[0];

        // Podemos até começar o 'i' no 1, já que o 0 já está na variável 'maior',
        // mas começar no 0 também funciona perfeitamente!
        for (int i = 0; i < pontuacoes.length; i++) {

            // Se o valor da gaveta atual for maior que o recorde...
            if (pontuacoes[i] > maior) {
                maior = pontuacoes[i]; // ...atualizamos o recorde!
            }
        }

        System.out.println("🏆 O recorde do jogo é: " + maior);
    }
}
```
