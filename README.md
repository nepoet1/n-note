# n

Minimalist utility for quick plain-text notes.

## Behavior

Running `n` opens a lightweight input dialog. Typing text and pressing Enter saves the input as a timestamped `.txt` file in `~/Documents/notes` (or `$NOTES_DIR` if set) and closes the window immediately.

## Installation

### NixOS / Nix

Run directly without installation:

```sh
nix --extra-experimental-features "nix-command flakes" run github:nepoet1/n-note
```

Install into user profile:

```sh
nix --extra-experimental-features "nix-command flakes" profile add github:nepoet1/n-note
```

### Arch Linux

Install with a single command:

```sh
git clone https://github.com/nepoet1/n-note.git /tmp/n-note && cd /tmp/n-note && makepkg -si --noconfirm && cd - && rm -rf /tmp/n-note
```

## Configuration

By default, notes are saved to `~/Documents/notes`. To change the directory, set the `NOTES_DIR` environment variable.

Bash / Zsh:

```sh
export NOTES_DIR="$HOME/notes"
```

Fish:

```fish
set -Ux NOTES_DIR "$HOME/notes"
```
