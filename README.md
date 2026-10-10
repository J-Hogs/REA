# REA

Workspace for using [REA (Reverse Engineer Anything)](https://github.com/morluto/rea)
from Claude Code cloud sessions, including from the Claude iPhone app.

## How it works

`.mcp.json` registers REA's MCP server (`npx -y rea-agents@6.3.0 mcp`), so a
Claude Code session started with this repository can use REA's tools. The first
time, Claude Code asks you to approve the `rea` server.

## Usage

1. Start a Claude Code cloud session with this repository selected.
2. Approve the `rea` MCP server if prompted.
3. Ask, for example: "Use REA to analyse the JavaScript app at <link>."

Static JavaScript/Electron analysis works without extra software. Native binary
analysis needs Ghidra, Hopper or IDA, which are not installed by default.

## Updating

Change the version in `.mcp.json` to the latest
[`rea-agents` release](https://www.npmjs.com/package/rea-agents).
