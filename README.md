# Tesea MCP

Plugin oficial da Tesea para Claude, Cowork, Claude Code, ChatGPT Desktop, Codex e Hermes Agent.

## ChatGPT Desktop e Codex

No ChatGPT Desktop, abra **Settings → Plugins**, adicione o marketplace customizado:

```text
https://github.com/Tesea-AI/tesea-mcp
```

Depois, instale o plugin **Tesea**. Na tela de conexão, escolha uma das opções:

- entrar com sua conta Tesea via OAuth;
- colar uma chave de API Tesea ativa.

A chave é usada somente para autorizar a conexão. O ChatGPT recebe tokens OAuth
com os mesmos escopos e restrições da chave original.

O mesmo fluxo pode ser iniciado pelo terminal:

```bash
codex plugin marketplace add Tesea-AI/tesea-mcp
codex plugin add tesea@tesea-ai
```

## Claude (claude.ai, Desktop e Cowork)

Abra **Customize → Plugins → Add marketplace** e informe:

```text
Tesea-AI/tesea-mcp
```

Depois, instale o plugin **Tesea**, abra a aba **Connectors** do plugin e
conecte sua conta Tesea.

Para adicionar somente o conector, abra
[este link](https://claude.ai/customize/connectors?modal=add-custom-connector&connectorName=Tesea&connectorUrl=https%3A%2F%2Fapi.tesea.com.br%2Fmcp),
escolha **Registrar automaticamente** como cliente OAuth e clique em
**Continuar**. Nos planos Team e Enterprise, o Owner adiciona o conector ou o
marketplace para a organização.

## Claude Code

```bash
claude plugin marketplace add Tesea-AI/tesea-mcp
claude plugin install tesea@tesea-ai
```

Depois de instalar, use `/mcp` para conectar sua conta Tesea.

## Hermes Agent

```bash
hermes mcp add tesea --url https://api.tesea.com.br/mcp --auth oauth
hermes mcp login tesea
hermes mcp test tesea
```

Depois de executar os comandos, siga as instruções para conectar sua conta.

## Licença

[MIT](LICENSE)
