## Cauê Franco

**Desenvolvedor backend e automação.** Integro sistemas e IA para reduzir custo e tempo operacional.

Atualmente na **GeniAI**, onde desenvolvo dashboards e automações em n8n integradas ao Chatwoot e às APIs oficiais da Meta. Experiência real com APIs RESTful, arquitetura RAG, Clean Architecture e pipelines de IA — orquestrando LLMs e integrando serviços para eliminar tarefas manuais e acelerar processos em produção.

Vejo software como produto: soluções escaláveis e confiáveis, que reduzem custo, ganham tempo e geram valor real para o negócio.

📍 João Pessoa - PB · Análise e Desenvolvimento de Sistemas

---

### Stack

**Linguagens:** Python · TypeScript
**Automação e IA:** n8n · orquestração de LLMs · RAG · APIs RESTful
**Web:** Next.js · React
**Dados e infra:** PostgreSQL · Supabase · Docker · Dokku

---

### Em produção

Os dois projetos abaixo estão em uso real e têm **código fechado** — são sistemas de cliente ou produto interno. Descrevo o problema e a solução; o código não é público.

#### Automação de provisionamento — Chatwoot + n8n `código fechado`

**O problema.** Cada atendente novo em uma unidade exigia criar à mão cinco artefatos encadeados no Chatwoot — usuário, time pessoal, regra de automação, label e vínculo de inbox. Feito manualmente, repetido a cada contratação, em dezenas de contas. Lento, sujeito a erro e sem rastro de quem mudou o quê.

**O que construí.** Workflows n8n que executam o provisionamento ponta a ponta pela API do Chatwoot, com uma trava de duas fontes: o cadastro no banco e o estado real no Chatwoot precisam concordar antes de qualquer escrita, e qualquer divergência aborta a execução em vez de gravar pela metade. A remoção segue o caminho inverso, com a ordem das exclusões pensada para que nada fique órfão.

**Por que é a mesma automação para todos.** Roda hoje em **~20 contas de cliente** de uma rede de franquias de saúde. Não são vinte automações: é uma só, parametrizada por unidade. Cada conta tem convenção própria de nomes, times e regras, e generalizar isso sem duplicar lógica foi o trabalho de engenharia real do projeto.

**Stack:** n8n · Python · API REST do Chatwoot · PostgreSQL/Supabase

#### Plataforma de governança de contratos `código fechado` `produto interno`

**O que é.** Sistema de gestão de contratos de aluguel: cadastro, carteira, reajustes, anexos e extração automática de dados do contrato via LLM. Produto interno, sem cliente externo ainda.

**O que fiz.** Features entregues por TDD sobre uma base Next.js/Supabase com isolamento por RLS e arquitetura em camadas — domínio separado da camada de dados e da apresentação. A suíte foi de 75 para 82 testes no período.

**O achado que mais importa.** Numa auditoria do próprio código encontrei uma falha de autorização: uma rota de download de documento usava o cliente administrativo do banco — que ignora RLS por definição — e verificava apenas se o usuário estava autenticado, nunca se aquele documento era dele. Na prática, trocar um identificador na URL entregava o contrato de outra pessoa. Corrigi e escrevi quatro testes de regressão para a falha.

**Stack:** Next.js · TypeScript · Supabase/PostgreSQL com RLS · Vitest · pdf-lib

---

### Código aberto

| Projeto | Sobre |
|---|---|
| [Projeto-FullStack-ReNTAI](https://github.com/cauedev30/Projeto-FullStack-ReNTAI) | Teleconsultoria fullstack em TypeScript — API, validação de documentos, notificação em tempo real, E2E com Playwright |
| [ilovebkn-site](https://github.com/cauedev30/ilovebkn-site) | Site institucional em Next.js com TypeScript e Tailwind |
| [Gerenciador-de-estoque-padaria](https://github.com/cauedev30/Gerenciador-de-estoque-padaria) | Gerenciador de estoque em Python |
| [projeto-movie-manager](https://github.com/cauedev30/projeto-movie-manager) | Catálogo de filmes em JavaScript |
| [portfolio-caue-franco](https://github.com/cauedev30/portfolio-caue-franco) | Portfólio pessoal — [no ar](https://cauedev30.github.io/portfolio-caue-franco/) |

---

### Contato

[LinkedIn](https://www.linkedin.com/in/cauefranco01/) · cauefranco01@gmail.com · [Portfólio](https://cauedev30.github.io/portfolio-caue-franco/)
