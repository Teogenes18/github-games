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

Os exemplos abaixo correspondem a demandas registradas no fork, não a defeitos ou necessidades hipotéticas:

### Bug — [#31](https://github.com/Teogenes18/github-games/issues/31)
O índice aleatório usa um limite superior exclusivo que impede a seleção do último item do saco de peças. A demanda pode ser verificada inspecionando `randomPiece()` e testando uma escolha próxima ao limite superior.

### Feature — [#13](https://github.com/Teogenes18/github-games/issues/13)
A contagem regressiva 3-2-1 ao sair da pausa era uma funcionalidade nova. A issue foi implementada e encerrada pela [PR #16](https://github.com/Teogenes18/github-games/pull/16).

### Enhancement — [#14](https://github.com/Teogenes18/github-games/issues/14)
A sombra já podia ser alternada com G, mas a escolha não era lembrada após recarregar e seu estado não era indicado no painel.

### Documentation — [#15](https://github.com/Teogenes18/github-games/issues/15)
A issue pede que o README documente os controles existentes e a pausa automática ao perder o foco.

### Investigação de possível bug — [#12](https://github.com/Teogenes18/github-games/issues/12)
Esta issue permanece explicitamente como investigação: o GitHub Pages não está publicado, então a falha no endereço principal ainda não foi reproduzida. Uma resposta 404 sem uma publicação ativa não confirma o defeito. Ative o Pages e repita os passos descritos na issue antes de alterar o jogo ou classificá-la como bug confirmado.

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
git switch -c fix/issue-31-piece-selection
```

No PR:

```text
Closes #31

Title: fix: inclui o último item no sorteio de peças

Alterações:
- sorteia um índice inteiro em todo o intervalo do saco
- permite que o último item também seja escolhido

Teste:
- testar a seleção com um valor aleatório próximo ao limite superior
- confirmar que o último tipo de peça pode ser sorteado
```

## 6. Checklist de entrega

- [ ] Uma issue pertinente para cada categoria.
- [ ] Labels e prioridades incluídas.
- [ ] Assignees definidos.
- [ ] A prioridade foi justificada em comentário.
- [ ] A issue escolhida foi implementada em branch própria e vinculada ao PR com `Closes #N`.
- [ ] O código foi revisado por outro membro.
- [ ] Após aprovação, o merge foi realizado, a issue foi fechada e a alteração validada na `main`.
- [ ] Links e evidências da entrega foram registrados.
