# 💣 Campo Minado Swing

Uma versão gráfica do clássico **Campo Minado**, desenvolvida em **Java**, utilizando **Swing** para a interface visual.

Projeto criado como prática de **Programação Orientada a Objetos (POO)** e manipulação de **eventos gráficos**, com base no curso de **Java da Cod3r**.

## 🎯 Objetivos do Projeto

- Praticar os fundamentos de **POO** (encapsulamento, herança, polimorfismo e abstração)  
- Aplicar **eventos e observadores** entre modelo e interface  
- Aprender a criar **interfaces gráficas (GUI)** com **Java Swing**  
- Implementar a lógica completa do jogo **Campo Minado**, com **vitória**, **derrota** e **reinício automático**

## 📂 Estrutura do Projeto

A arquitetura segue o padrão **MVC (Model-View-Controller)** simplificado, separando **modelo** (regras do jogo) e **visão** (interface Swing):
```swift
campo-minado-swing/
├── src/br/com/campominado/
│ ├── modelo/
│ │ ├── Campo.java
│ │ ├── CampoEvento.java
│ │ ├── CampoObservador.java
│ │ ├── ResultadoEvento.java
│ │ └── Tabuleiro.java
│ │
│ └── visao/
│ ├── BotaoCampo.java
│ ├── PainelTabuleiro.java
│ └── TelaPrincipal.java
│
├── .gitignore
├── README.md

```

## 🧩 Descrição dos pacotes

- **modelo/** → Contém toda a lógica do jogo (regras, eventos e tabuleiro)  
- **visao/** → Implementa a interface Swing, compondo os painéis e botões do jogo  

## 🖥️ Como executar o projeto

### 1. Clonar o repositório
```bash
git clone https://github.com/pitercoding/campo-minado-swing.git
cd campo-minado-swing
```

### 2. Abrir no IntelliJ IDEA
- Vá em **File > Open...**
- Selecione a pasta do projeto
- Certifique-se de que o SDK do projeto está configurado para **Java 17** (ou superior)

### 3. Executar o jogo
- Abra a classe `TelaPrincipal.java`
- Clique em **Run ▶️**

O jogo será aberto em uma janela Swing com o título **"Campo Minado"**.

## 🎮 Funcionalidades do Jogo

### 🧱 Grade de botões interativos
- Clique esquerdo → abre o campo  
- Clique direito → marca/desmarca bandeira  

### 💥 Explosão de mina
- Ao abrir um campo minado, o botão muda de cor e mostra **“X”**

### 🚩 Marcação de bandeira
- Botões marcados ficam **azuis** e mostram **“M”**

### 🏆 Vitória / Derrota
- Mostra uma mensagem (`JOptionPane`) ao ganhar ou perder  
- O tabuleiro é **reiniciado automaticamente** após cada partida

### 🔁 Sistema de eventos reativos
- A interface é atualizada automaticamente sempre que o modelo muda (via `CampoObservador`)

## 📸 Capturas de Tela

### 💣 Derrota:

![perdeu](https://github.com/user-attachments/assets/664ba702-d77d-46f8-842d-80aff4cd2d6a)

### 🏆 Vitória:
![ganhou](https://github.com/user-attachments/assets/3317db7c-bc81-4cc4-be24-b365e14bf89c)

## 🧠 Tecnologias Utilizadas

- ☕ **Java 21**
- 🖥️ **Swing / AWT**
- 🧩 **Padrão Observer**
- 🧱 **Layouts de interface (GridLayout, BorderLayout)**
- 🧪 **Programação orientada a eventos**

## 📜 Licença

Este projeto é licenciado sob a **MIT License** — você é livre para usar, estudar e modificar.

## ✨ Créditos

Projeto desenvolvido como exercício prático baseado no **Curso de Java da Cod3r**.

