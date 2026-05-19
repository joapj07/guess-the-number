# 🎮 Battle Quiz Arena - Ultimate Edition

Projeto desenvolvido em C++ utilizando Qt Creator, Qt Widgets e conceitos de Programação Orientada a Objetos.

---

## 📌 Descrição

Battle Quiz Arena é um RPG de texto e quiz em turnos com interface gráfica. O jogador escolhe uma classe de personagem (Guerreiro, Mago ou Arqueiro) e enfrenta o temível "Grão-Mestre do Silício".

Esta versão expandida conta com:
- **Sistema de Quiz Técnico:** Perguntas de POO e Eletrônica Básica.
- **Sistema de Inventário:** Itens consumíveis com herança e polimorfismo.
- **Persistência de Dados Dupla:** Gravação de Ranking local e exportação de logs de combate para arquivos `.txt`.
- **Eventos Aleatórios:** Modificadores de partida a cada turno (Fator RPG).
- **Sistema de Conquistas (Achievements):** Desbloqueio de medalhas por feitos na arena.
- **Customização Estética:** Alternância em tempo de execução entre os temas "Terminal Hacker" (Escuro) e "Laboratório" (Claro).

---

## 🧠 Conceitos de POO Utilizados

- **Encapsulamento:** Atributos de personagens, itens e conquistas protegidos e expostos via métodos de acesso seguros.
- **Herança e Polimorfismo:** Aplicados nos Personagens (classes derivadas de `Character`) e nos Itens (classes derivadas de `Item`).
- **Agregação e Composição:** O herói agrega uma lista de ponteiros de `Item`, e a `MainWindow` compõe a lista de `Achievement`.
- **Persistência e Arquivos:** Fluxo de entrada e saída (I/O) de arquivos com `QFile` e `QTextStream` para persistência do ranking e geração de relatórios de partida (Logs).

---

## 🧱 Estrutura do Projeto

```text
battle-quiz-arena/
│
├── CMakeLists.txt              # Configuração do build
├── main.cpp                    # Ponto de entrada
├── mainwindow.h | mainwindow.cpp | mainwindow.ui
│
├── character.h | character.cpp
├── warrior.h | mage.h | archer.h
│
├── item.h | item.cpp
├── healthpotion.h | attackbuff.h
│
├── questionmanager.h | questionmanager.cpp
│
├── docs/                       # Documentação do projeto
│   ├── analise.md
│   ├── narrativa.md            # Perguntas, falas, eventos e conquistas
│   ├── projeto.md
│   └── testes.md
│
└── README.md
