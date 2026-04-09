# mise-en-place-resources

## Project

[mise-en-place](https://github.com/jdx/mise.git)

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

[mise-completions](https://mise-completions.alltuner.com/) provides community-maintained
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
| [micoo](https://github.com/hasansezertasan/micoo) | A collection of mise plugins for common development tools. |
| [mise-amber](https://github.com/devastion/mise-amber) | Installs the Amber programming language (compiles to Bash) via mise. |
| [mise-gib](https://github.com/jbadeau/mise-gib) | Mise plugin for Gib. |
| [mise-krew](https://github.com/soupglasses/mise-krew) | Installs krew, the kubectl plugin manager, via mise. |
| [mise-nix](https://github.com/jbadeau/mise-nix) | Nix integration for mise. |
| [mise-oxc](https://github.com/malept/mise-oxc) | Installs the oxc JavaScript linter and formatter via mise. |
| [mise-postgres-binary](https://github.com/KyleKing/mise-postgres-binary) | Installs PostgreSQL binaries via mise. |
| [mise-selene](https://github.com/quentin-rodriguez/mise-selene) | Installs the Selene Lua static analyzer via mise. |
| [mise-uvtool](https://github.com/michaelprowacki/mise-uvtool) | Installs Python tools via `uv`. Credentials are currently hardcoded; keyring support is not implemented. A patch or fork adding keyring integration is worth investigating. |
| [mise-vite-plus](https://github.com/markmals/mise-vite-plus) | Integrates the Vite+ unified web development toolchain with mise. |
| [poissonnier](https://github.com/dljsjr/poissonnier) | A mise plugin focused on Rust toolchain management. |
| [vfox-mongod](https://github.com/echocat/vfox-mongod) | Installs MongoDB using the vfox backend for mise. |

> [!Note]
> `mise-uvtool` is particularly useful for scenarios like private PyPI support, as `mise` already provides a built-in solution for public packages via `uv tool` (using the `pipx` backend with `uvx=true`). While it currently lacks keyring integration, it offers a solid foundation, making it a worthwhile option to avoid starting from scratch.

### Secret and credential integrations

| Project | Description                                               |
|---------|------------------------------------------------------------------------------------------------------------|
| [mise-env-1password](https://github.com/kujenga/mise-env-1password) | Loads secrets from 1Password into the mise environment through the `[env]` section. |
| [mise-env-fnox](https://github.com/jdx/mise-env-fnox) | Loads secrets from fnox into the mise environment through the `[env]` section. |

### Other jdx tools worth exploring

If you are already using mise, a few adjacent projects from jdx are also worth a look:

- [fnox](https://github.com/jdx/fnox) for encrypted and remote secret management across development, CI, and production
- [usage](https://github.com/jdx/usage) for CLI specification and documentation patterns
- [pitchfork](https://github.com/jdx/pitchfork) for managing project daemons with a strong developer-experience focus
- [communique](https://github.com/jdx/communique) for generating editorialized release notes from git history and pull requests.

They solve different problems, but they share the same focus on practical developer experience and can fit naturally into task-driven repositories.

> [!Note]
> [hk](https://github.com/jdx/hk) is interesting and fast, but if your main goal is to replace `pre-commit`, [prek](https://github.com/j178/prek) deserves stronger consideration. Its biggest practical advantage is compatibility with existing `pre-commit` setups, which lowers migration cost significantly. GitHub star counts also point to a stronger current adoption curve: `prek` is around 7k stars, while `hk` is around 700. That does not settle the technical comparison on its own, but combined with `pre-commit` compatibility it makes `prek` an easier recommendation for teams that want faster hook execution without rewriting their current hook definitions.

### Task libraries and configuration patterns

| Project | Description |
|---------|-------------|
| [mise-cookbooks](https://github.com/hasansezertasan/mise-cookbooks) | Recipe-style configuration patterns and reusable task definitions for mise projects. |
| [tasks](https://github.com/seletz/tasks) | Example task library showing patterns for organizing mise task collections. |
