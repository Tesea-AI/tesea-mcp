# Tesea MCP

Conector oficial para usar a Tesea em clientes compatíveis com o
[Model Context Protocol](https://modelcontextprotocol.io/).

O servidor MCP é remoto, usa OAuth 2.1 com PKCE e não exige instalar código
local. A API key da Tesea é informada somente na página de autorização da
Tesea e não deve ser colocada neste repositório nem na configuração do cliente.

## Claude Code

```bash
claude plugin marketplace add Tesea-AI/tesea-mcp
claude plugin install tesea@tesea-ai
```

Abra `/mcp` no Claude Code e conclua a autenticação no navegador.

## Hermes Agent

```bash
hermes mcp add tesea --url https://api.tesea.com.br/mcp --auth oauth
hermes mcp login tesea
hermes mcp test tesea
```

O arquivo [`hermes/manifest.yaml`](hermes/manifest.yaml) está pronto para uma
futura submissão ao catálogo oficial do Hermes. Até sua aprovação upstream, o
comando `hermes mcp add` acima é o instalador suportado.

## Endpoint

```text
https://api.tesea.com.br/mcp
```

O MCP é um cliente fino da API privada da Tesea. Ele não expõe acesso ao
navegador, Docker, sessões ou URLs internas.

## Licença

[MIT](LICENSE)
