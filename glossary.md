# Glossary — Neovim & the video's vocabulary

A plain-language reference for terms used in
[`nvim-video-share.md`](./nvim-video-share.md) and in Neovim setups in general.
If a word here still feels fuzzy, that's normal — come back after watching the video once.

## Editor basics

- **Editor** — the program you type code into. Neovim is one.
- **Neovim (nvim)** — a modern, improved version of Vim. Free and open source.
- **Vim** — the older editor Neovim grew out of. Most Vim knowledge carries over.
- **Modal editing** — the idea that the editor has different "modes" (normal, insert, visual, …)
  and keys do different things in each. This is Vim/Neovim's defining feature.
- **Normal mode** — the default mode. Keys are commands, not text. Press `Esc` to get here.
- **Insert mode** — where you actually type text. Enter with `i`, `a`, `o`, etc.
- **Visual mode** — for selecting text. Enter with `v` (char), `V` (line), `Ctrl-v` (block).
- **Command mode** — type `:` then a command (e.g. `:w` to save, `:q` to quit).
- **Buffer** — an open file in memory. You can have many buffers; only some are visible.
- **Window** — a view onto a buffer. One buffer can show in several windows.
- **Tab** — a layout of windows. Different from browser tabs; more like a "workspace".
- **Split** — dividing a window into two (horizontal/vertical) to see two files at once.
- **Session** — a saved snapshot of your open files and layout, so you can resume later.

## Configuration

- **Config / dotfiles** — your personal settings files. For Neovim, usually `~/.config/nvim/`.
- **`init.lua`** — the main Neovim config file (Lua). Replaces the older `init.vim`.
- **Lua** — the scripting language Neovim uses for configuration. Small and readable.
- **Vimscript** — the older config language; still works, but Lua is preferred now.
- **Keymap / mapping** — binding a key (or keys) to an action, e.g. `Space + f` finds files.
- **Leader key** — a "prefix" key (often `Space`) that starts custom shortcuts.
- **Option / setting** — a toggle or value, e.g. line numbers, tab width.

## Plugins

- **Plugin** — an add-on that extends Neovim (colors, file trees, LSP, etc.).
- **Plugin manager** — installs and updates plugins. Common one: `lazy.nvim`.
- **Lazy loading** — loading a plugin only when needed, to keep startup fast.
- **Colorscheme** — the color theme of the editor (text, background, highlights).
- **Statusline** — the info bar at the bottom (mode, file, git branch, etc.).
- **File explorer** — a sidebar showing your folder tree (e.g. `neo-tree`, `nvim-tree`).
- **Dashboard** — a startup screen with recent files and shortcuts.
- **Which-key** — a popup that lists available shortcuts after you press the leader key.

## Code intelligence

- **LSP (Language Server Protocol)** — a standard way for editors to get smart features
  (autocomplete, go-to-definition, rename, diagnostics) from a language server.
- **Language server** — a program that understands one language and talks LSP to Neovim.
- **Mason** — a Neovim plugin that installs language servers and tools for you.
- **Tree-sitter** — a parser that gives accurate syntax highlighting and code structure.
- **Completion** — suggestions that appear as you type (often via `nvim-cmp`).
- **Snippet** — a reusable code template you expand with a trigger word.
- **Diagnostic** — an error/warning/hint shown inline by the LSP.
- **Formatter** — a tool that rewrites code to a standard style (e.g. `prettier`, `stylua`).
- **Linter** — a tool that flags code smells without changing the file.

## Navigation & search

- **Fuzzy finder** — search by typing partial names; results narrow as you type.
- **Telescope** — the most popular fuzzy finder plugin for Neovim.
- **Grep / live grep** — searching text across files.
- **Buffer list** — switching between open files.

## Git

- **Git** — version control system tracking changes to your code.
- **Gitsigns** — a plugin showing added/changed/deleted lines in the gutter.
- **Fugitive** — a plugin for running git commands inside Neovim.

## Terminal & tools

- **Terminal** — a command-line window; Neovim can host one inside a split.
- **tmux** — a terminal multiplexer; lets you split terminals and keep sessions alive.
- **CLI** — command-line interface (typing commands instead of clicking).
- **Shell** — the program that runs your commands (bash, zsh, fish).

## AI / "agentic coding"

- **Agentic coding** — using AI agents that can read, edit, and run code on your behalf,
  often inside the editor or terminal.
- **Copilot / AI assistant** — a tool suggesting or writing code from prompts.
- **Prompt** — the instruction you give to an AI.
- **Context** — the code/info the AI can see when answering.

## ASMR / aesthetics (video-specific)

- **ASMR** — "Autonomous Sensory Meridian Response": soft sounds (typing, clicks) that many
  find relaxing. Here, the video has no voiceover, just these sounds.
- **Aesthetics** — how the setup looks and feels: colors, spacing, cleanliness.
- **Minimal** — keeping only what's needed; fewer plugins, less clutter.

## Misc.

- **Dotfiles repo** — a git repo holding your config so you can sync it across machines.
- **PWA** — Progressive Web App (not Neovim-related, but appears in other shares).
- **Open source** — software whose source code is public and freely usable.

---

*This glossary is a living document. Add terms as you meet them.*