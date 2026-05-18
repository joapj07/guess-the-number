# Testes

## ✅ Teste 1 - Escolha de personagem

Ação:
Selecionar uma classe na tela de seleção (Warrior, Mage ou Archer).

Resultado esperado:
Instância do personagem correspondente carregada corretamente na memória com seus respectivos atributos de HP e ataque iniciais.

---

## ✅ Teste 2 - Resposta correta

Ação:
Responder à pergunta do quiz corretamente.

Resultado esperado:
O jogador executa seu ataque polimórfico (`performAttack()`) e o HP do inimigo diminui com base no poder de ataque do personagem escolhido.

---

## ✅ Teste 3 - Resposta incorreta

Ação:
Responder à pergunta do quiz incorretamente (ou estourar o tempo, se houver).

Resultado esperado:
O inimigo contra-ataca e o jogador recebe dano, diminuindo o seu valor atual de HP (`receiveDamage()`).

---

## ✅ Teste 4 - Vitória

Ação:
Reduzir a vida (HP) do inimigo para 0.

Resultado esperado:
O jogo bloqueia novas ações, exibe uma tela ou mensagem de vitória e salva a pontuação no ranking.

---

## ✅ Teste 5 - Derrota

Ação:
Reduzir a vida (HP) do jogador para 0.

Resultado esperado:
O jogo interrompe a partida, exibe uma mensagem de "Game Over" (derrota) e redireciona o jogador para a tela inicial ou ranking.
