---

### 🧪 4. `docs/testes.md`
```markdown
# Testes

## ✅ Teste 1 - Escolha de personagem

Ação:
Selecionar o personagem desejado na tela inicial.

Resultado esperado:
Instância do herói correspondente carregada na memória com seus atributos específicos.

---

## ✅ Teste 2 - Resposta correta (Ataque ao Chefão)

Ação:
Clicar na alternativa correta dentre as opções na tela.

Resultado esperado:
O jogador executa seu ataque polimórfico e o Chefão recebe dano, diminuindo sua barra de vida. O Chefão não ataca neste turno.

---

## ✅ Teste 3 - Resposta incorreta (Contra-ataque do Chefão)

Ação:
Clicar em uma alternativa incorreta de pergunta na tela.

Resultado esperado:
O jogador falha em atacar e o Chefão executa um contra-ataque automático, diminuindo a barra de vida do jogador.

---

## ✅ Teste 4 - Vitória contra o Chefão

Ação:
Reduzir a vida (HP) do Chefão para 0.

Resultado esperado:
O jogo encerra o combate, bloqueia os botões de alternativas e exibe uma mensagem de Vitória na tela.

---

## ✅ Teste 5 - Derrota para o Chefão

Ação:
Reduzir a vida (HP) do jogador para 0 devido aos ataques do Chefão.

Resultado esperado:
O jogo interrompe a partida e exibe uma mensagem de Derrota/Game Over na tela.
