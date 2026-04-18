# ✅ Gabarito: Módulo 02 - Operadores

Se você chegou até aqui, muito bem! Os operadores exigem um pouco mais de atenção lógica, especialmente quando começamos a misturar matemática com decisões de "Verdadeiro ou Falso".

Lembre-se: não existe apenas um jeito certo de escrever código. Se as suas variáveis têm nomes diferentes ou se você fez o cálculo em uma ordem ligeiramente diferente, mas chegou ao mesmo resultado, **você acertou!**

Abaixo estão as soluções sugeridas para os exercícios.

---

## 🥖 Resolução: Exercício 1 (Padaria.java)

**O objetivo:** Calcular o valor total da compra de cafés e pão de queijo, e depois calcular o troco com base na nota de R$ 50 entregue.

**Como resolvemos:**

```java
public class Padaria {
    public static void main(String[] args) {

        // 1. Criando as variáveis para os preços e quantidades
        // Usamos double porque estamos lidando com dinheiro (casas decimais)
        double precoCafe = 5.50;
        int quantidadeCafe = 3;

        double precoPaoDeQueijo = 12.00;
        int quantidadePaoDeQueijo = 1;

        double dinheiroEntregue = 50.00;

        // 2. Calculando o total
        // Multiplicamos o preço pela quantidade e somamos tudo
        double totalCompra = (precoCafe * quantidadeCafe) + (precoPaoDeQueijo * quantidadePaoDeQueijo);

        // 3. Calculando o troco
        double troco = dinheiroEntregue - totalCompra;

        // 4. Mostrando o resultado
        System.out.println("--- Cupom Fiscal ---");
        System.out.println("Valor Total: R$ " + totalCompra);
        System.out.println("Valor Entregue: R$ " + dinheiroEntregue);
        System.out.println("Troco a devolver: R$ " + troco);
    }
}
🎓 Resolução: Exercício 2 (Escola.java)
O objetivo: Usar operadores relacionais e lógicos para descobrir se o aluno passou, lembrando que ele precisa de nota e de presença.

Como resolvemos:

Java
public class Escola {
    public static void main(String[] args) {

        // 1. Dados do aluno
        double nota1 = 8.5;
        double nota2 = 5.5;
        int frequencia = 80; // 80%

        // 2. Calculando a média
        // Os parênteses são OBRIGATÓRIOS aqui! O Java faz a divisão antes da soma se você não colocar.
        double media = (nota1 + nota2) / 2;

        // 3. Verificando a aprovação
        // Ele precisa da média >= 7.0 "E" (&&) da frequência >= 75
        boolean aprovado = (media >= 7.0) && (frequencia >= 75);

        // 4. Exibindo os resultados
        System.out.println("--- Boletim do Aluno ---");
        System.out.println("Média final: " + media);
        System.out.println("Frequência: " + frequencia + "%");

        // O resultado será false, porque a média (7.0) é atingida, mas se a nota fosse menor, ele reprovaria.
        // Como a nota1 e nota2 dão exatamente média 7.0, a resposta será true!
        System.out.println("Aluno aprovado? " + aprovado);
    }
}
🚀 Resolução: Desafio (Balada.java)
O objetivo: Usar o operador de resto (%) para saber se um número é par e combinar isso com um ingresso VIP.

Como resolvemos:

Java
public class Balada {
    public static void main(String[] args) {

        // 1. Dados do cliente
        int idade = 24;
        boolean pagouVip = true;

        // 2. A mágica do número par
        // Se pegarmos a idade (24) e dividirmos por 2, sobra alguma coisa?
        // Não! O resto é 0. Então a comparação (0 == 0) dá true.
        boolean idadePar = (idade % 2) == 0;

        // 3. A regra de entrada
        // Só entra se a idade for par E se tiver pagado o VIP
        boolean podeEntrar = idadePar && pagouVip;

        // 4. Exibindo o resultado
        System.out.println("--- Controle de Entrada VIP ---");
        System.out.println("Idade do cliente: " + idade);
        System.out.println("Tem ingresso VIP? " + pagouVip);
        System.out.println("Acesso Liberado? " + podeEntrar);
    }
}

---

### 💬 Precisa de ajuda com este módulo?

Ficou confuso ou o código deu erro? Lembre-se de que a mentoria está aqui exatamente para isso! Consulte os nossos canais de contato disponíveis lá no **Canvas** e mande sua dúvida. Estou aqui para te ajudar a avançar! 💪
```
