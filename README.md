# n

Minimalist utility for quick plain-text notes.

## Behavior

Running `n` opens a lightweight input dialog. Typing text and pressing Enter saves the input as a timestamped `.txt` file in `~/Documents/notes` (or `$NOTES_DIR` if set) and closes the window immediately.

## Installation

### NixOS / Nix (Flakes)

Run directly without installation:

```bash
nix run github:nepoet1/n-note
```

Install into user profile:

```bash
nix profile install github:nepoet1/n-note
```

### Arch Linux

Install with a single command:

```bash
git clone https://github.com/nepoet1/n-note.git /tmp/n-note && cd /tmp/n-note && makepkg -si --noconfirm && cd - && rm -rf /tmp/n-note
```

## Configuration

By default, notes are saved to `~/Documents/notes`. To change the directory, export the `NOTES_DIR` environment variable in your shell configuration:

```bash
export NOTES_DIR="$HOME/notes"
```
