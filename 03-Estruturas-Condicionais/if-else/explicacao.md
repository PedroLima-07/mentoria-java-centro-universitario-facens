# 🔀 Tomando Decisões: If, Else If e Else

Bem-vindo ao coração da lógica de programação! Até agora, nossos programas faziam sempre a mesma coisa. Mas, no mundo real, as ações dependem de **condições**.

- "Se chover, levo guarda-chuva. Senão, levo óculos de sol."

Em Java, nós ensinamos o computador a tomar essas decisões usando as palavras-chave `if` (se) e `else` (senão).

---

## 🚦 1. O básico: O `if` (Se)

O `if` é como um porteiro. Ele verifica uma condição (que deve ser verdadeira ou falsa). Se for verdadeira (`true`), ele abre a porta e executa o código que está dentro das chaves `{ }`.

```java
int idade = 20;

// O porteiro faz a pergunta: "A idade é maior ou igual a 18?"
if (idade >= 18) {
    // Como 20 é maior que 18, a porta se abre e este código roda!
    System.out.println("Acesso liberado. Pode entrar!");
}
```

### 🛑 2. A alternativa: O else (Senão)

Mas e se a pessoa tiver 15 anos? O if vai dar falso, e o programa simplesmente não vai fazer nada. Para dar uma resposta quando a condição falha, usamos o else.

O else nunca tem uma condição do lado dele, porque ele significa "em qualquer outro caso que não seja o de cima".

```java
int idade = 15;

if (idade >= 18) {
    System.out.println("Acesso liberado. Pode entrar!");
} else {
    // Como 15 NÃO é maior/igual a 18, o if é ignorado e o else assume.
    System.out.println("Acesso negado. Volte para casa.");
}
```

### 🛤️ 3. Múltiplos Caminhos: O else if (Senão Se)

Às vezes, a vida não é só "preto no branco". Temos várias opções. Imagine classificar a idade de alguém em Criança, Adolescente ou Adulto.

Para adicionar novos testes lógicos, usamos o else if:

```java
int idade = 14;

if (idade < 12) {
    System.out.println("Você é uma Criança.");
} else if (idade < 18) {
    // O Java só chega aqui se a primeira condição for falsa.
    // Então sabemos que a idade é 12 ou mais, E menor que 18.
    System.out.println("Você é um Adolescente.");
} else {
    // Se não for criança nem adolescente, só pode ser adulto!
    System.out.println("Você é um Adulto.");
}
```

💡 Dica do Mentor: Cuidado com as Chaves { }
Tudo o que você quer que aconteça dentro de um if ou else DEVE estar "abraçado" pelas chaves. Se você esquecer delas, o Java pode executar comandos na hora errada e causar bugs bizarros!

### 💻 Exemplo Completo

Copie e cole este código no seu VS Code, mude o valor da variável saldo e veja como o programa toma caminhos diferentes:

```java
public class CaixaEletronico {
    public static void main(String[] args) {
        double saldo = 100.0;
        double valorSaque = 150.0;

        System.out.println("Tentando sacar R$ " + valorSaque);

        if (valorSaque <= saldo) {
            saldo = saldo - valorSaque; // Atualiza o saldo
            System.out.println("Saque realizado com sucesso!");
            System.out.println("Novo saldo: R$ " + saldo);
        } else {
            System.out.println("Operação negada: Saldo insuficiente.");
        }
    }
}
```

Pronto para testar sua lógica? Vá para o arquivo exercicios.md!

---

### 💬 Precisa de ajuda com este módulo?

Ficou confuso ou o código deu erro? Lembre-se de que a mentoria está aqui exatamente para isso! Consulte os nossos canais de contato disponíveis lá no **Canvas** e mande sua dúvida. Estou aqui para te ajudar a avançar! 💪
