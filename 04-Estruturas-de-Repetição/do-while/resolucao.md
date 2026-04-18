# ✅ Gabarito: Do-While e Scanner

Se você chegou até aqui, você subiu de nível! Manipular dados vindos do usuário (via teclado) é o que separa códigos teóricos de softwares reais.

Confira abaixo as sugestões de resolução:

---

## 🔐 Resolução: Exercício 1 (Senha.java)

**Como resolvemos:**
O `do-while` garante que a pergunta "Digite a senha" vai aparecer pelo menos a primeira vez antes de checar se está certa.

```java
import java.util.Scanner;

public class Senha {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        int senhaCerta = 1234;
        int senhaDigitada;

        do {
            System.out.println("🔒 Digite a senha de 4 dígitos: ");
            senhaDigitada = leitor.nextInt(); // Lê a digitação do usuário

            if (senhaDigitada != senhaCerta) {
                System.out.println("❌ Senha incorreta! Tente novamente.\n");
            }

        } while (senhaDigitada != senhaCerta); // Repete se for diferente da certa

        System.out.println("✅ Acesso Permitido!");
    }
}
🎲 Resolução: Exercício 2 (Adivinhacao.java)
Como resolvemos:
Usamos lógicas de if e else if dentro do laço para ir guiando o usuário até ele acertar.

Java
import java.util.Scanner;

public class Adivinhacao {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        int numeroSecreto = 7;
        int palpite;

        System.out.println("Bem-vindo ao Jogo de Adivinhação!");
        System.out.println("Pensei em um número de 1 a 10. Tente adivinhar!");

        do {
            System.out.print("Qual é o seu palpite? ");
            palpite = leitor.nextInt();

            if (palpite < numeroSecreto) {
                System.out.println("Errado! Tente um número MAIOR. ⬆️");
            } else if (palpite > numeroSecreto) {
                System.out.println("Errado! Tente um número MENOR. ⬇️");
            }

        } while (palpite != numeroSecreto);

        System.out.println("🎉 Parabéns! Você acertou na mosca!");
    }
}
🍕 Resolução: Desafio (Lanchonete.java)
Como resolvemos:
Combinamos o do-while com o switch case (poderia ser um if/else também) para montar um sistema de caixa registradora clássico.

Java
import java.util.Scanner;

public class Lanchonete {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        int escolha;
        double totalConta = 0.0;

        System.out.println("Bem-vindo à Lanchonete Dev!");

        do {
            System.out.println("\n--- Cardápio ---");
            System.out.println("1. Hamburguer - R$ 20.00");
            System.out.println("2. Refrigerante - R$ 5.00");
            System.out.println("0. Finalizar Pedido");
            System.out.print("O que deseja adicionar ao pedido? ");

            escolha = leitor.nextInt();

            switch (escolha) {
                case 1:
                    totalConta += 20.00; // Soma 20 na conta
                    System.out.println("🍔 Hamburguer adicionado!");
                    break;
                case 2:
                    totalConta += 5.00; // Soma 5 na conta
                    System.out.println("🥤 Refrigerante adicionado!");
                    break;
                case 0:
                    System.out.println("Preparando sua conta...");
                    break;
                default:
                    System.out.println("Opção inválida!");
                    break;
            }

        } while (escolha != 0); // Continua até o cliente digitar 0

        System.out.println("\n=========================");
        System.out.println("Total a pagar: R$ " + totalConta);
        System.out.println("Bom apetite!");
    }
}

---

### 💬 Precisa de ajuda com este módulo?

Ficou confuso ou o código deu erro? Lembre-se de que a mentoria está aqui exatamente para isso! Consulte os nossos canais de contato disponíveis lá no **Canvas** e mande sua dúvida. Estou aqui para te ajudar a avançar! 💪
```
