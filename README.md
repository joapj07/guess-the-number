🎮 Guess the Number (C++)

Mini jogo de adivinhação de número desenvolvido em C++ utilizando conceitos de Programação Orientada a Objetos.

---

📌 Descrição

Este projeto consiste em um jogo simples onde o jogador deve adivinhar um número aleatório gerado pelo sistema.

A cada tentativa, o jogo informa se o número digitado é **maior** ou **menor** que o número secreto, até que o jogador acerte.

---

🎯 Objetivo

Aplicar na prática conceitos fundamentais de Programação Orientada a Objetos, utilizando uma aplicação simples e interativa no terminal.

---

🧠 Conceitos de POO Utilizados

* Encapsulamento
* Organização em classes
* Separação de responsabilidades
* Interação entre objetos

---

🧱 Estrutura do Projeto

```
.
├── main.cpp
├── Game.cpp
├── Game.h
├── Player.cpp
├── Player.h
```

 🔹 Descrição das Classes

* **Game**

  * Responsável pela lógica do jogo
  * Gera o número aleatório
  * Verifica os palpites do jogador

* **Player**

  * Armazena informações do jogador
  * Controla o número de tentativas

---

⚙️ Como Compilar e Executar

🔧 Compilação

Utilizando o compilador `g++`:

```
g++ main.cpp Game.cpp Player.cpp -o game
```

 ▶️ Execução

```
./game
```

---

 🎮 Como Jogar

1. O jogo gera um número aleatório (ex: entre 1 e 10)
2. O jogador digita um palpite
3. O sistema informa:

   * "Maior" → tente um número maior
   * "Menor" → tente um número menor
4. O jogo termina quando o jogador acerta

---

💡 Possíveis Melhorias

* Adicionar níveis de dificuldade
* Limitar número de tentativas
* Sistema de pontuação
* Permitir reiniciar o jogo

---

👤 Autor

João Carlos Padoveze Junior

---

📚 Contexto Acadêmico

Projeto desenvolvido para a disciplina de Programação Orientada a Objetos.

---
