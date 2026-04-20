# ✅ Gabarito: Switch Case

Se você chegou até aqui, muito bem! O `switch` é super divertido de usar quando entendemos a lógica de "selecionar uma gaveta". A maior dificuldade no começo é só lembrar de colocar o `break`.

Confira abaixo as sugestões de resolução:

---

## 📅 Resolução: Exercício 1 (DiaDaSemana.java)

**Como resolvemos:**
Usamos os números de 1 a 7 como os `cases`. O `default` garante que o programa não quebre se alguém digitar 8 ou 0.

```java
public class DiaDaSemana {
    public static void main(String[] args) {
        int dia = 3;

        switch (dia) {
            case 1:
                System.out.println("Domingo");
                break;
            case 2:
                System.out.println("Segunda-feira");
                break;
            case 3:
                System.out.println("Terça-feira");
                break;
            case 4:
                System.out.println("Quarta-feira");
                break;
            case 5:
                System.out.println("Quinta-feira");
                break;
            case 6:
                System.out.println("Sexta-feira");
                break;
            case 7:
                System.out.println("Sábado");
                break;
            default:
                System.out.println("Erro: Dia inválido! Digite um número de 1 a 7.");
                break;
        }
    }
}
```

## 🎧 Resolução: Exercício 2 (Atendimento.java)

Como resolvemos:
Bem parecido com o primeiro, simulando a navegação de um menu de telefone real.

```java
public class Atendimento {
    public static void main(String[] args) {
        int opcaoEscolhida = 2;

        System.out.println("Bem-vindo ao Atendimento da NetLink!");

        switch (opcaoEscolhida) {
            case 1:
                System.out.println("Encaminhando para o Suporte Técnico. Tempo de espera: 2 minutos.");
                break;
            case 2:
                System.out.println("Sua 2ª via do boleto foi enviada para o seu e-mail cadastrado.");
                break;
            case 3:
                System.out.println("Redirecionando para o setor de Vendas e Planos...");
                break;
            case 4:
                System.out.println("Poxa, que pena que deseja cancelar. Transferindo para o setor de Retenção.");
                break;
            default:
                System.out.println("Opção inválida. Por favor, desligue e ligue novamente.");
                break;
        }
    }
}
```

## 🚀 Resolução: Desafio (Calculadora.java)

Como resolvemos:
Aqui está o poder do switch trabalhando com Strings! Note que o texto fica sempre entre aspas duplas " ".

```java
public class Calculadora {
    public static void main(String[] args) {
        double num1 = 20.0;
        double num2 = 4.0;

        // Troque o sinal aqui para testar as outras operações (+, -, *, /)
        String operacao = "/";

        System.out.println("Calculando: " + num1 + " " + operacao + " " + num2);

        switch (operacao) {
            case "+":
                System.out.println("Resultado: " + (num1 + num2));
                break;
            case "-":
                System.out.println("Resultado: " + (num1 - num2));
                break;
            case "*":
                System.out.println("Resultado: " + (num1 * num2));
                break;
            case "/":
                System.out.println("Resultado: " + (num1 / num2));
                break;
            default:
                System.out.println("Operação inválida. Use apenas +, -, * ou /.");
                break;
        }
    }
}
```

---

### 💬 Precisa de ajuda com este módulo?

Ficou confuso ou o código deu erro? Lembre-se de que a mentoria está aqui exatamente para isso! Consulte os nossos canais de contato disponíveis lá no **Canvas** e mande sua dúvida. Estou aqui para te ajudar a avançar! 💪
