# Bugnet

**Disposable cloud sandboxes for AI coding agents.** Pay per run, no account.

Your coding agent notices when work should not run on your machine: a repo someone sent you, a
local AI model, a tool that needs Linux or a GPU, an experiment that might break things. It offers
to run it in a throwaway Linux sandbox instead, tells you the price, and starts it once you agree.
When the sandbox ends, everything in it is deleted.

- **Checks first, for free.** A rule-based look at the repo, model or script before anything runs.
- **Pays per run.** USDC on Solana, from your own wallet or a pay link. No sign-up, no API key.
- **Pay-per-call APIs inside.** Code in the sandbox can use x402 APIs without a key. Bugnet pays
  them from a capped allowance, outside the sandbox.
- **A summary of every run.** Commands, payments and logs on a private page for 48 hours.

Bugnet speaks [MCP](https://modelcontextprotocol.io), so it works with Claude Code and other MCP
clients:

```sh
claude mcp add --scope user --transport http bugnet https://mcp.bugnet.sh/mcp
```

## Repositories

| | |
|---|---|
| [bugnet](https://github.com/bugnet-sh/bugnet) | The MCP server and the local bridge, with setup for every client |
| [website](https://github.com/bugnet-sh/website) | [bugnet.sh](https://bugnet.sh) |

## Contact

Questions and abuse reports: [support@bugnet.org](mailto:support@bugnet.org). Security issues:
follow [SECURITY.md](https://github.com/bugnet-sh/bugnet/blob/main/SECURITY.md).
