# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Structure

Dotfiles organized by tool with each in its own subdirectory:
- `claude/.claude/CLAUDE.md` - User's global Claude Code instructions
- `git/.gitconfig` - Git config with aliases, pull.rebase, push.autoSetupRemote
- `starship/.config/starship.toml` - Starship prompt (Gruvbox Dark theme)
- `ghostty/.config/ghostty/config` - Ghostty terminal config
- `npm/.npmrc` - npm config with save-exact, engine-strict, audit settings
- `zsh/.zshrc` - Zsh shell config (currently empty)

## Git Configuration

### Credential Helpers
Uses multiple helpers - git tries each until one succeeds:
- macOS: osxkeychain (built-in)
- Arch Linux: libsecret (requires `git-credential-libsecret` package)

### Aliases
- `stashpull` - Stash changes, pull, pop stash
- `fix` - Shorthand for `commit --fixup`
- `fere` - Fetch + interactive rebase with autosquash on origin branch
- `recent` - Show 5 most recent branches

## Installation

No automated setup script exists. Symlink configs manually to home directory.
