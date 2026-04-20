# 🔄 Estrutura While: Repetindo "Enquanto..."

No módulo passado, vimos o `for`. Ele é ótimo quando sabemos _exatamente_ quantas vezes queremos repetir algo (ex: contar de 1 a 10).

Mas e se você não souber a quantidade exata? Imagine um jogo de videogame: você não sabe quantos passos o jogador vai dar, mas sabe que o jogo deve continuar **enquanto** o personagem estiver vivo.

É para isso que usamos a estrutura **`while`** (que significa "enquanto").

---

## ✍️ A Anatomia do While

A estrutura do `while` é muito parecida com a do `if`. A diferença é que o `if` checa a condição, roda o código uma vez e vai embora. O `while` checa a condição, roda o código, e **volta para o começo** para checar de novo!

```java
int vida = 3;

// Lemos assim: "Enquanto a vida for maior que zero..."
while (vida > 0) {
    System.out.println("O jogador está vivo!");

    // IMPORTANTE: Alguma coisa precisa acontecer para diminuir a vida,
    // senão o jogo nunca acaba!
    vida--;
}
```

## 🚨 O Perigo Oculto: O Loop Infinito!

O maior erro de todo programador iniciante (e até dos experientes rs) é criar um loop infinito.
Se você esquecer de atualizar a variável que está sendo testada na condição do while, a condição será sempre verdadeira e o programa vai rodar para sempre (ou até o computador travar).

Exemplo de um desastre:

```java
int bateria = 100;

while (bateria > 0) {
    System.out.println("Celular ligado!");
    // Esqueceu de colocar bateria-- aqui! O celular terá 100% de bateria para sempre.
}
```

## 💻 Exemplo Prático: Comendo uma Pizza

Vamos simular alguém comendo uma pizza inteira. Não sabemos quantas mordidas vai levar, só sabemos que a pessoa vai continuar comendo enquanto houver fatias!

```java
public class ComendoPizza {
    public static void main(String[] args) {

        int fatias = 8;

        System.out.println("A pizza chegou! Temos " + fatias + " fatias.");

        while (fatias > 0) {
            System.out.println("Comi uma fatia! 🍕");
            fatias--; // Diminui 1 fatia da caixa

            System.out.println("Fatias restantes: " + fatias);
        }

        System.out.println("Acabou a pizza! Estou cheio.");
    }
}
```

Pronto para testar se você entendeu a lógica do "Enquanto"? Vá para o arquivo exercicios.md!

---

### 💬 Precisa de ajuda com este módulo?

Ficou confuso ou o código deu erro? Lembre-se de que a mentoria está aqui exatamente para isso! Consulte os nossos canais de contato disponíveis lá no **Canvas** e mande sua dúvida. Estou aqui para te ajudar a avançar! 💪
