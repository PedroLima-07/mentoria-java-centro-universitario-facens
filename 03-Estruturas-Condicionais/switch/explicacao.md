Como havíamos conversado, aqui estão os 3 arquivos completinhos e focados 100% no Switch Case, seguindo exatamente aquela estrutura de ouro (Explicação, Exercícios e Resoluções).

Se você preferir chamar todos eles de README.md (colocando cada um dentro de uma subpasta, por exemplo: explicacao/README.md, exercicios/README.md), o conteúdo abaixo vai encaixar perfeitamente!

1. README de Explicação (explicacao.md ou README.md principal)
   Markdown

# 💡 Escolhas Diretas: A Estrutura Switch Case

Você já sabe usar o `if` e `else` para tomar decisões. Ele é ótimo para checar "maior que", "menor que" ou juntar várias regras. Mas e quando você tem um **menu de opções exatas**?

Imagine um menu de telefone: _"Digite 1 para Vendas, 2 para Suporte, 3 para Financeiro"_.
Fazer isso com `if / else if` ficaria gigante e repetitivo. É para isso que existe o **Switch Case**!

O `switch` age como um seletor de canais de TV. Ele pega uma variável e testa: "É o canal 1? É o canal 2?".

---

## ✍️ A Estrutura do Switch

```java
int opcao = 2;

// O switch "liga" a verificação na variável 'opcao'
switch (opcao) {
    case 1:
        System.out.println("Você escolheu a Opção 1");
        break; // O break manda o Java PARAR e sair do switch

    case 2:
        System.out.println("Você escolheu a Opção 2");
        break;

    default: // É como o 'else', roda se nenhum dos 'cases' for verdadeiro
        System.out.println("Opção inválida!");
        break;
}
🚨 A Regra de Ouro: Nunca esqueça o break;!
A maior pegadinha do switch é o break.
Se você não colocar o break no final de um case, o Java vai sofrer do "Efeito Cascata" (Fall-through). Ele vai ignorar os próximos testes e sair executando TUDO o que estiver pela frente até achar um break ou o switch acabar.

🧵 Funciona com Textos (Strings) também!
A partir do Java 7, o switch ficou mais inteligente e passou a aceitar textos, o que facilita muito a nossa vida.

Java
String plano = "PREMIUM";

switch (plano) {
    case "BASICO":
        System.out.println("Você tem 10GB de espaço.");
        break;
    case "PREMIUM":
        System.out.println("Você tem espaço ilimitado!");
        break;
    default:
        System.out.println("Plano não reconhecido.");
        break;
}
💻 Exemplo Completo: Máquina de Café
Copie o código abaixo no seu VS Code, troque o número da variável botaoApertado e veja o que a máquina de café vai te servir!

Java
public class MaquinaDeCafe {
    public static void main(String[] args) {
        int botaoApertado = 1;

        System.out.println("Preparando sua bebida...");

        switch (botaoApertado) {
            case 1:
                System.out.println("☕ Aqui está o seu Café Expresso!");
                break;
            case 2:
                System.out.println("🥛 Aqui está o seu Café com Leite!");
                break;
            case 3:
                System.out.println("🍫 Aqui está o seu Cappuccino!");
                break;
            default:
                System.out.println("❌ Erro: Botão inexistente. Tente 1, 2 ou 3.");
                break;
        }
    }
}
Pronto para testar? Vá para a pasta de exercícios!

---

### 💬 Precisa de ajuda com este módulo?

Ficou confuso ou o código deu erro? Lembre-se de que a mentoria está aqui exatamente para isso! Consulte os nossos canais de contato disponíveis lá no **Canvas** e mande sua dúvida. Estou aqui para te ajudar a avançar! 💪
```
