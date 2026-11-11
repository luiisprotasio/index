# Conceitos básicos de desenvolvimento com IA

## CLI de IA e seu uso

CLI (*command-line interface*) é uma interface usada pelo terminal. Uma CLI de IA permite conversar com um modelo ou agente a partir da pasta do projeto. Dependendo da ferramenta e das permissões configuradas, o agente pode ler e editar arquivos, além de executar comandos.
Alguns exemplos de CLI de IA:
Antigravity, Claude Code, Codex, OpenCode, Cursor.
Observe que não se precisa ser uma fornecedora de modelos para ter um app que roda os mesmos! (tanto que o antigravity roda Opus e GPT)

Um fluxo comum:

1. Abra o terminal na pasta do projeto e inicie a ferramenta.
2. Descreva a tarefa, o contexto e as restrições. Diga também como espera receber o resultado.
3. Revise as alterações propostas e os comandos executados. Rode os testes ou verificações adequados antes de aceitar a mudança.

**Exemplo de uso comum**(considerando o Codex, que é o padrão da empresa hoje): 
1. `codex`
2. “Leia `src/`, encontre por que o formulário não envia e proponha uma correção. Preserve o estilo atual e explique como validar.”

## MCP e Connectors

MCP (*Model Context Protocol*) é um protocolo aberto que padroniza a comunicação entre aplicações de IA e serviços externos. Um servidor MCP pode oferecer ferramentas para executar ações ou recursos para consultar dados. A aplicação de IA, como cliente, conversa com esses servidores.

Um *connector* (conector) é uma integração configurada entre uma aplicação de IA e um serviço, como um repositório ou uma ferramenta de gestão de tarefas. Ele pode disponibilizar busca, leitura de dados ou ações, conforme as permissões concedidas. Alguns conectores usam MCP; o termo também pode descrever integrações feitas de outras formas.

**Em resumo:** MCP define uma forma de comunicação; o conector é a integração que você configura e usa. Antes de habilitar um, confira quais dados e ações ele pode acessar.

**Exemplos usados frequentemente:** 
1. MCP do Notion, permite alteração e leitura de bases de dados do Notion diretamente pelo agente de IA.
2. Connector do Github, permite leitura e alteração de repositórios automáticos com IA.

## Skills

Uma *skill* é um conjunto reutilizável de instruções e materiais que orienta um agente a realizar um tipo de tarefa. Pode incluir exemplos, modelos ou scripts. Em geral, um arquivo `SKILL.md` descreve quando a skill se aplica e quais passos seguir.

Use skills para rotinas que se repetem, como revisar código seguindo os padrões do projeto ou preparar uma documentação com um formato definido.

Assim como libs, você não precisa criar todas as suas Skills, na verdade, o mais comum é usar Skills da comunidade. 

**Exemplo prático:**
- Você deseja criar um protótipo para uma landing page de um Clube do Livro, com um design minimalista, filtrando bem o público alvo da página. Você pode usar skills que vão te ajudar com isso!
- Prompt(Sintaxe do Codex):
"Você é um Engenheiro de Software sênior, especializado em UI/UX, contratado para criar a landing page de um portal para um clube de leitura, o "ProdBooks". O site deverá apresentar a proposta do clube: reunir pessoas focadas em produtividade que desejam receber mensalmente livros de hábitos, filosofia, produtividade e business. O site deve manter um padrão minimalista, usando tons neutros e fontes moderno-minimalistas. Utilize $using-superpowers e seus derivados para planejar, porém, inclua no plano as seguintes recomendações: $taste-skill para evitar designs genéricos, $humanizer:humanizer para gerar textos naturais e $emil-design-eng para construir a direção de design."

- **Disclaimer:** cada uma das skills citadas neste exemplo será desenvolvida melhor no arquivo `materiais/skills/importadas/catalog.md`

## Context Engineering

*Context engineering* é o trabalho de escolher, organizar e atualizar as informações disponíveis ao modelo durante uma tarefa. O contexto pode incluir o pedido, instruções do projeto, arquivos relevantes, decisões anteriores e resultados de ferramentas.

Para uma tarefa de código, comece indicando o objetivo e os critérios de conclusão. Aponte os arquivos ou módulos relacionados e inclua restrições importantes, como compatibilidade ou convenções do projeto. Acrescente novas informações quando a investigação trouxer fatos úteis e retire o que ficou desatualizado ou não ajuda na tarefa.

Contexto claro ajuda o agente a tomar decisões alinhadas ao projeto. Contexto excessivo, irrelevante ou contraditório pode desviar a resposta.

**Exemplo de uso quase que obrigatório:**
- O arquivo `AGENTS.md`, presente em quase todo repositório construído com IA (exemplo de demonstração neste repositório!). Ele define o contexto do projeto para direcionar o agente, evitando a necessidade do modelo ler todo o projeto sempre que for trabalhar nele.
## Para consultar

- [Model Context Protocol: introdução](https://modelcontextprotocol.io/introduction)
- [Skills na documentação da OpenAI](https://developers.openai.com/plugins/concepts/skills)
- [Boas práticas de prompt engineering da OpenAI](https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-the-openai-api)
