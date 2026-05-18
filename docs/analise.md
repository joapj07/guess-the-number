# 📊 Análise do Sistema - Battle Quiz Arena

## 📌 Objetivo

Desenvolver um mini jogo de batalha em turnos utilizando C++, Qt Creator e conceitos de Programação Orientada a Objetos. O jogador deverá responder perguntas corretamente para desferir ataques contra o inimigo.

---

## ✅ Requisitos Funcionais (O que o jogo faz)

- **RF01:** Permitir que o jogador escolha uma classe de personagem (Warrior, Mage ou Archer).
- **RF02:** Exibir perguntas de múltipla escolha de forma aleatória ou sequencial.
- **RF03:** Validar se a resposta selecionada pelo jogador está correta ou incorreta.
- **RF04:** Executar ataques baseados na resposta (se acertar, o jogador ataca; se errar, o inimigo contra-ataca).
- **RF05:** Controlar a vida (HP) atual e máxima dos personagens em tempo real.
- **RF06:** Encerrar a partida assim que o HP do jogador ou do inimigo atingir zero, declarando o vencedor.
- **RF07:** Gravar e exibir a pontuação do jogador em um sistema de ranking.

---

## 🎨 Requisitos de Interface (UI)

- **RI01:** Interface gráfica totalmente desenvolvida utilizando a biblioteca Qt Widgets.
- **RI02:** Organização das telas do jogo através de abas (`QTabWidget`) para separar a Seleção de Personagem, a Arena de Batalha e o Ranking.

---

## ⚙️ Requisitos Não Funcionais (Como o sistema é feito)

- **RNF01:** Desenvolvido na linguagem de programação C++ (padrão moderno C++17 ou superior).
- **RNF02:** Utilização da IDE Qt Creator com o sistema de build **CMake**.
- **RNF03:** Compilação através do **MinGW (64-bit)**.
- **RNF04:** Organização modular do código (separação clara entre arquivos `.h` e `.cpp`).
- **RNF05:** Aplicação obrigatória dos pilares de POO: **Encapsulamento** (atributos protegidos/getters), **Herança** (classes derivadas de Character) e **Polimorfismo** (método de ataque reescrito por classe).
