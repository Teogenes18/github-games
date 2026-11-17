## Welcome to GitHub Games

A project based learning activity for people who are getting started with Git and GitHub.

You can play the game at: https://githubschool.github.io/github-games/

>> _*SUPPORTED BROWSERS*: Chrome, Firefox, Safari, Opera and IE9+_

This fun open source game was cloned from: https://github.com/jakesgordon/javascript-tetris

## Modos de jogo

O modo é escolhido na tela inicial, antes de clicar em **Jogar** (ou apertar Enter). As opções de tempo limite e de meta de linhas só ficam ativas no modo correspondente.

| Modo | Objetivo | Opções | Como a partida termina |
|---|---|---|---|
| **Padrão** | Fazer a maior pontuação possível, sem limite de tempo | nenhuma | **Game Over**, quando as peças chegam ao topo (ou ESC) |
| **Contra o tempo** | Fazer a maior pontuação antes de o tempo acabar | tempo limite: 1, 2 (padrão), 3 ou 5 min | **Tempo esgotado!** quando o cronômetro chega a `00:00`, ou **Game Over** antes disso |
| **Desafio de linhas** | Completar a meta de linhas | meta: 5, 10, 20 (padrão) ou 40 linhas | **Você venceu!** ao atingir a meta, ou **Game Over** antes disso |

### Padrão
- O cronômetro conta o tempo jogado (pausas não contam).
- As peças caem mais rápido conforme as linhas são completadas.

### Contra o tempo
- O cronômetro conta para trás, a partir do tempo limite escolhido.
- A velocidade aumenta com as linhas e também com o tempo: quanto menos tempo resta, mais rápido as peças caem.
- Nos últimos 10 segundos, o cronômetro fica vermelho e pisca.
- **Apagão:** de tempos em tempos (a cada 10 a 20 segundos), o tabuleiro escurece por 2 segundos, e o jogador precisa continuar jogando "no escuro".

### Desafio de linhas
- O cronômetro conta o tempo jogado.
- A velocidade aumenta conforme as linhas são completadas, como no modo Padrão.
- A vitória acontece assim que o total de linhas completadas chega à meta.

## Pontuação

Cada peça fixada no tabuleiro adiciona 10 pontos. Quando uma jogada completa `n` linhas de uma vez, ela também adiciona um bônus de `100 × 2^(n - 1)` pontos: 1 linha vale 100 pontos, 2 valem 200, 3 valem 400 e 4 valem 800.
