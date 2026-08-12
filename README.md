# Colossus Homebrew Tap

This is the official Homebrew tap for
[Colossus](https://github.com/obscuritylabs/Colossus), an auditable runtime for
agent work and durable automation.

## Install

Install the latest stable release directly from the tap:

```bash
brew install obscuritylabs/tap/colossus
colossus --version
```

Homebrew owns installations made through this tap. Upgrade or remove Colossus
through Homebrew:

```bash
brew upgrade obscuritylabs/tap/colossus
brew uninstall obscuritylabs/tap/colossus
```

`colossus update` detects the Homebrew ownership marker and will not replace the
managed executable.

## Supported systems

The formula supports Apple Silicon and Intel macOS. It downloads the immutable
native archive from the corresponding Colossus GitHub Release and verifies the
archive against its pinned SHA-256 digest before installation.

## Maintenance

The reviewed formula source is maintained in the
[Colossus repository](https://github.com/obscuritylabs/Colossus/blob/main/packaging/homebrew/Formula/colossus.rb)
and mirrored here only after the release assets and anonymous public-install flow
have passed validation. Formula changes in this tap must pass installation tests
on standard Apple Silicon and Intel GitHub-hosted runners.
