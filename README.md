# Mission MCP

Mission MCP is a Trust Graduation gate for AI agents. It gives Claude and other MCP clients a visible approval ceremony before consequential actions such as sending email, posting publicly, scheduling, spending money, publishing artifacts, or modifying external records.

This repository is a small runnable public wrapper around the published `@gomission/mcp` npm package so MCP directories and evaluators can start the stdio server directly.

## Run

```sh
npm install
npm start
```

The server speaks MCP over newline-delimited JSON-RPC on stdio.

## Tools

- `mission_status`
- `request_approval`
- `log_action`
- `get_receipt`
- `mission_ask`

## Docker

```sh
docker build -t gomission-mcp .
docker run -i gomission-mcp
```

Learn more: https://claude.gomission.io
