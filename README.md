## Cauê Franco

**AI Full Stack Engineer.** Construo agentes de LLM e o produto inteiro em volta deles: back-end, interface, integrações e deploy. Hoje na **GeniAI**.

📍 João Pessoa - PB · Análise e Desenvolvimento de Sistemas

### Como eu construo com LLM

- **O modelo interpreta, o código decide.** Saída em JSON validado por schema; fluxo e efeitos colaterais ficam em código testável.
- **Grounding.** O agente responde só com a base aprovada; o resto vai para uma pessoa.
- **Falha previsível.** Timeout ou resposta inválida têm uma nova tentativa e depois caem num caminho seguro.
- **Eval antes de trocar de modelo.** Acerto e latência medidos em cada candidato.

### Projetos

**[Agente de suporte no WhatsApp](https://github.com/cauedev30/chatbot-atendimento-geniai)** `código aberto`\
Agente LLM como bot do Chatwoot: identifica o cliente, abre o ticket, responde pelo FAQ com grounding, transcreve áudio, lê imagem e transfere para humano. Kanban e indicadores para a equipe. A triagem, que era manual, passou a ser 100% automática. Arquitetura em camadas com portas e adaptadores, outbox, eval próprio e 785 testes.\
`Python` `FastAPI` `PostgreSQL` `Next.js` `Pytest` `Playwright`

**Automação de provisionamento no Chatwoot** `código fechado`\
Uma automação idempotente e parametrizada que cria usuário, times, regras e inboxes em cerca de 20 contas de uma rede de franquias de saúde. Confere banco e Chatwoot antes de escrever e para em vez de gravar pela metade.\
`n8n` `Python` `Supabase` `API do Chatwoot`

**Site de pedidos para restaurante no edge** `código fechado` `freelance`\
Cardápio digital com sacola que fecha o pedido no WhatsApp, e painel com senha para a dona abrir o dia e desligar item esgotado.\
`Next.js` `Cloudflare Workers` `Workers KV` `Vitest`

**Plataforma de governança de contratos** `código fechado` `produto interno`\
Gestão de contratos de aluguel com extração de dados via LLM, RLS e TDD. Encontrei e corrigi uma falha de autorização (IDOR) no próprio código, com testes de regressão.\
`Next.js` `TypeScript` `Supabase` `Vitest`

### Engenharia assistida por IA

Claude Code com skills e hooks por projeto, contexto versionado (estado, decisões e specs), MCP servers e aprovação humana antes de qualquer ação irreversível. Toda feature nasce com critério de aceite executável e só fecha quando ele roda verde.

### Stack

**IA aplicada:** LLMs · RAG · embeddings e bancos vetoriais · agentes e multiagentes · function calling · MCP · context engineering · evals · n8n\
**Full stack:** Python · FastAPI · TypeScript · Node.js · React · Next.js · PostgreSQL/Supabase · Docker · Cloudflare Workers · GitHub Actions · Pytest · Vitest · Playwright

### Outros repositórios

[Projeto-FullStack-ReNTAI](https://github.com/cauedev30/Projeto-FullStack-ReNTAI) · [Gerenciador-de-estoque-padaria](https://github.com/cauedev30/Gerenciador-de-estoque-padaria) · [projeto-movie-manager](https://github.com/cauedev30/projeto-movie-manager) · [portfolio](https://cauedev30.github.io/portfolio-caue-franco/)

### Contato

[LinkedIn](https://www.linkedin.com/in/cauefranco01/) · cauefranco01@gmail.com
