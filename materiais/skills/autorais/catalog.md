# Skills autorais

Este é um catálogo de Skills incremental, separado por área de aplicação e pacote de skills pertencente.

Sem mais delongas, ás skills:

## Scrum e facilitação

### [`luiisprotasio/scrum-master`](https://github.com/luiisprotasio/scrum-master)

Grupo autoral de skills voltado ao trabalho de Scrum Master.

#### `writing-cards`

Skill que auxilia na criação de cards a partir de conteúdo de qualquer tipo.
Tem um documento de escopo, notas de reunião, ou até mesmo um documento de texto informal, contedo qualquer tipo de especificação do projeto? Esta skill transforma conteúdo solto em cards organizados e padronizados, além de automatizar o upload para o GitHub no formato de issues.

Inputs necessários: 
- É preciso um documento/texto explicando algum tipo de escopo/ideia/projeto.
- É preciso identificar a qual repositório remoto (github) as tarefas serão linkadas caso queria a sincronizaçãoa, alternativamente, serão criados todos localmente, em markdown.
- Ainda sobre sincronização: garanta que seu GitHub CLI esteja logado corretamente! A sincronização ocorre por meio do mesmo.

Comando para adicionar todas as skills deste repositório:

```bash
npx skills add luiisprotasio/scrum-master --skill '*'
```
