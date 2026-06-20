# Mission MCP

Mission MCP is governed execution infrastructure for AI agents. It creates visible approval ceremonies, receipt-backed audit trails, and trust boundaries before consequential actions such as sending email, posting publicly, scheduling, spending money, publishing artifacts, or modifying external records.

This repository is a lightweight public wrapper around the published `@gomission/mcp` package so MCP directories, evaluators, and local clients can start the stdio server directly.

## Run

```sh
npm install
npm start
```

The server speaks MCP over newline-delimited JSON-RPC on stdio and exposes Mission's five approval and receipt primitives for governed agent execution.

## Tools

- `mission_status`
- `request_approval`
- `log_action`
- `get_receipt`
- `mission_ask`

## Why it exists

Most agent governance servers focus on policy, risk, or review layers in the abstract. Mission focuses on governed execution: agents can do real work, but consequential actions are held behind visible approval ceremonies and receipt-backed boundaries until a principal decides otherwise.

## Docker

```sh
docker build -t gomission-mcp .
docker run -i gomission-mcp
```

Learn more: https://claude.gomission.io
