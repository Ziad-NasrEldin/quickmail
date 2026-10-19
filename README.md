# Quickinbox

Self-hosted mail for a domain you already own — a real web inbox, no third-party mailbox.

## Who it's for

Founders, small teams, and anyone who'd rather run mail themselves than rent an inbox. You bring a domain and a Cloudflare account; Quickinbox is the client you actually use day to day.

## What you can do

- Read and send mail from a full web client on a domain you control
- Follow replies as threads, with quoted history tucked out of the way
- Attach files that stay in storage you own, inbound and outbound
- Give each person their own addresses, plus a catch-all for everything else
- Send and read the same mail from the terminal, a REST API, or an AI agent

## Try it

There isn't a public hosted demo — you run your own instance. The setup wizard is the fastest path:

```bash
bun run setup
# if bun isn't installed yet:
bash scripts/setup.sh
```

Full walkthrough — DNS, providers, first account, API, and CLI — is in [docs/SETUP.md](docs/SETUP.md).

## How it works

Mail hits a Cloudflare Worker the moment it arrives. Conversations live in D1, attachments in R2, and you read them in the browser. Pick Cloudflare Email or Resend as the provider — one per install. The same Worker sends mail back out.

---

Built by [Ziad Ahmed](https://github.com/Ziad-NasrEldin) at [MaVoid](https://mavoid.com).

[Website](https://mavoid.com) · [LinkedIn](https://linkedin.com/in/ziad-ahmed-634202332) · [GitHub](https://github.com/Ziad-NasrEldin)
