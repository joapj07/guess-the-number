# Testes

## ✅ Teste 1 - Escolha de personagem
Ação: Selecionar o personagem desejado na tela inicial.
Resultado esperado: Instância do herói correspondente carregada na memória com seus atributos específicos.

## ✅ Teste 2 - Resposta correta (Ataque ao Chefão)
Ação: Clicar na alternativa correta dentre as opções na tela.
Resultado esperado: O jogador executa seu ataque polimórfico e o Chefão recebe dano, diminuindo sua barra de vida. O Chefão não ataca neste turno.

## ✅ Teste 3 - Resposta incorreta (Contra-ataque do Chefão)
Ação: Clicar em uma alternativa incorreta de pergunta na tela.
Resultado esperado: O jogador falha em atacar e o Chefão executa um contra-ataque automático, diminuindo a barra de vida do jogador e exibindo uma provocação no log.

## ✅ Teste 4 - Uso de Item Consumível (Cura)
Ação: Durante o combate, clicar no botão "Usar Poção de Cura".
Resultado esperado: O item é removido do inventário, o HP do jogador aumenta em 50 pontos, o Chefão solta uma frase de reclamação e não ataca neste turno.

## ✅ Teste 5 - Gravação e Leitura do Ranking (Persistência)
Ação: Vencer o jogo, salvar o nome e reiniciar o programa.
Resultado esperado: O programa grava os dados no arquivo `ranking.txt` e, ao reabrir, renderiza a lista salva diretamente na tabela da interface gráfica.

## ✅ Teste 6 - Vitória ou Derrota
Ação: Reduzir o HP do Chefão ou do Jogador a 0.
Resultado esperado: O jogo bloqueia os comandos, sorteia uma das frases temáticas de fim de jogo e encerra o combate.
