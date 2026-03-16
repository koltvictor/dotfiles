# dotfiles

My personal development environment configuration. Optimized for full-stack TypeScript/Node.js development on macOS.

---

## Contents

| File | Description |
| ---- | ----------- |
| `.zshrc` | Shell aliases, functions, and environment setup |
| `.gitconfig` | Git aliases, defaults, and editor config |

---

## Highlights

### Shell Functions

**`killport <port>`** — Kill whatever process is holding a port hostage.
```bash
killport 3001
```

**`whatsport <port>`** — See what's running on a port before killing it.
```bash
whatsport 3000
```

**`mkcd <dir>`** — Create a directory and cd into it in one step.
```bash
mkcd my-new-project
```

**`gcm "<message>"`** — Stage everything and commit in one command.
```bash
gcm "fix: resolve auth token expiry"
```

**`ghopen`** — Open the current repo on GitHub in your browser.
```bash
ghopen
```

---

### Git Aliases

```bash
git lg          # Visual branch graph (oneline, decorated)
git undo        # Undo last commit, keep changes staged
git staged      # Diff of what's staged
git contributors # Ranked list of contributors by commit count
```

---

## Installation

```bash
# Clone
git clone git@github.com:koltvictor/dotfiles.git ~/dotfiles
cd ~/dotfiles

# Symlink (or copy) to home directory
ln -sf ~/dotfiles/.zshrc ~/.zshrc
ln -sf ~/dotfiles/.gitconfig ~/.gitconfig

# Reload shell
source ~/.zshrc
```

---

## Philosophy

A development environment should be invisible — fast enough, quiet enough, and opinionated enough that you stop thinking about it and start thinking about the problem.
