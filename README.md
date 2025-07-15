# Coffee Machine ☕

Essential utilities to keep your development workflow percolating.

## Tools

### barista

Serves up AI in a dedicated tmux window.

**Usage:**
```bash
barista
```

Pulls a fresh shot of local AI in the `barista` session.

### bloom

Extracts the perfect development environment in a fresh tmux session.

**Usage:**
```bash
bloom [project_directory]
```

If no directory is specified, uses the current directory.

**Default Behavior:**

Without a config file, bloom opens a single `zsh` window. The `zsh` window is always created first.

**Configuration:**

Bloom uses YAML configuration files to define additional tools to open. Configuration priority:
1. Project config: `<project>/.bloom.yml` (highest priority)
2. Global config: `$XDG_CONFIG_HOME/bloom/config.yml` or `~/.config/bloom/config.yml`

**Requirements:**
- `tmux`
- `yq`

### cold-brew

Keeps your Homebrew fresh and potent.

**Usage:**
```bash
cold-brew
```

Maintains the blend:
- `brew update` - Update Homebrew
- `brew upgrade --greedy` - Upgrade all packages (including auto-update casks)
- `brew cleanup` - Remove old grounds
- `brew doctor` - Check the machine

## Installation

Tamp these scripts into your PATH:

```bash
./immersion
```
