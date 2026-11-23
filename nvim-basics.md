# Neovim Basics — a gentle start

If the video [`nvim-video-share.md`](./nvim-video-share.md) felt overwhelming, start here.
It assumes you already know how to move around in Neovim. This guide fills that gap.

## 1. What is Neovim?

Neovim is a text editor that runs in your terminal. It is fast, keyboard-driven, and
highly customizable. You do not need to be a programmer to start; you just need patience
for a new way of typing.

## 2. Install

- macOS: `brew install neovim`
- Linux (Debian/Ubuntu): `sudo apt install neovim`
- Windows: download from https://neovim.io or use `winget install Neovim.Neovim`

Check it works: open a terminal and run `nvim`. You should see a welcome screen.
Quit with `:q` then `Enter`.

## 3. The one idea that matters: modes

Neovim has modes. The most important two:

- **Normal mode** — you are here when Neovim opens. Keys are *commands*, not text.
  Press `Esc` anytime to return here. When in doubt, press `Esc`.
- **Insert mode** — where you type text. Enter it with `i` (insert before cursor),
  `a` (after cursor), `o` (new line below). Leave with `Esc`.

Other modes (Visual for selecting, Command for `:` commands) come later.

## 4. Moving around (Normal mode)

Forget the mouse. Use these:

| Key | Move |
|-----|------|
| `h` `j` `k` `l` | left / down / up / right |
| `w` / `b` | next / previous word |
| `0` / `$` | start / end of line |
| `gg` / `G` | top / bottom of file |
| `Ctrl-d` / `Ctrl-u` | half page down / up |

Tip: hold a number before a move to repeat it — `5j` moves down 5 lines.

## 5. Editing (Normal mode)

| Key | Action |
|-----|--------|
| `i` / `a` | insert before / after cursor |
| `o` / `O` | new line below / above |
| `x` | delete character |
| `dd` | delete whole line |
| `yy` | copy (yank) line |
| `p` | paste below |
| `u` | undo |
| `Ctrl-r` | redo |
| `ciw` | change inner word (delete word and type new) |

## 6. Saving and quitting (Command mode)

Press `:` to enter Command mode, type, then `Enter`:

| Command | Meaning |
|---------|---------|
| `:w` | save (write) |
| `:q` | quit |
| `:wq` | save and quit |
| `:q!` | quit without saving (discard changes) |
| `:e filename` | open a file |

## 7. Your first config

Neovim reads `~/.config/nvim/init.lua` (create the folder if missing).

Minimal starter:

```lua
-- ~/.config/nvim/init.lua
vim.opt.number = true          -- show line numbers
vim.opt.relativenumber = true  -- relative line numbers (great for jumps)
vim.opt.tabstop = 2            -- tab width
vim.opt.shiftwidth = 2
vim.opt.expandtab = true       -- spaces instead of tabs
vim.opt.wrap = false           -- no line wrapping
vim.g.mapleader = " "         -- Space as leader key
```

Restart Neovim after editing. If something breaks, the error message tells you the line.

## 8. Plugins (the short version)

Plugins are add-ons. You usually install a plugin manager (like `lazy.nvim`) and list
plugins in a `plugins/` folder. The video uses this approach. Do not copy the whole
config at once — add one plugin, restart, test, then add the next.

## 9. A 10-minute practice routine

1. Open `nvim practice.txt`.
2. Type a few lines in Insert mode, `Esc` back to Normal.
3. Move with `hjkl`, delete a line with `dd`, undo with `u`.
4. Save with `:w`, quit with `:q`.
5. Reopen and confirm your text is there.

Repeat daily for a week. Speed comes from repetition, not memorization.

## 10. When you are stuck

- Press `Esc` — it fixes most confusion.
- `:help <topic>` opens built-in help, e.g. `:help motion`.
- Search "neovim beginner" — many free guides exist.
- Keep the [`glossary.md`](./glossary.md) open for unknown words.

## Where to go next

- Read [`glossary.md`](./glossary.md) for terms used in the video.
- Watch the video once without copying — just observe the flow.
- On a second watch, recreate one small piece at a time.

*You do not need to understand everything on day one. Neovim rewards slow, steady use.*