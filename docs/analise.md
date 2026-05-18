### 📊 2. `docs/analise.md` (Novos Requisitos)
```markdown
# Análise (Atualizada)

## 📌 Objetivo
Desenvolver um jogo de batalha em turnos utilizando C++, Qt e POO, focado no combate contra um Chefão através de um Quiz técnico, incluindo gerenciamento de recursos (itens) e armazenamento persistente.

---

## ✅ Requisitos Funcionais (Novos & Atualizados)

- **[RF01] Escolha de Personagem:** Escolher entre Warrior, Mage ou Archer.
- **[RF02] Sistema de Quiz:** Exibir perguntas com 4 alternativas e validar a resposta.
- **[RF03] Combate:** Atacar o Chefão ao acertar; receber contra-ataque ao errar.
- **[RF04] Sistema de Inventário:** O jogador inicia a partida com itens consumíveis limitados (ex: 2 Poções de Cura, 1 Elixir de Ataque).
- **[RF05] Uso de Itens:** O jogador pode optar por usar um item em seu turno em vez de responder a uma pergunta.
- **[RF06] Persistência do Ranking:** Salvar o nome do jogador e seu recorde em um arquivo local (`ranking.txt`) ao vencer.
- **[RF07] Exibição de Histórico:** Ler o arquivo `ranking.txt` ao abrir o jogo e renderizar o ranking atualizado na interface gráfica.

---

## ⚙️ Requisitos Não Funcionais

- Persistência utilizando as bibliotecas nativas do Qt (`QFile` e `QTextStream`).
- Aplicação de Herança e Polimorfismo tanto nos Personagens quanto nos Itens.
