# <picture><source media="(prefers-color-scheme: dark)" srcset="docs/leverage-dark.svg"><img src="docs/leverage-light.svg" alt="Leverage Computer" height="24"></picture> OpenCode on Leverage

<a href="https://leverage.computer/integrations/#opencode"><img src="https://img.shields.io/badge/Docs-leverage.computer-3f3f46?labelColor=0a0a0a" alt="Docs on leverage.computer"></a>
<a href="#features"><img src="https://img.shields.io/badge/Connects%20over-HTTP-3f3f46?labelColor=0a0a0a" alt="Connects over HTTP"></a>
<a href="#desktop"><img src="https://img.shields.io/badge/OpenCode%20Desktop-%E2%89%A52.0.15-3f3f46?labelColor=0a0a0a" alt="OpenCode Desktop 2.0.15 or later"></a>

[Features](#features) · [Desktop](#desktop) · [Terminal](#terminal) ·
[Other clients](#other-opencode-clients) · [leverage.computer](https://leverage.computer)

[![Syncing a Leverage workspace into OpenCode Desktop from the Leverage desktop app, then opening a session](docs/desktop.gif)](docs/desktop.mp4)

## Features

- **Multiplayer harness**: each prompt shows who sent it, and a teammate's
  prompt appears as soon as they send it.
- **Company computer**: sessions run in Leverage's sandbox and are shared with
  your team. Leverage serves OpenCode's HTTP API, so nothing runs on your
  machine.
- **Steering**: your prompt shows at once and steers a running turn. Prompts
  sent while it is busy wait in a queue you can list, take back or send now.
- **Governance**: the agent asks you to pick an option, approve a plan, or
  allow a call: once, for the session, or always.

Each space shows as a folder.

## Desktop

In the Leverage desktop app, open Settings → Developer tools and click
**Sync into OpenCode**. If OpenCode is open, it closes and opens again with the
workspace.

From a terminal instead:

```sh
leverage opencode setup
```

Mac only, OpenCode Desktop 2.0.15 or later. Sync again after you change spaces
in Settings. OpenCode Desktop holds one workspace at a time.

## Terminal

```sh
leverage opencode engineering
```

With no space, it opens the whole workspace.

[![A terminal runs leverage opencode general. OpenCode opens on the space, /sessions finds a session, and it opens with a teammate's messages and the agent's diff](docs/terminal.gif)](docs/terminal.mp4)

## Other OpenCode clients

Make a token in Settings → Developer tools → OpenCode, then connect with:

- Server: `https://app.leverage.computer/api/opencode[/<space>]`
- Password: your token

## The Leverage CLI

The terminal commands need the Leverage CLI. In the Leverage app, Settings →
Developer tools → CLI gives its install command, for macOS and Linux.

A session you start from OpenCode is private until you share it.
