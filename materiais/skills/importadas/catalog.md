# Skills da comunidade

Este é um catálogo de Skills incremental, separado por área de aplicação e pacote de skills pertencente.

Estou deixando um método de instalar (o meu preferido) recomendado, que é usando o CLI Skills, da Vercel Labs:

Segue a [referência oficial da CLI Skills](https://github.com/vercel-labs/skills/blob/main/docs/commands.md).

O comando roda com `npx skills add {url do repo/skill/afins}`

Sem mais delongas, ás skills:

## Fluxos de trabalho com agentes

### [`obra/superpowers`](https://github.com/obra/superpowers)

Coleção de skills para estruturar o trabalho de agentes, do entendimento do pedido à implementação e revisão.

#### `using-superpowers`

Ajuda o agente a reconhecer e aplicar o fluxo de trabalho apropriado.

#### `brainstorming`

Explora objetivos, restrições e abordagens antes de iniciar um trabalho novo.

#### `writing-plans`

Transforma requisitos e decisões em um plano de implementação.

#### `executing-plans`

Executa um plano aprovado em etapas verificáveis.

#### `dispatching-parallel-agents`

Divide trabalho independente entre agentes e coordena os resultados.

#### `subagent-driven-development`

Coordena implementação e revisão com subagentes em tarefas separáveis.

#### `using-git-worktrees`

Prepara um worktree isolado para trabalhar em uma mudança.

#### `finishing-a-development-branch`

Ajuda a concluir uma branch e escolher como integrar o trabalho.

#### `systematic-debugging`

Investiga bugs e comportamentos inesperados antes de propor uma correção.

#### `test-driven-development`

Organiza a implementação começando por testes que descrevem o comportamento esperado.

#### `diagnosing-superpowers`

Investiga o que causou problemas durante o uso de um fluxo de trabalho com skills.

#### `requesting-code-review`

Prepara uma revisão de código após uma implementação.

#### `receiving-code-review`

Analisa comentários de revisão antes de decidir como aplicá-los.

#### `verification-before-completion`

Confere as evidências necessárias antes de declarar uma tarefa concluída.

#### `writing-skills`

Cria, atualiza e verifica skills e seus arquivos de apoio.

Comando para adicionar todas as skills deste subgrupo:

```bash
npx skills add obra/superpowers \
  --skill using-superpowers \
  --skill brainstorming \
  --skill writing-plans \
  --skill executing-plans \
  --skill dispatching-parallel-agents \
  --skill subagent-driven-development \
  --skill using-git-worktrees \
  --skill finishing-a-development-branch \
  --skill systematic-debugging \
  --skill test-driven-development \
  --skill diagnosing-superpowers \
  --skill requesting-code-review \
  --skill receiving-code-review \
  --skill verification-before-completion \
  --skill writing-skills
```
## Otimização de uso

### [`DietrichGebert/ponytail`](https://github.com/DietrichGebert/ponytail)

Ponytail orienta o agente a resolver a tarefa com a menor mudança que a conclua por inteiro. Ele incentiva o reuso do que já existe e evita abstrações e dependências sem necessidade. Mantém validação, segurança, tratamento de erros, acessibilidade e testes quando a mudança exige esses cuidados.

#### `ponytail`

Aplica esse modo de trabalho durante tarefas de programação, buscando uma solução pequena e completa.

#### `ponytail-review`

Revisa uma mudança específica em busca de bugs, riscos de segurança, falhas sob carga, testes ausentes e código desnecessário. Apenas apresenta os achados.

#### `ponytail-audit`

Faz uma revisão do repositório inteiro e ordena os problemas por prioridade, incluindo complexidade que pode ser removida.

#### `ponytail-debt`

Reúne comentários `shortcut:` ou `ponytail:` em uma lista de simplificações pendentes e seus critérios para revisão.

#### `ponytail-gain`

Mostra os indicadores medidos pelo projeto Ponytail sobre tamanho de código, custo e velocidade.

#### `ponytail-help`

Resume os níveis de uso e os comandos disponíveis. Não altera o projeto.

Comando para adicionar as seis skills deste repositório:

```bash
npx skills add DietrichGebert/ponytail --skill '*'
```


## Design de telas

### [`nextlevelbuilder/ui-ux-pro-max-skill`](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)

Repositório de design para interfaces, sistemas visuais, identidade de marca, banners e apresentações.

#### `design`

Ajuda a criar identidade visual, tokens e materiais de interface.

#### `design-system`

Organiza tokens de design e especificações de componentes.

#### `ui-ux-pro-max`

Ajuda a projetar experiências e interfaces para web, mobile e desktop.

#### `ui-styling`

Orienta a estilização com shadcn/ui, Radix UI, Tailwind e canvas.

#### `brand`

Ajuda a definir voz, identidade visual e consistência de marca.

#### `banner-design`

Cria banners para redes sociais, anúncios, sites e materiais impressos.

#### `slides`

Planeja apresentações em HTML, com estrutura narrativa e visual.

Comando para adicionar todas as skills deste subgrupo:

```bash
npx skills add nextlevelbuilder/ui-ux-pro-max-skill \
  --skill design \
  --skill design-system \
  --skill ui-ux-pro-max \
  --skill ui-styling \
  --skill brand \
  --skill banner-design \
  --skill slides
```

### [`Leonxlnx/taste-skill`](https://github.com/Leonxlnx/taste-skill)

Skills para orientar a criação de interfaces frontend com direção visual definida.

#### `design-taste-frontend`

Ajuda a criar páginas com hierarquia, tipografia, espaçamento e estilo visual coerentes.

Comando para adicionar todas as skills deste subgrupo:

```bash
npx skills add Leonxlnx/taste-skill --skill design-taste-frontend
```

### [`emilkowalski/skills`](https://github.com/emilkowalski/skills)

Coleção de skills de design de interface, prototipagem, usabilidade e implementação frontend.

#### `emil-design-eng`

Orienta o acabamento visual, o desenho de componentes e os detalhes das interações.

#### `prototype`

Cria variações de uma interface para comparar abordagens antes de escolher uma.

#### `pick-ui-library`

Ajuda a escolher bibliotecas para componentes e interações de interface.

#### `break-ui`

Procura problemas de layout usando conteúdo extremo ou incomum.

#### `mobile-native`

Adapta interfaces web para uma experiência mais natural em celulares.

Comando para adicionar todas as skills deste subgrupo:

```bash
npx skills add emilkowalski/skills \
  --skill emil-design-eng \
  --skill prototype \
  --skill pick-ui-library \
  --skill break-ui \
  --skill mobile-native
```

### [`pbakaus/impeccable`](https://github.com/pbakaus/impeccable)

Skill de avaliação e refinamento de interfaces frontend. A origem não consta no arquivo local de instalação; este comando aponta para a skill pública atual no GitHub.

#### `impeccable`

Ajuda a projetar, revisar, simplificar e polir interfaces, incluindo conteúdo, acessibilidade e comportamento responsivo.

Comando para adicionar todas as skills deste subgrupo:

```bash
npx skills add https://github.com/pbakaus/impeccable/tree/main/.agent/skills/impeccable
```

## Animação e interação

### [`emilkowalski/skills`](https://github.com/emilkowalski/skills)

Skills para planejar, implementar e revisar animações e interações em interfaces web e mobile.

#### `animate`

Projeta e implementa animações web com movimento adequado ao propósito da interface.

#### `animate-expo`

Implementa animações em aplicações React Native e Expo.

#### `animation-performance`

Analisa gargalos e melhora o desempenho de animações web.

#### `animation-vocabulary`

Identifica o nome técnico de um efeito de movimento descrito informalmente.

#### `apple-design`

Aplica princípios de interface e movimento associados ao design da Apple.

#### `choreograph`

Coordena o movimento de vários elementos para que a animação funcione como uma sequência.

#### `find-animation-opportunities`

Analisa uma interface e sugere onde uma animação pode ajudar a experiência.

#### `gestures`

Implementa interações de arrastar, deslizar e flingar em interfaces.

#### `improve-animations`

Audita animações existentes e propõe correções em ordem de prioridade.

#### `remove-animations`

Identifica animações que atrapalham a leitura ou o uso e orienta sua remoção.

#### `review-animations`

Revisa a implementação de animações e interações com foco em qualidade visual e técnica.

Comando para adicionar todas as skills deste subgrupo:

```bash
npx skills add emilkowalski/skills \
  --skill animate \
  --skill animate-expo \
  --skill animation-performance \
  --skill animation-vocabulary \
  --skill apple-design \
  --skill choreograph \
  --skill find-animation-opportunities \
  --skill gestures \
  --skill improve-animations \
  --skill remove-animations \
  --skill review-animations
```

## Revisão de código

### [`awesome-skills/code-review-skill`](https://github.com/awesome-skills/code-review-skill)

Orientação de revisão para identificar problemas em código de diferentes linguagens e frameworks.

#### `code-review-skill`

Aplica critérios de revisão de acordo com a tecnologia do projeto.

Comando para adicionar todas as skills deste subgrupo:

```bash
npx skills add awesome-skills/code-review-skill --skill code-review-skill
```

## Escrita e comunicação

### [`blader/humanizer`](https://github.com/blader/humanizer)

Skill para revisar textos e remover padrões que soam genéricos ou artificiais.

#### `humanizer`

Reescreve textos preservando o sentido e ajustando ritmo, estrutura e linguagem.

Comando para adicionar todas as skills deste subgrupo:

```bash
npx skills add blader/humanizer --skill humanizer
```

### [`hardikpandya/stop-slop`](https://github.com/hardikpandya/stop-slop)

Skill para edição concisa e direta de textos.

#### `stop-slop`

Corta enchimento, exageros e construções previsíveis.

Comando para adicionar todas as skills deste subgrupo:

```bash
npx skills add hardikpandya/stop-slop --skill stop-slop
```

## Desenvolvimento e bibliotecas

### [`emilkowalski/skills`](https://github.com/emilkowalski/skills)

O repositório também inclui skills pontuais para Swift e componentes React.

#### `write-swift`

Orienta a escrita de Swift moderno, incluindo concorrência e segurança de tipos.

#### `ask-sonner`

Ajuda a integrar notificações com a biblioteca Sonner em projetos React.

Comando para adicionar todas as skills deste subgrupo:

```bash
npx skills add emilkowalski/skills \
  --skill write-swift \
  --skill ask-sonner
```

## Vercel

### [`vercel-labs/agent-skills`](https://github.com/vercel-labs/agent-skills)

Skills para publicar aplicações e cuidar de projetos hospedados na Vercel.

#### `deploy-to-vercel`

Orienta a publicação de sites e aplicações na Vercel.

#### `vercel-cli-with-tokens`

Usa a CLI da Vercel com autenticação por token.

#### `vercel-optimize`

Analisa custos e desempenho de projetos hospedados na Vercel.

Comando para adicionar todas as skills deste subgrupo:

```bash
npx skills add vercel-labs/agent-skills \
  --skill deploy-to-vercel \
  --skill vercel-cli-with-tokens \
  --skill vercel-optimize
```
