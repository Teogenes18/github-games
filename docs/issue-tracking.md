# Roteiro de atividade prática: issues e rastreamento de bugs

## 1. Objetivo
Este projeto usa o fork do repositório `githubtraining/github-games` para praticar a criação de issues, classificação por categoria, definição de prioridade, atribuição de responsáveis e revisão por pull request.

## 2. Categorias e labels

- `bug`: comportamento incorreto em relação ao esperado.
- `feature`: funcionalidade nova, inexistente no jogo.
- `enhancement`: melhoria de algo que já existe.
- `documentation`: criação ou atualização de instruções do projeto.

Prioridade recomendada:

- `priority:high`: bloqueia uso do jogo ou trabalho crítico.
- `priority:medium`: afeta funcionalidade relevante, sem bloquear totalmente.
- `priority:low`: melhoria pequena ou opcional.

Acompanhamento opcional:

- `status:in-progress`
- `status:blocked`

## 3. Exemplos de issues para este projeto

### Bug
Título: [BUG] Reiniciar partida não zera a pontuação

Descrição:
Ao reiniciar uma partida, o jogo deve voltar ao estado inicial com a pontuação zerada, sem lembrar o valor anterior.

Como reproduzir:
1. Inicie uma partida.
2. Marque alguns pontos.
3. Use a opção de reinício.
4. Observe a pontuação exibida.

Esperado:
A pontuação volta para 00000.

Observado:
A pontuação pode continuar a partir do valor anterior.

Critérios:
- [ ] A pontuação reinicia em zero.
- [ ] O estado do jogo volta ao início da partida.
- [ ] O restante do jogo continua funcionando.

### Feature
Título: [FEATURE] Modo de desafio com limite de tempo

Necessidade:
O jogo ainda não oferece uma modalidade com pressão de tempo ao jogador.

Proposta:
Implementar um modo de jogo com cronômetro e incentivo ao desempenho.

Fluxo do jogador:
1. O usuário escolhe o modo "Contra o tempo".
2. A partida inicia com limite configurado.
3. O jogo encerra ao atingir o tempo máximo.

Critérios:
- [ ] O modo fica disponível na tela inicial.
- [ ] O tempo é exibido e decrementado corretamente.
- [ ] O jogo encerra ao atingir o limite.

### Enhancement
Título: [ENHANCEMENT] Melhorar feedback visual ao fim da partida

Situação atual:
Ao terminar uma partida, a tela de Game Over apresenta informações básicas, mas sem diferenciação clara de recordes e alertas.

Melhoria proposta:
Melhorar a legibilidade da tela final com destaque para pontuação, linhas e recorde.

Benefício esperado:
O jogador entende rapidamente o resultado e o que foi alcançado.

Critérios:
- [ ] A tela final permanece clara.
- [ ] O recorde é destacado visualmente.
- [ ] A interação de reinício continua funcionando.

### Documentation
Título: [DOCS] Atualizar README com instruções de execução e controles

Conteúdo que falta ou está desatualizado:
O README atual é curto e não detalha a execução do jogo em ambiente local nem os controles disponíveis.

Seção/arquivo:
README.md

Critérios:
- [ ] O README explica como executar o projeto localmente.
- [ ] Os controles do jogo ficam documentados.
- [ ] O conteúdo foi conferido contra a interface real.

## 4. Fluxo recomendado de trabalho

1. Criar a issue no fork da equipe.
2. Definir categoria e prioridade.
3. Atribuir responsável e registrar a justificativa da prioridade.
4. Resolver a demanda em branch própria.
5. Enviar PR com referência para a issue.
6. Solicitar revisão por outro participante.
7. Realizar merge após aprovação.
8. Verificar se a issue foi fechada automaticamente ou encerrar manualmente, se necessário.

## 5. Exemplo de branch e PR

```bash
git switch main
git pull origin main
git switch -c fix/issue-12-reiniciar-pontuacao
```

No PR:

```text
Closes #12

Title: fix: reinicia pontuação ao confirmar reinício

Alterações:
- zera o estado da pontuação ao reiniciar a partida
- preserva o restante do fluxo do jogo

Teste:
- iniciar partida
- marcar pontos
- reiniciar
- confirmar que a pontuação voltou para 00000
```

## 6. Checklist de entrega

- [ ] Quatro issues criadas com categorias corretas.
- [ ] Labels e prioridades incluídas.
- [ ] Assignees definidos.
- [ ] Uma issue foi executada com branch e PR.
- [ ] O código foi revisado por outro membro.
- [ ] O merge foi realizado e a issue foi fechada.
