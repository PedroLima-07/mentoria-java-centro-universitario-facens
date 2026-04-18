# 🔄 Estrutura For (Para): O Contador Oficial

Sabe quando você vai na academia e o instrutor fala: _"Faça 3 séries de 10 repetições"_? Ele te deu um ponto de partida, um limite e de quanto em quanto você deve contar.

Na programação, quando **já sabemos exatamente quantas vezes** queremos que o código repita, usamos a estrutura `for` (que significa "para").

Ele é perfeito para contagens, tabuadas e, no futuro, para ler listas de dados!

---

## ✍️ A Anatomia do For

O `for` pode parecer meio feio na primeira vez que você bate o olho, mas ele é super organizado. Ele obriga você a colocar as 3 regras da repetição na mesma linha, separadas por ponto e vírgula `;`.

```java
for (1. Início ; 2. Condição de parada ; 3. Passo) {
    // Código que vai repetir
}
Traduzindo para o Java:

Início (Inicialização): Onde a contagem começa? (Ex: int i = 1)

Condição: Até quando ele deve repetir? (Ex: i <= 5)

Passo (Incremento): Ele conta de 1 em 1? De 2 em 2? (Ex: i++, que é o atalho para i = i + 1)

💻 Exemplo Prático: Contando até 5
Veja como é simples pedir para o Java contar de 1 até 5:

Java
public class Contador {
    public static void main(String[] args) {

        System.out.println("Iniciando a contagem...");

        // Lemos assim: "Para um i começando em 1; enquanto i for menor ou igual a 5; aumente i em 1"
        for (int i = 1; i <= 5; i++) {
            System.out.println("Número: " + i);
        }

        System.out.println("Fim da contagem!");
    }
}
💡 Por que sempre usamos a letra i?
É uma tradição antiga na programação! O i vem de Índice ou Iterador (aquele que repete). Mas você pode usar qualquer nome, como int contador = 1;.

📉 Contagem Regressiva (De trás pra frente)
O for também sabe contar para trás! Basta começar com um número maior, mudar a condição para "maior que", e usar o decremento i-- (que tira 1 a cada volta).

Java
for (int i = 10; i > 0; i--) {
    System.out.println("Faltam " + i + " segundos!");
}
Pronto para testar a sua lógica de repetição? Vá para o arquivo exercicios.md!


---

### 💬 Precisa de ajuda com este módulo?

Ficou confuso ou o código deu erro? Lembre-se de que a mentoria está aqui exatamente para isso! Consulte os nossos canais de contato disponíveis lá no **Canvas** e mande sua dúvida. Estou aqui para te ajudar a avançar! 💪
```
