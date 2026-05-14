# scry-marketplace

Self-hosted [Claude Code](https://code.claude.com) plugin marketplace for [scry](https://github.com/K-alt-123/scry).

## Install

```text
claude plugin marketplace add https://github.com/K-alt-123/scry-marketplace --scope user
claude plugin install scry@scry-marketplace --scope user
```

To get a newer pinned version after this marketplace is updated:

```text
claude plugin marketplace update scry-marketplace
claude plugin update scry@scry-marketplace
```

## What this repo is

A pointer file. The catalog at [.claude-plugin/marketplace.json](.claude-plugin/marketplace.json) tells Claude Code where the scry plugin source lives and which commit SHA to install.

The scry plugin code lives in a separate repo: <https://github.com/K-alt-123/scry>.

## Versioning

Each scry release bumps the `sha` field in `marketplace.json` to a tested commit. Users only receive updates when this file changes.

## License

MIT
