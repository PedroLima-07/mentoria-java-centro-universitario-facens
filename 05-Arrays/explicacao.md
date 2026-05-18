# 📦 Módulo 05: Arrays (Vetores) em Java

Até agora, nossas variáveis eram como "caixas pequenas" que guardavam um único valor por vez. Se quiséssemos guardar a nota de 5 alunos, teríamos que criar 5 variáveis diferentes (`nota1`, `nota2`, `nota3`...). Imagina fazer isso para uma escola com 1000 alunos? Impossível!

É para resolver esse problema que existem os **Arrays** (também chamados de Vetores).

Um Array é como um **armário com várias gavetas numeradas**. Ele guarda vários valores do _mesmo tipo_ dentro de uma única variável.

---

## ✍️ Como criar um Array em Java?

Existem duas formas principais de criar esse "armário" no Java:

### Forma 1: Criando o armário vazio (sabendo o tamanho)

Se você sabe quantas gavetas precisa, mas ainda não tem os valores, você cria o Array dizendo o tamanho dele usando a palavra `new`.

```java
// Cria um array de números inteiros com 5 espaços (gavetas) vazios
int[] idades = new int[5];
Forma 2: Criando o armário já com as coisas dentro
Se você já sabe quais valores quer guardar logo de cara, pode colocar tudo entre chaves { }. O Java descobre o tamanho sozinho!
```

```java
// Cria um array de textos (String) já com 3 nomes
String[] nomes = {"Ana", "Carlos", "Beatriz"};
```

### 🚨 A Regra de Ouro: O índice começa no ZERO!

Na vida real, nós começamos a contar do 1. Na programação, nós começamos a contar do ZERO.
O número da gaveta é chamado de índice (ou index).

Se o seu array tem tamanho 3, as gavetas são: 0, 1 e 2.

```java
String[] nomes = {"Ana", "Carlos", "Beatriz"};

System.out.println(nomes[0]); // Imprime "Ana"
System.out.println(nomes[1]); // Imprime "Carlos"
System.out.println(nomes[2]); // Imprime "Beatriz"

// System.out.println(nomes[3]); -> ❌ ERRO! Essa gaveta não existe!
```

### ✏️ Guardando e alterando valores

Para colocar ou trocar um valor dentro de uma gaveta, basta chamar o nome do array, abrir colchetes [ ] com o número do índice e usar o sinal de igual =.

```java
int[] notas = new int[3]; // Armário com 3 gavetas vazias

notas[0] = 8;  // Guarda 8 na primeira gaveta
notas[1] = 10; // Guarda 10 na segunda gaveta
notas[2] = 5;  // Guarda 5 na terceira gaveta

notas[2] = 7;  // Ops, o aluno recuperou a nota! Trocando o 5 por 7.
```

### 🔄 O Pulo do Gato: Arrays + Laço For

Os Arrays e o laço for (que aprendemos no módulo passado) foram feitos um para o outro! Em vez de imprimir gaveta por gaveta manualmente, nós usamos o for para percorrer o array inteiro.

Para não precisarmos adivinhar o tamanho do array, o Java nos dá uma ferramenta mágica chamada .length (comprimento), que diz exatamente quantas gavetas o array tem.

```java
public class PercorrendoArray {
    public static void main(String[] args) {

        String[] frutas = {"Maçã", "Banana", "Uva", "Morango"};

        // O 'i' começa no 0 (primeira gaveta)
        // Vai até antes do frutas.length (tamanho do array, que é 4)
        for (int i = 0; i < frutas.length; i++) {
            System.out.println("Fruta na posição " + i + ": " + frutas[i]);
        }
    }
}
```

Pronto para organizar seus dados em Arrays? Vá para o arquivo exercicios.md e coloque a mão na massa!
