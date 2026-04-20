# 🛠️ Preparando o Ambiente Java (Windows)

Bem-vindo(a)! 👋  
Antes de começar a programar, vamos preparar o seu computador.

Pense assim:

- ☕ **JDK** → é o “motor” que faz o Java funcionar
- 🧑‍💻 **VS Code** → é onde você vai escrever seus códigos

Fica tranquilo(a), vamos fazer tudo juntos, passo a passo.

---

## ✅ Passo 1: Instalando o Java (JDK)

O JDK é essencial. Sem ele, o Java não roda.

### 🔽 Download

1. Acesse: https://adoptium.net/
2. Clique em **"Latest LTS Release"**
3. Baixe o arquivo `.msi`

---

### ⚙️ Instalação

1. Dê **duplo clique** no arquivo baixado
2. Clique em **Next** até chegar em **Custom Setup**

👉 **Passo importante:**

- Procure por: `Set JAVA_HOME variable`
- Clique no X vermelho
- Selecione: **"Will be installed on local hard drive"**

✔ Isso garante que o Windows reconheça o Java corretamente.

3. Continue:
   - Next → Install → Finish

---

### 🧪 Testar se funcionou (IMPORTANTE)

1. Aperte `Win + R`
2. Digite: `cmd`
3. No terminal, digite:

bash
java -version

✔ Se aparecer algo como:

java version "17..."

Tudo certo! 🎉

---

# 🧑‍💻 Instalando o VS Code (Seu Editor de Código)

Agora que o Java já está instalado, precisamos de um lugar para escrever nossos códigos.

É aqui que entra o **VS Code (Visual Studio Code)** — leve, gratuito e perfeito para iniciantes.

Pense nele como o seu “caderno inteligente” de programação. 📓✨

---

## ✅ Passo 1: Baixar o VS Code

1. Acesse o site oficial:
   👉 https://code.visualstudio.com/

2. Clique no botão azul:
   **Download for Windows**

---

## ✅ Passo 2: Instalar o VS Code

1. Abra o arquivo que você baixou
2. Aceite os termos de uso
3. Vá clicando em **Próximo**

---

### ⚙️ Atenção nessa parte (IMPORTANTE)

Durante a instalação, você verá a tela de **tarefas adicionais**.

Marque estas opções:

- ✔ Adicionar "Abrir com Code" ao menu de contexto
- ✔ Adicionar ao PATH (se aparecer)

💡 Isso facilita MUITO sua vida depois.

---

## ✅ Passo 3: Finalizar instalação

1. Clique em **Instalar**
2. Depois em **Concluir**

✔ O VS Code vai abrir automaticamente.

---

## 🧪 Testando se deu certo

Se o VS Code abriu com uma tela parecida com um editor (escura ou clara), já está funcionando.

Você deve ver:

- Uma tela inicial
- Um menu lateral (com ícones)
- Um espaço grande para código

✔ Pronto! Seu editor está funcionando.

---

## 🧩 Próximo passo (IMPORTANTE)

O VS Code ainda não entende Java sozinho.

No próximo guia, vamos instalar o suporte ao Java (extensões).

---

## 🤝 Em caso de dúvidas

Travou em algum ponto? Relaxa, isso é normal.

Você pode:

- 💡 Pedir ajuda para uma IA (como o ChatGPT)
- 📩 Falar com o seu mentor

O importante é continuar. 🚀

---

# 🧩 Instalando o Suporte ao Java no VS Code

Agora que você já tem o VS Code instalado, falta um detalhe importante:

👉 Ele ainda **não entende Java sozinho**.

Vamos resolver isso instalando um pacote de extensões que transforma o VS Code em um ambiente completo para programar em Java.

---

## ✅ O que vamos instalar?

Um pacote chamado:

Extension Pack for Java

💡 Ele já vem com tudo que você precisa:

- Compilador
- Debug (depuração)
- Autocomplete (auto completar código)
- Execução de programas

---

## ✅ Passo 1: Abrir a aba de extensões

1. Abra o VS Code
2. No lado esquerdo, clique no ícone de **Extensões** (🧩 ou 4 quadradinhos)

---

## ✅ Passo 2: Buscar a extensão

1. Na barra de pesquisa, digite:

Extension Pack for Java

---

## ✅ Passo 3: Instalar

1. Clique na extensão criada pela **Microsoft**
2. Clique no botão **Install (Instalar)**

⏳ Aguarde alguns instantes...

---

## ✅ Passo 4: Verificar se deu certo

Depois da instalação:

- O botão **Install** deve sumir
- Vai aparecer um ícone de engrenagem ⚙️

✔ Isso significa que está instalado corretamente

---

## 🔄 Reiniciar (se necessário)

Se o VS Code pedir para reiniciar:

👉 Clique em **Reload** ou feche e abra novamente

---

## 🧪 Teste rápido

Agora, quando você criar um arquivo `.java`, o VS Code já deve:

- Colorir o código 🎨
- Sugerir automaticamente comandos 🤖
- Mostrar botão de executar ▶️

✔ Se isso aconteceu, deu tudo certo!

---

## 🚀 Próximo passo

Agora você já pode:

👉 Criar e executar seu primeiro código Java (Hello World)

---

## 🤝 Em caso de dúvidas

Se algo não funcionar como esperado:

- 💡 Use uma IA (como o ChatGPT) para te ajudar
- 📩 Fale com o seu mentor

Errar faz parte — o importante é continuar. 🚀
