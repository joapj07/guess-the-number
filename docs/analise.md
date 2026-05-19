---

### 📊 2. `docs/analise.md` (Análise de Requisitos)
```markdown
# Análise

## 📌 Objetivo

Desenvolver um jogo de batalha em turnos utilizando C++, Qt Creator e conceitos de Programação Orientada a Objetos. O jogador responderá perguntas técnicas para enfrentar um Chefão, gerenciará itens consumíveis e terá seu recorde salvo em um ranking local.

---

## ✅ Requisitos Funcionais

- **[RF01] Escolha de Personagem:** Permitir que o usuário escolha entre Warrior, Mage ou Archer na tela inicial.
- **[RF02] Sistema de Quiz:** Exibir perguntas de múltipla escolha (POO e Eletrônica) com 4 alternativas na tela.
- **[RF03] Combate:** Executar ataques do jogador contra o Chefão ao acertar a pergunta, e contra-ataques do Chefão caso o jogador erre.
- **[RF04] Sistema de Inventário:** O jogador inicia a partida com itens consumíveis limitados em seu inventário.
- **[RF05] Uso de Itens:** O jogador pode optar por gastar seu turno usando um item (Cura ou Bônus de Dano) em vez de responder a uma pergunta.
- **[RF06] Persistência do Ranking:** Salvar o nome do jogador e a quantidade de turnos que ele levou para vencer em um arquivo local chamado `ranking.txt`.
- **[RF07] Exibição de Histórico:** Ler o arquivo `ranking.txt` ao iniciar o programa e exibir os recordes salvos em uma tabela organizada por abas.
- **[RF08] Controle de Vida:** Controlar e exibir o HP de todos os personagens em tempo real usando barras de progresso.

---

## ⚙️ Requisitos Não Funcionais

- **[RNF01] Linguagem:** Desenvolvido puramente em C++.
- **[RNF02] Interface:** Construído usando a biblioteca gráfica Qt Widgets (`QTabWidget`, `QProgressBar`, etc).
- **[RNF03] Armazenamento:** Uso obrigatório de `QFile` e `QTextStream` para a persistência de dados.
- **[RNF04] Arquitetura POO:** Aplicação rigorosa de encapsulamento, herança, polimorfismo e agregação de classes.
