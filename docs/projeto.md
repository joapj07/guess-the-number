# Projeto (Arquitetura Atualizada)

## 🧱 Novas Classes e Modificações

### Modificação em Character
A classe base `Character` agora agrega uma lista ou vetor de itens (`QList<Item*>`), representando o inventário do personagem. Foram adicionados métodos como `useItem(int index)` e `addItem(Item* item)`.

### Item (Classe Abstrata)
Classe base para todos os consumíveis do jogo.
- **Atributos:** `QString name`, `QString description`.
- **Método Virtual Puro:** `virtual void applyEffect(Character* target) = 0;`

### HealthPotion (Herda de Item)
Implementa o método `applyEffect` para restaurar uma quantidade fixa de HP (ex: +50 HP) no personagem do jogador.

### AttackBuff (Herda de Item)
Implementa o método `applyEffect` para aumentar temporariamente o atributo de ataque do jogador para o próximo turno.

### Fluxo de Persistência (MainWindow)
A classe `MainWindow` utilizará manipulação de arquivos para persistência de dados:
1. Ao iniciar, chama uma função interna que abre o arquivo `ranking.txt` via `QFile`, lê linha por linha e joga os dados para dentro do componente visual de tabela (`QTableWidget`).
2. Ao finalizar o jogo com vitória, abre o arquivo `ranking.txt` em modo de escrita/anexo (`QIODevice::Append`) e salva a nova pontuação formatada.

---

## 🧠 Diagramas de Herança do Projeto

### Personagens:
```text
Character (Heróis e Chefão)
 ├── Warrior
 ├── Mage
 └── Archer
