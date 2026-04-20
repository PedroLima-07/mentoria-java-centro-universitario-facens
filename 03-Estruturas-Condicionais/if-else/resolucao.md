# ✅ Gabarito: If, Else If e Else

Se você concluiu os exercícios, parabéns! Lidar com várias condições pode dar um nó na cabeça no começo. Confira abaixo as sugestões de resolução.

Lembre-se: se a sua lógica funcionou e respondeu corretamente às condições, seu código está certo, mesmo que esteja escrito de forma ligeiramente diferente do meu!

---

## 🗳️ Resolução: Exercício 1 (Votacao.java)

**Como resolvemos:**
Usamos a ordem lógica da idade, do menor para o maior, para o `else if` filtrar corretamente.

```java
public class Votacao {
    public static void main(String[] args) {
        int idade = 65; // Pode testar com 15, 17, 25, 75...

        if (idade < 16) {
            System.out.println("Você não pode votar.");
        }
        // O || significa "OU". Se a idade for menor que 18 OU maior que 70.
        else if (idade < 18 || idade > 70) {
            System.out.println("Seu voto é opcional (facultativo).");
        }
        else {
            // Se chegou aqui, é porque tem 18 ou mais, e 70 ou menos.
            System.out.println("Seu voto é OBRIGATÓRIO.");
        }
    }
}
```

## 🌡️ Resolução: Exercício 2 (Clima.java)

Como resolvemos:
Avaliamos os intervalos de temperatura.

```java
public class Clima {
    public static void main(String[] args) {
        double temperatura = 22.5;

        if (temperatura < 15) {
            System.out.println("Está frio! Leve um casaco.");
        }
        // Se o Java chegou aqui, sabemos que a temperatura é 15 ou mais.
        // Então só precisamos testar se é até 25.
        else if (temperatura <= 25) {
            System.out.println("Clima agradável! Uma camiseta está ótimo.");
        }
        else {
            System.out.println("Está calor! Não esqueça a água e o protetor solar.");
        }
    }
}
```

## 🚀 Resolução: Desafio (Emprestimo.java)

Como resolvemos:
Para o empréstimo ser aprovado, o nome do cliente não pode estar sujo. Ou seja, nomeSujo precisa ser false. Usamos o operador de "NÃO" lógico (!) ou comparamos com false.

```java
public class Emprestimo {
    public static void main(String[] args) {
        double salario = 3000.00;
        boolean nomeSujo = false;

        // Verifica: Salário é maior que 2500 E (&&) nomeSujo é igual a falso?
        if (salario > 2500 && nomeSujo == false) {
            System.out.println("Parabéns! Empréstimo Aprovado!");
        }
        else if (nomeSujo == true) {
            // Podemos dar um feedback específico se o problema for o nome sujo
            System.out.println("Empréstimo Negado: Cliente possui restrições no Serasa.");
        }
        else {
            // Se o nome não está sujo, o problema só pode ser a renda baixa
            System.out.println("Empréstimo Negado: Renda mínima não atingida.");
        }
    }
}
```

---

### 💬 Precisa de ajuda com este módulo?

Ficou confuso ou o código deu erro? Lembre-se de que a mentoria está aqui exatamente para isso! Consulte os nossos canais de contato disponíveis lá no **Canvas** e mande sua dúvida. Estou aqui para te ajudar a avançar! 💪
