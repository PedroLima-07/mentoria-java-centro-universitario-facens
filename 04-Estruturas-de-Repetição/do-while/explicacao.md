Para fechar o módulo de laços de repetição com chave de ouro, vamos para o Do-While.

A grande sacada de ensinar o do-while é mostrar que ele é a estrutura oficial dos Menus Interativos. E para isso ficar legal de verdade, introduzi um "bônus" na explicação: o Scanner (para o aluno finalmente poder digitar no teclado e interagir com o código!).

Aqui estão os 3 arquivos completinhos para a pasta 04-estruturas-de-repeticao/do-while/:

1. Arquivo: explicacao.md (ou README.md principal)
   Markdown

# 🔄 Estrutura Do-While: Faça primeiro, pergunte depois!

Nós vimos que o `while` é como um porteiro rigoroso: ele testa a condição **antes** de deixar o código rodar. Se a condição for falsa logo de cara, o código nunca será executado.

Mas e se você precisar que o código rode **pelo menos uma vez** antes de fazer o teste?
É para isso que usamos o **`do-while`** (Faça-Enquanto). Ele é o cara do "atira primeiro, faz perguntas depois".

---

## ✍️ A Anatomia do Do-While

A estrutura inverte a ordem das coisas. Primeiro vem o bloco de código (o `do`), e a verificação (o `while`) fica lá no finalzinho.

```java
int contador = 1;

do {
    // 1º: Ele FAZ isso obrigatoriamente pelo menos uma vez.
    System.out.println("Contagem: " + contador);
    contador++;

} while (contador <= 5); // 2º: Só agora ele PERGUNTA se deve voltar pro começo.
// ⚠️ Atenção: O do-while é a única estrutura que termina com PONTO E VÍRGULA (;) depois da condição!
🎁 Bônus: Interagindo com o usuário (Scanner)
O lugar onde o do-while mais brilha é na criação de Menus. E para um menu fazer sentido, o usuário precisa digitar a opção no teclado.

Para ler o teclado no Java, usamos uma ferramenta chamada Scanner. Veja como é fácil:

Java
import java.util.Scanner; // 1. Importamos a ferramenta lá no topo do arquivo

public class ExemploScanner {
    public static void main(String[] args) {
        // 2. "Ligamos" o Scanner no teclado do computador (System.in)
        Scanner leitor = new Scanner(System.in);

        System.out.println("Digite o seu nome:");
        String nome = leitor.nextLine(); // 3. O programa PAUSA e espera você digitar um texto

        System.out.println("Digite sua idade:");
        int idade = leitor.nextInt(); // 3. O programa PAUSA e espera você digitar um número inteiro

        System.out.println("Olá " + nome + ", você tem " + idade + " anos!");
    }
}
💻 Exemplo Prático: O Menu Interativo
Juntando o do-while com o Scanner, nós podemos criar um programa que fica rodando até o usuário decidir sair! Copie esse código no VS Code e brinque no terminal:

Java
import java.util.Scanner;

public class Menu {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);
        int opcao; // Criamos a variável fora do laço para o while conseguir enxergar ela depois

        do {
            System.out.println("--- MENU ---");
            System.out.println("1. Ver Saldo");
            System.out.println("2. Fazer Depósito");
            System.out.println("3. Sair");
            System.out.println("Escolha uma opção: ");

            opcao = leitor.nextInt(); // Lê o que o usuário digitou

            if (opcao == 1) {
                System.out.println("Seu saldo é R$ 100,00.\n");
            } else if (opcao == 2) {
                System.out.println("Depósito realizado!\n");
            } else if (opcao != 3) {
                System.out.println("Opção inválida! Tente de novo.\n");
            }

        } while (opcao != 3); // O menu repete ENQUANTO a opção for diferente de 3

        System.out.println("Encerrando o sistema. Até logo!");
    }
}
Pronto para criar seus próprios sistemas interativos? Vá para o arquivo exercicios.md!

---

### 💬 Precisa de ajuda com este módulo?

Ficou confuso ou o código deu erro? Lembre-se de que a mentoria está aqui exatamente para isso! Consulte os nossos canais de contato disponíveis lá no **Canvas** e mande sua dúvida. Estou aqui para te ajudar a avançar! 💪
```
