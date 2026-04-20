# ✅ Gabarito: Laço For

Se você conseguiu fazer o computador repetir o código, parabéns! O `for` é uma ferramenta incrível. O segredo para não errar é sempre conferir os três elementos: de onde saio, até onde vou e qual o tamanho do meu passo.

Confira abaixo as sugestões de resolução:

---

## 🚀 Resolução: Exercício 1 (Foguete.java)

**Como resolvemos:**
Usamos a lógica da contagem regressiva, começando o `i` em 10 e usando o `i--` para diminuir de 1 em 1.

```java
public class Foguete {
    public static void main(String[] args) {

        System.out.println("Iniciando sequência de lançamento...");

        // Começa em 10; vai até 1; diminui 1 por vez
        for (int i = 10; i >= 1; i--) {
            System.out.println(i);
        }

        // Essa linha só roda depois que o for termina de repetir
        System.out.println("Fogo! 🚀");
    }
}
```

## ✖️ Resolução: Exercício 2 (Tabuada.java)

Como resolvemos:
O laço for vai gerar os números de 1 a 10 (que são os multiplicadores). O nosso número principal (7) fica fixo, e nós apenas multiplicamos um pelo outro.

```java
public class Tabuada {
    public static void main(String[] args) {

        int numero = 7; // Mude este número para ver outras tabuadas!

        System.out.println("Tabuada do " + numero + ":");

        for (int i = 1; i <= 10; i++) {
            // Calculamos o resultado antes de imprimir para ficar mais organizado
            int resultado = numero * i;
            System.out.println(numero + " x " + i + " = " + resultado);
        }
    }
}
```

## 🐷 Resolução: Desafio (Cofrinho.java)

Como resolvemos:
Aqui entra o conceito de Variável Acumuladora. A variável totalGuardado precisa ser criada fora do for. Se você criar ela dentro do for, o Java vai zerar o cofrinho a cada repetição!

```java
public class Cofrinho {
    public static void main(String[] args) {

        // O cofre nasce vazio e FORA da repetição
        double totalGuardado = 0;

        System.out.println("Iniciando os depósitos...");

        for (int dia = 1; dia <= 5; dia++) {
            // Vamos simular que a cada dia depositamos R$ 15.00
            double depositoDoDia = 15.00;

            // O += soma o depósito ao que já existia no cofre
            totalGuardado += depositoDoDia;

            System.out.println("Dia " + dia + ": Depositou R$ " + depositoDoDia);
        }

        // O saldo final é impresso fora do for!
        System.out.println("--- Fim da semana ---");
        System.out.println("Total no cofrinho: R$ " + totalGuardado);
    }
}
```

---

### 💬 Precisa de ajuda com este módulo?

Ficou confuso ou o código deu erro? Lembre-se de que a mentoria está aqui exatamente para isso! Consulte os nossos canais de contato disponíveis lá no **Canvas** e mande sua dúvida. Estou aqui para te ajudar a avançar! 💪
