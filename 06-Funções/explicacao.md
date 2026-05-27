# 🧠 Módulo 04: Funções em Java

Até agora, todo o nosso código ficou dentro do `main`. Isso funciona em programas pequenos… mas imagine criar um sistema enorme com centenas de linhas misturadas. Viraria um caos 😵‍💫

É aí que entram as **Funções** (também chamadas de métodos no Java).

Uma função é como uma **máquina especializada**:
- você dá uma tarefa para ela,
- ela executa,
- e pode até devolver um resultado.

Isso ajuda a:
- organizar o código 📂
- evitar repetição 🔁
- deixar o programa mais fácil de entender 👀

---

# ✍️ Como criar uma função em Java?

A estrutura básica é esta:

```java
public static void nomeDaFuncao() {

    // código aqui dentro

}
```

Exemplo:

```java
public static void mostrarMensagem() {
    System.out.println("Olá, seja bem-vindo!");
}
```

Mas criar a função não faz ela executar automaticamente.

Para usar, precisamos **chamar** a função:

```java
public class Main {

    public static void mostrarMensagem() {
        System.out.println("Olá, seja bem-vindo!");
    }

    public static void main(String[] args) {

        mostrarMensagem();

    }
}
```

---

# 📥 Funções com parâmetros

Às vezes queremos que a função receba informações.

Essas informações são chamadas de **parâmetros**.

Exemplo:

```java
public static void cumprimentar(String nome) {
    System.out.println("Olá, " + nome + "!");
}
```

Chamando a função:

```java
cumprimentar("Pedro");
cumprimentar("Ana");
```

Saída:

```java
Olá, Pedro!
Olá, Ana!
```

O valor enviado para a função é chamado de argumento.

---

# 📤 Funções com retorno

Algumas funções apenas executam ações.
Outras devolvem um resultado.

Para isso usamos o `return`.

Exemplo:

```java
public static int somar(int a, int b) {

    int resultado = a + b;

    return resultado;
}
```

Usando a função:

```java
int total = somar(5, 3);

System.out.println(total);
```

Saída:

```java
8
```

---

# 🚨 Entendendo o `void`

Quando usamos:

```java
public static void
```

O `void` significa:

👉 “essa função não devolve nenhum valor”.

Ela apenas executa algo.

Exemplo:

```java
public static void mostrarLinha() {
    System.out.println("----------------");
}
```

---

# 🔄 Reaproveitando código

O maior poder das funções é evitar repetição.

Sem função:

```java
System.out.println("Olá!");
System.out.println("Olá!");
System.out.println("Olá!");
```

Com função:

```java
public static void saudacao() {
    System.out.println("Olá!");
}
```

Chamando:

```java
saudacao();
saudacao();
saudacao();
```

Muito mais organizado 😎

---

# 🧩 Exemplo completo

```java
public class Main {

    public static void mostrarTitulo() {
        System.out.println("=== Sistema Escolar ===");
    }

    public static int somarNotas(int n1, int n2) {
        return n1 + n2;
    }

    public static void main(String[] args) {

        mostrarTitulo();

        int resultado = somarNotas(7, 8);

        System.out.println("Total das notas: " + resultado);
    }
}
```

Agora que você aprendeu como criar e usar funções, vá para o arquivo `exercicios.md` e pratique 🚀