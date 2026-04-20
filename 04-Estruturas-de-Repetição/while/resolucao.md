# ✅ Gabarito: Laço While

Seu computador sobreviveu ou você travou ele com um loop infinito? 😂 Brincadeiras à parte, é super comum esquecer o decremento/incremento nas primeiras vezes. O importante é entender a lógica!

Confira abaixo como resolvemos os exercícios:

---

## ⏱️ Resolução: Exercício 1 (BombaRelogio.java)

**Como resolvemos:**
Usamos a variável de tempo como nossa condição de parada. Se não colocarmos `tempo--`, a bomba nunca vai explodir (ou melhor, o cronômetro nunca vai descer).

```java
public class BombaRelogio {
    public static void main(String[] args) {
        int tempo = 10;

        System.out.println("Iniciando cronômetro da bomba!");

        while (tempo >= 0) {
            System.out.println("Tempo restante: " + tempo + " segundos.");

            // ESSENCIAL: diminuir o tempo para não virar loop infinito!
            tempo--;
        }

        System.out.println("Bomba desarmada com sucesso! ✂️🔴");
    }
}
```

## 💰 Resolução: Exercício 2 (Poupanca.java)

Como resolvemos:
Aqui o while brilha! Nós não sabíamos quantos meses iam demorar, deixamos o Java calcular isso pra gente aumentando a variável meses a cada vez que o dinheiro caía na conta.

```java
public class Poupanca {
    public static void main(String[] args) {
        double saldo = 0;
        double meta = 3000.0;
        int meses = 0;

        System.out.println("Iniciando o projeto Videogame Novo!");

        // Enquanto não atingir a meta, continue guardando
        while (saldo < meta) {
            saldo += 450.0; // Guarda o dinheiro do mês
            meses++;        // Conta que se passou um mês
            System.out.println("Mês " + meses + ": Saldo atual R$ " + saldo);
        }

        System.out.println("--- Parabéns! ---");
        System.out.println("Você atingiu a meta em " + meses + " meses.");
        System.out.println("Saldo final: R$ " + saldo);
    }
}
```

## 🐉 Resolução: Desafio (BatalhaRPG.java)

Como resolvemos:
O combate roda até o Dragão morrer (HP chegar a 0 ou menos).

```java
public class BatalhaRPG {
    public static void main(String[] args) {
        int hpDragao = 500;
        int danoDoHeroi = 45;
        int ataquesRealizados = 0;

        System.out.println("Um dragão selvagem apareceu! HP: " + hpDragao);

        // Enquanto o dragão tiver vida...
        while (hpDragao > 0) {
            System.out.println("Herói ataca e causa " + danoDoHeroi + " de dano!");
            hpDragao -= danoDoHeroi; // Tira a vida do dragão
            ataquesRealizados++;     // Conta o ataque

            // Verifica se o HP ficou negativo, só para não imprimir "HP: -40" na tela
            if (hpDragao < 0) {
                hpDragao = 0;
            }

            System.out.println("HP restante do Dragão: " + hpDragao);
            System.out.println("-------------------------");
        }

        System.out.println("Vitória épica!");
        System.out.println("O dragão foi derrotado em " + ataquesRealizados + " ataques.");
    }
}
```

---

### 💬 Precisa de ajuda com este módulo?

Ficou confuso ou o código deu erro? Lembre-se de que a mentoria está aqui exatamente para isso! Consulte os nossos canais de contato disponíveis lá no **Canvas** e mande sua dúvida. Estou aqui para te ajudar a avançar! 💪
