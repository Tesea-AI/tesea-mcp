# Tesea MCP

Conector oficial da Tesea para Claude Code, Codex e Hermes Agent.

## Claude Code

```bash
claude plugin marketplace add Tesea-AI/tesea-mcp
claude plugin install tesea@tesea-ai
```

Depois de instalar, use `/mcp` para conectar sua conta Tesea.

## Codex

```bash
codex mcp add tesea --url https://api.tesea.com.br/mcp
codex mcp login tesea
codex mcp list
```

Depois de executar os comandos, use `/mcp` para confirmar a conexão.

## Hermes Agent

```bash
hermes mcp add tesea --url https://api.tesea.com.br/mcp --auth oauth
hermes mcp login tesea
hermes mcp test tesea
```

Depois de executar os comandos, siga as instruções para conectar sua conta.

## Licença

[MIT](LICENSE)
