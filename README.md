# Neovim Keymaps for Web Development - Table of Contents

## Key Notation Legend
- `<C-x>` = Press Ctrl + x
- `<S-x>` = Press Shift + x (or capital X)
- `<A-x>` = Press Alt + x
- `<leader>` = Leader key (default: space)
- `<CR>` = Enter/Return key
- `<Esc>` = Escape key

## Table of Contents

1. [Basic Movement](#basic-movement)
2. [Fast Movement](#fast-movement)
3. [Selecting Text](#selecting-text)
4. [Bracket & Parenthesis Navigation](#bracket--parenthesis-navigation)
5. [Code Navigation](#code-navigation)
6. [File Navigation](#file-navigation)
7. [Window Management](#window-management)
8. [File Explorer (Neo-tree)](#file-explorer-neo-tree)
9. [Terminal Integration](#terminal-integration)
10. [Web Development Specific](#web-development-specific)
11. [Git Integration](#git-integration)
12. [LSP Features](#lsp-features)
13. [File Operations](#file-operations)
14. [Search and Replace](#search-and-replace)
15. [Visual Mode Tricks](#visual-mode-tricks)
16. [LazyVim Default Plugins](#lazyvim-default-plugins)

## Basic Movement

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `h` | Move cursor left | Normal, Visual | Lowercase h |
| `j` | Move cursor down | Normal, Visual | Lowercase j |
| `k` | Move cursor up | Normal, Visual | Lowercase k |
| `l` | Move cursor right | Normal, Visual | Lowercase l |
| `w` | Jump to start of next word | Normal, Visual | Lowercase w |
| `b` | Jump to start of previous word | Normal, Visual | Lowercase b |
| `e` | Jump to end of current word | Normal, Visual | Lowercase e |
| `0` | Jump to start of line | Normal, Visual | Zero key |
| `$` | Jump to end of line | Normal, Visual | Dollar sign key |
| `gg` | Jump to start of file | Normal, Visual | Lowercase g pressed twice |
| `G` | Jump to end of file | Normal, Visual | Uppercase G (Shift+g) |
| `{` | Jump to previous paragraph | Normal, Visual | Left curly brace |
| `}` | Jump to next paragraph | Normal, Visual | Right curly brace |

## Fast Movement

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `<C-u>` | Move half page up | Normal, Visual | Ctrl + u |
| `<C-d>` | Move half page down | Normal, Visual | Ctrl + d |
| `<C-b>` | Move full page up | Normal, Visual | Ctrl + b |
| `<C-f>` | Move full page down | Normal, Visual | Ctrl + f |
| `zz` | Center screen on cursor | Normal | Lowercase z pressed twice |
| `<leader>j` | Move current line/selection down | Normal, Visual | Leader key then j |
| `<leader>k` | Move current line/selection up | Normal, Visual | Leader key then k |

## Selecting Text

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `V` | Select entire line | Normal | Uppercase V (Shift+v) |
| `v` | Enter visual mode (character selection) | Normal | Lowercase v |
| `<C-v>` | Enter visual block mode | Normal | Ctrl + v |
| `vip` | Select inner paragraph | Normal | v, then i, then p |
| `vit` | Select inside tag | Normal | v, then i, then t |
| `viw` | Select inner word | Normal | v, then i, then w |
| `ggVG` | Select entire file | Normal | gg, then Shift+v, then G |
| `va{` | Select block including braces | Normal | v, then a, then { |
| `vi{` | Select inside braces | Normal | v, then i, then { |

## Bracket & Parenthesis Navigation

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `%` | Jump to matching bracket/parenthesis | Normal, Visual | Percent sign |
| `]}` | Jump to next closing curly brace | Normal | Right bracket, then right curly brace |
| `[{` | Jump to previous opening curly brace | Normal | Left bracket, then left curly brace |
| `])` | Jump to next closing parenthesis | Normal | Right bracket, then right parenthesis |
| `[(` | Jump to previous opening parenthesis | Normal | Left bracket, then left parenthesis |
| `ci{` | Change text inside curly braces | Normal | c, then i, then { |
| `ca{` | Change text including curly braces | Normal | c, then a, then { |
| `ci(` | Change text inside parentheses | Normal | c, then i, then ( |
| `ci"` | Change text inside quotes | Normal | c, then i, then " |
| `di{` | Delete text inside curly braces | Normal | d, then i, then { |
| `<Esc>` | Exit from auto-created closing bracket | Insert | Escape key |
| `<C-l>` | Exit from auto-created closing bracket | Insert | Ctrl + l (with lexima.vim) |
| `<Right>` | Move right past closing bracket | Insert | Right arrow key |
| `a` | Exit bracket and append after | Normal | Lowercase a (when cursor is inside bracket) |
| `<Tab>` | Jump past closing bracket | Insert | Tab key (with some snippets plugins) |

## Code Navigation

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `gd` | Go to definition | Normal | g, then d |
| `gr` | Go to references | Normal | g, then r |
| `gI` | Go to implementation | Normal | g, then uppercase I (Shift+i) |
| `<leader>ca` | Code actions | Normal | Leader key, then c, then a |
| `<leader>rn` | Rename symbol | Normal | Leader key, then r, then n |
| `]d` | Go to next diagnostic | Normal | Right bracket, then d |
| `[d` | Go to previous diagnostic | Normal | Left bracket, then d |
| `]e` | Go to next error | Normal | Right bracket, then e |
| `[e` | Go to previous error | Normal | Left bracket, then e |

## File Navigation

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `<leader>ff` | Find files | Normal | Leader key, then f, then f |
| `<leader>fg` | Live grep (search in files) | Normal | Leader key, then f, then g |
| `<leader>fb` | Find buffers | Normal | Leader key, then f, then b |
| `<leader>fr` | Find recent files | Normal | Leader key, then f, then r |
| `<C-o>` | Jump back in jump list | Normal | Ctrl + o |
| `<C-i>` | Jump forward in jump list | Normal | Ctrl + i |

## Window Management

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `<C-w>v` | Split window vertically | Normal | Ctrl + w, then v |
| `<C-w>s` | Split window horizontally | Normal | Ctrl + w, then s |
| `<C-h>` | Navigate to left window | Normal | Ctrl + h |
| `<C-j>` | Navigate to bottom window | Normal | Ctrl + j |
| `<C-k>` | Navigate to top window | Normal | Ctrl + k |
| `<C-l>` | Navigate to right window | Normal | Ctrl + l |
| `<C-w>q` | Close current window | Normal | Ctrl + w, then q |
| `<leader>-` | Split window below | Normal | Leader key, then hyphen |
| `<leader>\|` | Split window right | Normal | Leader key, then pipe |
| `<leader>wd` | Delete window | Normal | Leader key, then w, then d |

## File Explorer (Neo-tree)

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `<leader>e` | Toggle file explorer | Normal | Leader key, then e |
| `<leader>o` | Focus file in explorer | Normal | Leader key, then o |
| `j` / `k` | Move up/down in file tree | Neo-tree | Lowercase j / k |
| `h` | Collapse folder/go to parent | Neo-tree | Lowercase h |
| `l` | Expand folder/open file | Neo-tree | Lowercase l |
| `<CR>` | Open file/folder | Neo-tree | Enter/Return key |
| `<C-v>` | Open file in vertical split | Neo-tree | Ctrl + v |
| `<C-x>` | Open file in horizontal split | Neo-tree | Ctrl + x |
| `<C-t>` | Open file in new tab | Neo-tree | Ctrl + t |
| `a` | Create new file/directory | Neo-tree | Lowercase a |
| `d` | Delete file/directory | Neo-tree | Lowercase d |
| `r` | Rename file/directory | Neo-tree | Lowercase r |
| `q` | Close file explorer | Neo-tree | Lowercase q |

## Terminal Integration

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `<leader>ft` | Open floating terminal | Normal | Leader key, then f, then t |
| `<leader>fT` | Open vertical terminal | Normal | Leader key, then f, then Shift+t |
| `<leader>ih` | Open horizontal terminal | Normal | Leader key, then i, then h |
| `<leader>iv` | Open vertical terminal | Normal | Leader key, then i, then v |
| `<C-\>` | Toggle terminal | Normal | Ctrl + backslash |
| `<C-\><C-n>` | Exit terminal mode to normal mode | Terminal | Ctrl + backslash, then Ctrl + n |
| `i` | Enter terminal mode | Normal (in terminal buffer) | Lowercase i |

## Web Development Specific

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `cit` | Change inside tag | Normal | c, then i, then t |
| `dit` | Delete inside tag | Normal | d, then i, then t |
| `vat` | Select entire tag | Normal | v, then a, then t |
| `dst` | Delete surrounding tag | Normal | d, then s, then t |
| `cst` | Change surrounding tag | Normal | c, then s, then t |
| `<leader>cf` | Format document | Normal | Leader key, then c, then f |
| `<leader>cp` | Show CSS properties | Normal | Leader key, then c, then p |
| `ysiw"` | Surround word with quotes | Normal | y, then s, then i, then w, then " |
| `<leader>cs` | Toggle string quotes | Normal | Leader key, then c, then s |

## Git Integration

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `<leader>gs` | Git status | Normal | Leader key, then g, then s |
| `<leader>gd` | Git diff | Normal | Leader key, then g, then d |
| `<leader>gc` | Git commit | Normal | Leader key, then g, then c |
| `<leader>gb` | Git blame | Normal | Leader key, then g, then b |
| `]c` | Go to next git change | Normal | Right bracket, then c |
| `[c` | Go to previous git change | Normal | Left bracket, then c |
| `<leader>ghp` | Preview git hunk | Normal | Leader key, then g, then h, then p |
| `<leader>ghr` | Reset git hunk | Normal | Leader key, then g, then h, then r |

## LSP Features

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `K` | Show hover documentation | Normal | Uppercase K (Shift+k) |
| `<C-k>` | Show signature help | Insert | Ctrl + k |
| `<leader>cr` | Show code references | Normal | Leader key, then c, then r |
| `<leader>cs` | Show document symbols | Normal | Leader key, then c, then s |
| `<leader>cw` | Show workspace symbols | Normal | Leader key, then c, then w |
| `<leader>ca` | Show code actions | Normal | Leader key, then c, then a |
| `<leader>cA` | Show source actions | Normal | Leader key, then c, then Shift+a |

## File Operations

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `<leader>fn` | New file | Normal | Leader key, then f, then n |
| `<leader>fs` | Save file | Normal | Leader key, then f, then s |
| `<leader>fS` | Save all files | Normal | Leader key, then f, then Shift+s |
| `<leader>fo` | Open file | Normal | Leader key, then f, then o |
| `<leader>fd` | Delete file | Normal | Leader key, then f, then d |

## Search and Replace

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `/` | Search forward | Normal | Forward slash |
| `?` | Search backward | Normal | Question mark |
| `*` | Search word under cursor | Normal | Asterisk |
| `:%s/old/new/g` | Replace in file | Command | Colon, percent, s, forward slash, search term, forward slash, replacement, forward slash, g |
| `<leader>sr` | Search and replace in file | Normal | Leader key, then s, then r |
| `<leader>sR` | Search and replace in project | Normal | Leader key, then s, then Shift+r |

## Visual Mode Tricks

| Command | What It Does | Mode | Key Explanation |
|---------|--------------|------|----------------|
| `<` | Indent left | Visual | Left angle bracket |
| `>` | Indent right | Visual | Right angle bracket |
| `J` | Move selected lines down | Visual | Uppercase J (Shift+j) |
| `K` | Move selected lines up | Visual | Uppercase K (Shift+k) |
| `p` | Paste over selection | Visual | Lowercase p |
| `gc` | Comment selection | Visual | g, then c |

## LazyVim Default Plugins

| Plugin | Description | Key Features |
|--------|-------------|-------------|
| **Neo-tree** | File explorer with tree view | File management, project navigation |
| **Telescope** | Fuzzy finder | Powerful search for files, buffers, and text |
| **Which-key** | Displays keybindings in popup | Shows available commands after pressing leader key |
| **LSP** | Language Server Protocol | Code intelligence, diagnostics, formatting |
| **nvim-cmp** | Autocompletion engine | Completion suggestions for code |
| **LuaSnip** | Snippet engine | Code snippets for faster development |
| **Mason** | LSP/DAP/linter installer | Easy installation of language servers |
| **Treesitter** | Advanced syntax highlighting | Improved code highlighting and parsing |
| **Gitsigns** | Git integration in the gutter | Shows git changes in the editor |
| **Mini** | Collection of plugins | Various utilities (e.g., surround, pairs, comment) |
| **Bufferline** | Tab/buffer management | Navigate between open buffers |
| **Lualine** | Status line | Shows file status, git info, and diagnostics |
| **Indent-blankline** | Indentation guides | Visual guides for code indentation |
| **Trouble** | List for diagnostics | Lists all problems in code |
| **Todo-comments** | Highlight TODO comments | Makes TODOs and FIXMEs stand out |
| **Neodev** | Better development for Neovim | Improved API documentation for Neovim |
| **Noice** | UI enhancements | Improves command line and notifications |
| **Conform** | Code formatter | Formats code according to style guidelines |
| **Leap** | Motion plugin | Efficient cursor movement |
| **Lazygit** | Git terminal UI | Interactive git interface |
| **nvim-notify** | Notification system | Custom notification popups |

### Plugin-Specific Shortcuts

| Command | What It Does | Plugin | Key Explanation |
|---------|--------------|--------|----------------|
| `<leader>ff` | Find files | Telescope | Leader key, then f, then f |
| `<leader>e` | Toggle file explorer | Neo-tree | Leader key, then e |
| `<leader>gg` | Open LazyGit | LazyGit | Leader key, then g, then g |
| `<leader>xx` | Toggle diagnostics list | Trouble | Leader key, then x, then x |
| `s{char}{char}` | Jump to matches | Leap | s, then two characters to search for |
| `<leader>tt` | Toggle todo list | Todo-comments | Leader key, then t, then t |
| `gcc` | Comment line | Mini.comment | g, then c, then c |
| `<C-Space>` | Complete suggestion | nvim-cmp | Ctrl + Space |
| `<Tab>` | Navigate through snippet placeholders | LuaSnip | Tab key (in snippet) |
| `<leader>cf` | Format document | Conform | Leader key, then c, then f |
| `<leader>bd` | Delete buffer | Bufferline | Leader key, then b, then d |
| `<leader>bp` | Pin buffer | Bufferline | Leader key, then b, then p |
