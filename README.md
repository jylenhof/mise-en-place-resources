# mise-en-place-resources

## Project

[mise-en-place](https://github.com/jdx/mise)

## Documentation

[mise-en-place documentation](https://mise.jdx.dev)

## Comparison with other tools

[github ranking](https://github.com/jdx/mise-analytics)

## Plugins home

[mise-plugins](https://github.com/orgs/mise-plugins/repositories)

## Ecosystem and related projects

This page lists community tools and projects in the mise ecosystem.

These are external resources that complement mise or extend its capabilities.
They are are maintained independently by their respective authors.

### Shell completion

[mise-completions](https://github.com/alltuner/mise-completions-sync) provides community-maintained
completion definitions for mise tools across a wide range of shells.

### Community guides and tutorials

| Project | Description |
|---------|-------------|
| [Stéphane Robert's Blog](https://blog.stephane-robert.info/docs/outils/systeme/mise/) | A comprehensive guide and documentation for mise (French). |

### Plugin and tool backends

Mise backends install tools from various sources.
The projects below offer custom backends or plugin patterns for specific tools.

| Project | Description |
|---------|-------------|
| [mise-db](https://github.com/lcmen/mise-db) | A custom mise backend plugin that provides a local database engine through native binaries. |
| [mise-gib](https://github.com/jbadeau/mise-gib) | Mise plugin for Gib. |
| [mise-git](https://github.com/lrntgr/mise-git) | Installs git via mise. |
| [mise-ghcup](https://github.com/wasp-lang/mise-ghcup) | Installs Haskell tools through GHCup via a mise backend plugin. |
| [mise-gno](https://github.com/junghoon-vans/mise-gno) | Installs and pins Gno CLI tools via a mise backend plugin. |
| [mise-krew](https://github.com/soupglasses/mise-krew) | Installs krew, the kubectl plugin manager, via mise. |
| [mise-nix](https://github.com/jbadeau/mise-nix) | Nix integration for mise. |
| [mise-oxc](https://github.com/malept/mise-oxc) | Installs the oxc JavaScript linter and formatter via mise. |
| [mise-shdoc](https://github.com/shunk031/mise-shdoc) | Installs `shdoc` documentation tooling via mise for shell script documentation generation. |
| [mise-php](https://github.com/verzly/mise-php) | Installs PHP via mise. |
| [mise-static-php](https://github.com/joshuarosato/mise-static-php) | Installs precompiled StaticPHP CLI and FPM binaries via mise. |
| [mise-postgres-binary](https://github.com/KyleKing/mise-postgres-binary) | Installs PostgreSQL binaries via mise. |
| [mise-mariadb](https://github.com/verzly/mise-mariadb) | MariaDB version manager plugin for mise. |
| [mise-selene](https://github.com/quentin-rodriguez/mise-selene) | Installs the Selene Lua static analyzer via mise. |
| [mise-expert](https://github.com/quentin-rodriguez/mise-expert) | Installs Expert, the Elixir language server, via mise. |
| [mise-uvtool](https://github.com/michaelprowacki/mise-uvtool) | Installs Python tools via `uv`. Credentials are currently hardcoded; keyring support is not implemented. A patch or fork adding keyring integration is worth investigating. |
| [mise-vite-plus](https://github.com/markmals/mise-vite-plus) | Integrates the Vite+ unified web development toolchain with mise. |
| [mise-ovhcloud-cli](https://github.com/pAkalpa/mise-ovhcloud-cli) | Provides an OVHcloud CLI backend for mise, enabling OVHcloud-specific tooling installs and configuration. |
| [mise-cf-terraforming](https://github.com/pAkalpa/mise-cf-terraforming) | Cloudflare Terraforming plugin for mise to terraform existing Cloudflare resources. |
| [poissonnier](https://github.com/dljsjr/poissonnier) | A mise plugin focused on Rust toolchain management. |
| [vfox-mongod](https://github.com/echocat/vfox-mongod) | Installs MongoDB using the vfox backend for mise. |
| [zim-mise](https://github.com/joke/zim-mise) | Integrates Zim wiki tooling with mise for documentation and note-taking workflows. |

> [!Note]
> `mise-uvtool` is particularly useful for scenarios like private PyPI support, as `mise` already provides a built-in solution for public packages via `uv tool` (using the `pipx` backend with `uvx=true`). While it currently lacks keyring integration, it offers a solid foundation, making it a worthwhile option to avoid starting from scratch.

### CI automation

| Project | Description |
|---------|-------------|
| [mise-update-tool](https://github.com/jylenhof/mise-update-tool) | A GitHub Action that upgrades tools from your local mise config with `mise upgrade --bump --local` and optionally opens pull requests when config files change. |
| [mise-action](https://github.com/jdx/mise-action) | Official mise GitHub Action for running mise tasks and workflows in CI. |
| [mise-buildkite-plugin](https://github.com/buildkite-plugins/mise-buildkite-plugin) | A Buildkite plugin for running mise tasks and workflows in Buildkite pipelines. |
| [workflows](https://github.com/lumirelle/workflows) | Reusable GitHub Actions workflows for mise-based CI, coverage, and release pipelines. |

### Git hooks

| Project | Description |
|---------|-------------|
| [pre-commit-mise-lock](https://github.com/lohn/pre-commit-mise-lock) | A pre-commit hook that keeps the mise lockfile (`mise.lock`) up to date automatically. |

### Dotfiles management

| Project | Description |
|---------|-------------|
| [mise-dotfiles-uninstall](https://github.com/veerendra2/mise-dotfiles-uninstall) | Safely unlinks TOML-configured dotfile symlinks created by mise until native uninstall support is available. |

### Secret and credential integrations

| Project | Description                                               |
|---------|------------------------------------------------------------------------------------------------------------|
| [mise-env-1password](https://github.com/kujenga/mise-env-1password) | Loads secrets from 1Password into the mise environment through the `[env]` section. |
| [mise-env-fnox](https://github.com/jdx/mise-env-fnox) | Loads secrets from fnox into the mise environment through the `[env]` section. |

### Editor Integrations

| Project | Description |
|---------|-------------|
| [miser.nvim](https://github.com/carldaws/miser.nvim) | Neovim plugin for mise. |
| [mise-vscode](https://github.com/hverlin/mise-vscode) | Visual Studio Code extension for mise. |

### Other jdx tools worth exploring

If you are already using mise, a few adjacent projects from jdx are also worth a look:

- [fnox](https://github.com/jdx/fnox) for encrypted and remote secret management across development, CI, and production
- [usage](https://github.com/jdx/usage) for CLI specification and documentation patterns
- [pitchfork](https://github.com/jdx/pitchfork) for managing project daemons with a strong developer-experience focus
- [communique](https://github.com/jdx/communique) for generating editorialized release notes from git history and pull requests.
- [Aube](https://github.com/jdx/aube) is a fast Node.js package manager.

They solve different problems, but they share the same focus on practical developer experience and can fit naturally into task-driven repositories.

> [!Note]
> [hk](https://github.com/jdx/hk) is interesting and fast, but if your main goal is to replace `pre-commit`, [prek](https://github.com/j178/prek) deserves stronger consideration. Its biggest practical advantage is compatibility with existing `pre-commit` setups, which lowers migration cost significantly. GitHub star counts also point to a stronger current adoption curve: `prek` is around 7k stars, while `hk` is around 700. That does not settle the technical comparison on its own, but combined with `pre-commit` compatibility it makes `prek` an easier recommendation for teams that want faster hook execution without rewriting their current hook definitions.

> [!Note]
> The lead maintainer of `mise` is now working full-time on these open source tools. Funding this product or subscribing to its services is the primary way to support the ongoing development and maintenance of the `mise` ecosystem.

> [!Note]
> **en.dev** is "The Developer Tooling Company," an enterprise dedicated to building the world's best developer tools for the next decade. It serves as the official home for `mise`, `aube`, `usage`, `pitchfork`, and `communique`. Supporting **en.dev** through sponsorships or product adoption ensures these high-performance open-source solutions remain sustainable, viable, and continuously improved.

### Task libraries and configuration patterns

| Project | Description |
|---------|-------------|
| [mise-cookbooks](https://github.com/hasansezertasan/mise-cookbooks) | Recipe-style configuration patterns and reusable task definitions for mise projects. |
| [tasks](https://github.com/seletz/tasks) | Example task library showing patterns for organizing mise task collections. |
| [mise-tasks](https://github.com/iwamot/mise-tasks) | A collection of predefined mise task templates and examples to streamline project automation. |
