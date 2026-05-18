# 🎮 Battle Quiz Arena

Projeto desenvolvido em C++ utilizando Qt Creator, Qt Widgets e conceitos avançados de Programação Orientada a Objetos.

---

## 📌 Descrição

Battle Quiz Arena é um jogo de batalha em turnos com interface gráfica. O jogador escolhe uma classe de personagem (Guerreiro, Mago ou Arqueiro) e enfrenta o temível Chefão da Arena ("O Grão-Mestre do Silício").

Para desferir ataques e vencer a batalha, o jogador deve responder corretamente a perguntas de múltipla escolha sobre POO e Eletrônica. O jogo conta com um **Sistema de Inventário (Itens Consumíveis)** para cura ou bônus de dano e um **Sistema de Ranking Persistente**, que grava o histórico de pontuações diretamente no disco do computador.

---

## 🧠 Conceitos de POO Utilizados

- **Encapsulamento:** Atributos de vida, ataque e inventário protegidos (`protected`/`private`) e acessados via getters/setters públicos.
- **Herança:** Classes de personagens derivadas de `Character` e classes de itens derivadas de uma classe base `Item`.
- **Polimorfismo:** Métodos virtuais puros para comportamentos de ataque dos heróis e para o efeito de uso de cada tipo de item.
- **Associação e Agregação:** A `MainWindow` gerencia o jogo (Associação), e cada personagem possui uma lista de objetos do tipo `Item` (Agregação).
- **Persistência de Dados:** Gravação e leitura do histórico de ranking em arquivos locais utilizando `QFile` e `QTextStream`.

---

## 🧱 Estrutura do Projeto

```text
battle-quiz-arena/
│
├── CMakeLists.txt              # Configuração do build
├── main.cpp                    # Ponto de entrada do programa
├── mainwindow.h                # Janela principal
├── mainwindow.cpp
├── mainwindow.ui
│
├── character.h                 # Classe base dos personagens
├── character.cpp
├── warrior.h | mage.h | archer.h  # Classes derivadas dos heróis
│
├── item.h                      # Classe base abstrata para itens do inventário
├── item.cpp
├── healthpotion.h              # Item derivado: Poção de Cura
├── attackbuff.h                # Item derivado: Elixir de Ataque
│
├── questionmanager.h           # Gerenciador do banco de dados do Quiz
├── questionmanager.cpp
│
├── docs/                       # Documentação do projeto
│   ├── analise.md
│   ├── narrativa.md
│   ├── projeto.md
│   └── testes.md
│
└── README.md
