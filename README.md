# PromptGuard Scan MCP

PromptGuard Scan MCP is a paid remote Model Context Protocol server for LLM security testing. It helps teams inspect AI apps for prompt injection, jailbreaks, hidden instruction leakage, unsafe tool-use signals, and release-gate risk.

This repository is the public MCP integration and directory listing package for the hosted service at [promptguardscan.space](https://promptguardscan.space/?utm_source=github&utm_medium=repository&utm_campaign=sbl202605). The production MCP endpoint is hosted remotely; the product source code is not published here.

## MCP endpoint

- Remote MCP URL: `https://promptguardscan.space/mcp`
- Transport: Streamable HTTP
- Authentication: `Authorization: Bearer <token>`
- Server card: [/.well-known/mcp/server-card.json](https://promptguardscan.space/.well-known/mcp/server-card.json?utm_source=github&utm_medium=repository&utm_campaign=sbl202605)
- Website: [PromptGuard Scan](https://promptguardscan.space/?utm_source=github&utm_medium=repository&utm_campaign=sbl202605)
- Pricing: [PromptGuard Scan pricing](https://promptguardscan.space/pricing/?utm_source=github&utm_medium=repository&utm_campaign=sbl202605)

Tokens are issued after checkout and MCP token claim. Do not paste access tokens into public issues, prompts, screenshots, logs, or pull requests.

## Connect

Use your issued Bearer token in an MCP client that supports remote Streamable HTTP servers.

```json
{
  "mcpServers": {
    "promptguardscan": {
      "type": "http",
      "url": "https://promptguardscan.space/mcp",
      "headers": {
        "Authorization": "Bearer <token>"
      }
    }
  }
}
```

## What it is for

- Prompt injection scanner workflows for AI apps, chatbots, agents, RAG systems, and custom GPT-style tools.
- Jailbreak detection and prompt security regression testing before release.
- LLM vulnerability scanner evidence for engineering teams and buyer security reviews.
- CI/CD release-gate context for high-risk prompt, retrieval, and tool-use changes.

## Public directory records

- Official MCP Registry name: `space.promptguardscan/promptguardscan-mcp`
- Smithery qualified name: `clauxel/prompt-injection-scanner-mcp`
- Primary website: [https://promptguardscan.space/](https://promptguardscan.space/?utm_source=github&utm_medium=repository&utm_campaign=sbl202605)

## Related security guides

- [Prompt Injection Scanner for LLM Apps](https://promptguardscan.space/prompt-injection-scanner/?utm_source=github&utm_medium=repository&utm_campaign=sbl202605)
- [LLM Security Testing Tool for Release Gates](https://promptguardscan.space/llm-security-testing-tool/?utm_source=github&utm_medium=repository&utm_campaign=sbl202605)
- [AI App Security Audit Checklist](https://promptguardscan.space/ai-app-security-audit/?utm_source=github&utm_medium=repository&utm_campaign=sbl202605)
- [Jailbreak Detection API for AI Products](https://promptguardscan.space/jailbreak-detection-api/?utm_source=github&utm_medium=repository&utm_campaign=sbl202605)

## Support

For account, checkout, token, or security-report questions, contact [support@aigeamy.com](mailto:support@aigeamy.com).
