# 🎮 Battle Quiz Arena

Projeto desenvolvido em C++ utilizando Qt Creator, Qt Widgets e conceitos de Programação Orientada a Objetos.

---

## 📌 Descrição

Battle Quiz Arena é um mini jogo de batalha em turnos com interface gráfica.
O jogador escolhe um personagem e responde perguntas para atacar o inimigo.
Cada personagem possui habilidades e atributos diferentes.
O sistema foi desenvolvido utilizando Qt Widgets e múltiplas abas (`QTabWidget`).

---

## 🎯 Objetivo

Aplicar conceitos fundamentais de Programação Orientada a Objetos utilizando uma aplicação gráfica em C++.

---

## 🧠 Conceitos de POO Utilizados

- **Encapsulamento:** Atributos de vida e ataque protegidos (`protected`) e acessados via getters.
- **Herança:** Classes filhas reutilizando a estrutura da classe base `Character`.
- **Polimorfismo:** Métodos virtuais puros para comportamentos de ataque customizados.
- **Associação entre classes:** A tela principal (`MainWindow`) gerencia e associa o jogador e o inimigo.
- **Organização modular:** Separação lógica entre interface gráfica e regras de negócio.

---

## 🧱 Estrutura do Projeto

```text
battle-quiz-arena/
│
├── CMakeLists.txt              # Configuração do build do sistema
├── main.cpp                    # Ponto de entrada do programa
├── mainwindow.h                # Header da janela principal
├── mainwindow.cpp              # Lógica da interface gráfica
├── mainwindow.ui               # Arquivo de design visual (Qt Designer)
│
├── character.h                 # Classe base dos personagens
├── character.cpp
├── warrior.h                   # Classe derivada (Guerreiro)
├── warrior.cpp
├── mage.h                      # Classe derivada (Mago)
├── mage.cpp
├── archer.h                    # Classe derivada (Arqueiro)
├── archer.cpp
│
├── docs/                       # Documentação do projeto
│   ├── analise.md
│   ├── projeto.md
│   └── testes.md
│
└── README.md
