# Projeto

## 📌 Estrutura do Sistema

O sistema foi desenvolvido utilizando três classes principais:

---

🧱 Classes

Game
Responsável pela lógica do jogo:
- Geração do número aleatório
- Verificação dos palpites
- Controle do fluxo do jogo

---

Player
Responsável por armazenar dados do jogador:
- Nome
- Número de tentativas

---

ScoreManager
Responsável pelo gerenciamento de ranking:
- Salvar resultados em arquivo
- Ler e exibir ranking

---

🔗 Relação entre as Classes

- Game utiliza Player para armazenar dados do jogador
- Game utiliza ScoreManager para salvar e exibir resultados

---

🎯 Objetivo da Arquitetura

Separar responsabilidades para facilitar:
- Organização do código
- Manutenção
- Reutilização
