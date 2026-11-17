# Entrega: issues e rastreamento de bugs

> Rascunho para anexar à atividade no Class. Substitua os logins pelos nomes completos dos participantes antes de enviar.

## Repositório e participantes

- Repositório da equipe: https://github.com/Teogenes18/github-games
- Participantes identificados no histórico de issues:
  - `Teogenes18` — nome completo: preencher
  - `Caique-Souza1` — nome completo: preencher
  - `deniselmatos` — nome completo: preencher
  - `ZeCarlos18` — nome completo: preencher
  - `Reullyson` (Eric Reullyson)

## Issues por participante

O PDF identifica cinco integrantes, mas as 16 issues (#12 a #31) estão distribuídas entre quatro autores. A linha de `Reullyson` está vazia no quadro de autoria; portanto, o conjunto atual não comprova quatro issues individuais para Eric.

| Participante (GitHub) | Categoria | Issue | Prioridade | Responsável | Situação |
|---|---|---:|---|---|---|
| `Teogenes18` | bug | [#12](https://github.com/Teogenes18/github-games/issues/12) | high | Teogenes18 | Investigação; não reproduzido |
| `Teogenes18` | feature | [#13](https://github.com/Teogenes18/github-games/issues/13) | medium | Teogenes18 | Fechada pela PR #16 |
| `Teogenes18` | enhancement | [#14](https://github.com/Teogenes18/github-games/issues/14) | low | Teogenes18 | Aberta |
| `Teogenes18` | documentation | [#15](https://github.com/Teogenes18/github-games/issues/15) | medium | Teogenes18 | Aberta |
| `Caique-Souza1` | bug | [#18](https://github.com/Teogenes18/github-games/issues/18) | medium | Caique-Souza1 | Aberta |
| `Caique-Souza1` | feature | [#19](https://github.com/Teogenes18/github-games/issues/19) | low | Caique-Souza1 | Aberta |
| `Caique-Souza1` | enhancement | [#20](https://github.com/Teogenes18/github-games/issues/20) | medium | Caique-Souza1 | Fechada pela PR #23 |
| `Caique-Souza1` | documentation | [#21](https://github.com/Teogenes18/github-games/issues/21) | low | Caique-Souza1 | Aberta |
| `deniselmatos` | bug | [#31](https://github.com/Teogenes18/github-games/issues/31) | medium | **não atribuído** | PR #35 aberta |
| `deniselmatos` | feature | [#17](https://github.com/Teogenes18/github-games/issues/17) | medium | **não atribuído** | Aberta |
| `deniselmatos` | enhancement | [#22](https://github.com/Teogenes18/github-games/issues/22) | medium | **não atribuído** | Aberta |
| `deniselmatos` | documentation | [#24](https://github.com/Teogenes18/github-games/issues/24) | low | ZeCarlos18 | Fechada pela PR #30 |
| `ZeCarlos18` | bug | [#25](https://github.com/Teogenes18/github-games/issues/25) | low | ZeCarlos18 | Fechada pela PR #29 |
| `ZeCarlos18` | feature | [#26](https://github.com/Teogenes18/github-games/issues/26) | medium | ZeCarlos18 | Aberta |
| `ZeCarlos18` | enhancement | [#27](https://github.com/Teogenes18/github-games/issues/27) | low | ZeCarlos18 | Aberta |
| `ZeCarlos18` | documentation | [#28](https://github.com/Teogenes18/github-games/issues/28) | low | ZeCarlos18 | Aberta |
| `Reullyson` | bug | — | — | — | **Issue não registrada no PDF** |
| `Reullyson` | feature | — | — | — | **Issue não registrada no PDF** |
| `Reullyson` | enhancement | — | — | — | **Issue não registrada no PDF** |
| `Reullyson` | documentation | — | — | — | **Issue não registrada no PDF** |

### Comparação de escopo

Não há títulos nem critérios idênticos entre as 16 issues listadas. Há temas próximos, mas com objetivos diferentes:

- [#17](https://github.com/Teogenes18/github-games/issues/17) guarda o histórico das últimas partidas; [#19](https://github.com/Teogenes18/github-games/issues/19) propõe um ranking das melhores pontuações.
- [#19](https://github.com/Teogenes18/github-games/issues/19) pede um ranking geral; [#20](https://github.com/Teogenes18/github-games/issues/20) separa o recorde por modo.
- [#25](https://github.com/Teogenes18/github-games/issues/25) corrige o alerta visual que persiste após o fim; [#27](https://github.com/Teogenes18/github-games/issues/27) propõe um aviso sonoro durante os últimos dez segundos.
- [#26](https://github.com/Teogenes18/github-games/issues/26) adiciona tempo por linha; [#27](https://github.com/Teogenes18/github-games/issues/27) adiciona aviso sonoro. Ambos afetam o modo Contra o Tempo, mas não são a mesma funcionalidade.
- [#12](https://github.com/Teogenes18/github-games/issues/12) investiga a publicação do jogo; [#28](https://github.com/Teogenes18/github-games/issues/28) atualiza a apresentação e o link do README.
- [#15](https://github.com/Teogenes18/github-games/issues/15), [#21](https://github.com/Teogenes18/github-games/issues/21), [#24](https://github.com/Teogenes18/github-games/issues/24) e [#28](https://github.com/Teogenes18/github-games/issues/28) tratam de seções diferentes do README.

As alterações feitas nesta continuação nas PRs #35, #36 e #37 trabalham, respectivamente, nas issues #31 (Denise), #14 (Teogenes) e #15 (Teogenes). Elas ajudam o projeto, mas não contam como quatro issues próprias e inéditas de `Reullyson`.

## Quatro issues selecionadas e implementadas

As quatro entregas abaixo são trabalho coletivo já presente na main; não são autoria individual de `Reullyson`.

| Categoria | Issue | Branch | Pull request | Revisão e conclusão |
|---|---|---|---|---|
| bug | [#25](https://github.com/Teogenes18/github-games/issues/25) | `fix/issue-25-alerta-cronometro` | [PR #29](https://github.com/Teogenes18/github-games/pull/29) | Aprovada por Teogenes18; merge realizado; issue fechada |
| feature | [#13](https://github.com/Teogenes18/github-games/issues/13) | `feature/issue-13-contagem-pausa` | [PR #16](https://github.com/Teogenes18/github-games/pull/16) | Aprovada por ZeCarlos18; merge realizado; issue fechada |
| enhancement | [#20](https://github.com/Teogenes18/github-games/issues/20) | `enhancement/issue-20-recorde-por-modo` | [PR #23](https://github.com/Teogenes18/github-games/pull/23) | Aprovada por Teogenes18; merge realizado; issue fechada |
| documentation | [#24](https://github.com/Teogenes18/github-games/issues/24) | `docs/issue-24-modos-de-jogo` | [PR #30](https://github.com/Teogenes18/github-games/pull/30) | Aprovada por Caique-Souza1; merge realizado; issue fechada |

As quatro PRs referenciam a issue correspondente com `Closes #N`. Os comentários de revisão registram testes e observações técnicas; os detalhes estão nas páginas de cada PR.

## Investigação de possível bug

A [issue #12](https://github.com/Teogenes18/github-games/issues/12) continua identificada como investigação, não como defeito confirmado. O GitHub Pages não está publicado; os endereços do fork retornam 404, o que não permite testar a hipótese do arquivo `inde.html`. A confirmação depende de ativar o Pages e repetir os passos registrados na issue.

## Pendências administrativas

- Registrar quatro issues novas e não duplicadas para `Reullyson`, uma por categoria, com labels, prioridade, assignee, justificativa e critérios verificáveis. A issue de bug precisa ser reproduzida; se não houver defeito confirmado, registrar explicitamente uma investigação, como foi feito na #12.
- Atribuir responsáveis às issues [#17](https://github.com/Teogenes18/github-games/issues/17), [#22](https://github.com/Teogenes18/github-games/issues/22) e [#31](https://github.com/Teogenes18/github-games/issues/31), atualmente sem assignee.
- As PRs adicionais [#35](https://github.com/Teogenes18/github-games/pull/35), [#36](https://github.com/Teogenes18/github-games/pull/36) e [#37](https://github.com/Teogenes18/github-games/pull/37) estão abertas e aguardam revisão de outro integrante antes do merge; não são necessárias para a seleção de quatro PRs já concluídas acima.
- A descrição da PR [#34](https://github.com/Teogenes18/github-games/pull/34) ainda cita uma alteração no README, embora o diff atual não o altere; corrigir a descrição antes do merge.
- Preencher os nomes completos dos participantes antes de enviar este documento ao Class.
