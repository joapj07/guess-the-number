# 🎮 Battle Quiz Arena

Projeto desenvolvido em C++ utilizando Qt Creator, Qt Widgets e conceitos avançados de Programação Orientada a Objetos.

---

## 📌 Descrição

Battle Quiz Arena é um mini jogo de batalha em turnos com interface gráfica. O jogador escolhe uma classe de personagem (Guerreiro, Mago ou Arqueiro) e enfrenta o temível Chefão da Arena ("O Grão-Mestre do Silício").

Para desferir ataques e vencer a batalha, o jogador deve responder corretamente a perguntas de múltipla escolha sobre POO e Eletrônica Básica. O jogo conta com um **Sistema de Inventário (Itens Consumíveis)** para cura ou bônus de dano e um **Sistema de Ranking Persistente**, que grava o histórico de pontuações diretamente no disco do computador para que os dados não sumam ao fechar o programa.

O sistema foi desenvolvido utilizando Qt Widgets e a navegação do jogo é organizada através de múltiplas abas (`QTabWidget`).

---

## 🎯 Objetivo

Aplicar conceitos fundamentais e avançados de Programação Orientada a Objetos utilizando uma aplicação gráfica interativa em C++.

---

## 🧠 Conceitos de POO Utilizados

- **Encapsulamento:** Atributos de vida, ataque e inventário protegidos (`protected`/`private`) e acessados via getters e setters públicos.
- **Herança:** Classes de personagens herdando da classe base `Character`, e classes de itens consumíveis herdando da classe base `Item`.
- **Polimorfismo:** Métodos virtuais puros para comportamentos de ataque customizados de cada herói e para a aplicação do efeito de cada item.
- **Associação e Agregação:** A tela principal (`MainWindow`) gerencia o ciclo do jogo (Associação), e o herói carrega uma lista de objetos do tipo `Item` (Agregação).
- **Persistência de Dados:** Manipulação de arquivos locais utilizando as classes nativas do Qt (`QFile` e `QTextStream`) para salvar e carregar o ranking de jogadores.

---

## 🧱 Estrutura do Projeto

```text
battle-quiz-arena/
│
├── CMakeLists.txt              # Configuração do build do sistema
├── main.cpp                    # Ponto de entrada do programa
├── mainwindow.h                # Header da janela principal
├── mainwindow.cpp              # Lógica da interface gráfica e turnos
├── mainwindow.ui               # Arquivo de design visual (Qt Designer)
│
├── character.h                 # Classe base dos personagens (Herói e Chefão)
├── character.cpp
├── warrior.h                   # Classe derivada (Guerreiro)
├── warrior.cpp
├── mage.h                      # Classe derivada (Mago)
├── mage.cpp
├── archer.h                    # Classe derivada (Arqueiro)
├── archer.cpp
│
├── item.h                      # Classe base abstrata para itens do inventário
├── item.cpp
├── healthpotion.h              # Item derivado (Poção de Cura)
├── healthpotion.cpp
├── attackbuff.h                # Item derivado (Elixir de Overclock)
├── attackbuff.cpp
│
├── questionmanager.h           # Gerenciador do banco de dados do Quiz
├── questionmanager.cpp
│
├── docs/                       # Documentação do projeto
│   ├── analise.md              # Requisitos e especificações
│   ├── narrativa.md            # Banco de perguntas, alternativas e falas do Chefão
│   ├── projeto.md              # Estrutura das classes e arquitetura
│   └── testes.md               # Casos de teste do sistema
│
└── README.md
