# LazyVim MERN Stack Development Cheatsheet

## Table of Contents
- [General Navigation](#general-navigation)
- [File Management](#file-management)
- [Buffer and Window Navigation](#buffer-and-window-navigation)
- [Selection Operations](#selection-operations)
- [Deletion Operations](#deletion-operations)
- [Project Management](#project-management)
- [Code Editing](#code-editing)
- [Code Navigation](#code-navigation)
- [Search and Replace](#search-and-replace)
- [JavaScript/TypeScript Specific](#javascripttypescript-specific)
- [React Specific](#react-specific)
- [MongoDB Operations](#mongodb-operations)
- [Express API Development](#express-api-development)
- [Git Operations](#git-operations)
- [Terminal Integration](#terminal-integration)
- [Debugging](#debugging)
- [Deployment](#deployment)
- [LazyVim Configuration](#lazyvim-configuration)

## General Navigation

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `h`, `j`, `k`, `l` | Move cursor left, down, up, right | Normal | Press key directly |
| `w` | Jump to start of next word | Normal | Press key directly |
| `b` | Jump to start of previous word | Normal | Press key directly |
| `e` | Jump to end of current word | Normal | Press key directly |
| `0` | Jump to start of line | Normal | Press key directly |
| `$` | Jump to end of line | Normal | Press key directly |
| `gg` | Go to top of file | Normal | Press `g` twice |
| `G` | Go to bottom of file | Normal | Press `Shift+g` |
| `Ctrl+o` | Jump back in jump list | Normal | Hold `Ctrl` and press `o` |
| `Ctrl+i` | Jump forward in jump list | Normal | Hold `Ctrl` and press `i` |
| `Ctrl+u` | Scroll half-page up | Normal | Hold `Ctrl` and press `u` |
| `Ctrl+d` | Scroll half-page down | Normal | Hold `Ctrl` and press `d` |
| `<Space>` | Leader key (used for many shortcuts) | Normal | Press spacebar |
| `zz` | Center cursor on screen | Normal | Press `z` twice |
| `H` | Move to top of screen | Normal | Press `Shift+h` |
| `M` | Move to middle of screen | Normal | Press `Shift+m` |
| `L` | Move to bottom of screen | Normal | Press `Shift+l` |

## File Management

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `<Space>ff` | Find file in project | Normal | Press `Space`, then `f`, then `f` |
| `<Space>fr` | Find recent files | Normal | Press `Space`, then `f`, then `r` |
| `<Space>fn` | New file | Normal | Press `Space`, then `f`, then `n` |
| `<Space>fs` | Save file | Normal | Press `Space`, then `f`, then `s` |
| `<Space>fS` | Save all files | Normal | Press `Space`, then `f`, then `Shift+s` |
| `<Space>fo` | Open file | Normal | Press `Space`, then `f`, then `o` |
| `:w` | Save file | Command | Type `:w` and press `Enter` |
| `:q` | Quit current buffer | Command | Type `:q` and press `Enter` |
| `:wq` | Save and quit | Command | Type `:wq` and press `Enter` |
| `:e <filename>` | Open file | Command | Type `:e filename` and press `Enter` |
| `<Space>bd` | Close current buffer | Normal | Press `Space`, then `b`, then `d` |
| `<Space>fd` | Delete file under cursor | Normal | Press `Space`, then `f`, then `d` |
| `gf` | Go to file under cursor | Normal | Press `g`, then `f` |
| `<Space>fp` | Copy path of current file | Normal | Press `Space`, then `f`, then `p` |
| `<Space>fP` | Copy absolute path of current file | Normal | Press `Space`, then `f`, then `Shift+p` |
| `<Space>fy` | Copy filename of current file | Normal | Press `Space`, then `f`, then `y` |
| `<Space>fD` | Duplicate current file | Normal | Press `Space`, then `f`, then `Shift+d` |
| `<Space>fR` | Rename current file | Normal | Press `Space`, then `f`, then `Shift+r` |

## Buffer and Window Navigation

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `<Space>bb` | Switch to buffer | Normal | Press `Space`, then `b`, then `b` |
| `<Space>bp` | Previous buffer | Normal | Press `Space`, then `b`, then `p` |
| `<Space>bn` | Next buffer | Normal | Press `Space`, then `b`, then `n` |
| `<Space>bd` | Delete buffer | Normal | Press `Space`, then `b`, then `d` |
| `<Space>b]` | Next buffer | Normal | Press `Space`, then `b`, then `]` |
| `<Space>b[` | Previous buffer | Normal | Press `Space`, then `b`, then `[` |
| `<Space>bl` | List all buffers | Normal | Press `Space`, then `b`, then `l` |
| `<Space>b1`-`9` | Go to buffer 1-9 | Normal | Press `Space`, then `b`, then `1`-`9` |
| `<Space>w-` | Split window horizontally | Normal | Press `Space`, then `w`, then `-` |
| `<Space>w\|` | Split window vertically | Normal | Press `Space`, then `w`, then `\|` |
| `<Space>ww` | Switch to other window | Normal | Press `Space`, then `w`, then `w` |
| `<Space>wd` | Delete window | Normal | Press `Space`, then `w`, then `d` |
| `<Space>wh` | Move to left window | Normal | Press `Space`, then `w`, then `h` |
| `<Space>wj` | Move to window below | Normal | Press `Space`, then `w`, then `j` |
| `<Space>wk` | Move to window above | Normal | Press `Space`, then `w`, then `k` |
| `<Space>wl` | Move to right window | Normal | Press `Space`, then `w`, then `l` |
| `<Space>wq` | Quit window | Normal | Press `Space`, then `w`, then `q` |
| `<Space>ws` | Split window and go to file | Normal | Press `Space`, then `w`, then `s` |
| `Ctrl+w =` | Make all windows equal size | Normal | Hold `Ctrl`, press `w`, release, then press `=` |

## Selection Operations

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `v` | Enter visual mode (character selection) | Normal | Press key directly |
| `V` | Enter visual line mode | Normal | Press `Shift+v` |
| `Ctrl+v` | Enter visual block mode | Normal | Hold `Ctrl` and press `v` |
| `ggVG` | Select entire file | Normal | Press `gg`, then `Shift+v`, then `Shift+g` |
| `vap` | Select around paragraph | Normal | Press `v`, then `a`, then `p` |
| `vaw` | Select around word | Normal | Press `v`, then `a`, then `w` |
| `viw` | Select inner word | Normal | Press `v`, then `i`, then `w` |
| `vi"` | Select inside double quotes | Normal | Press `v`, then `i`, then `"` |
| `vi'` | Select inside single quotes | Normal | Press `v`, then `i`, then `'` |
| `vi{` | Select inside curly braces | Normal | Press `v`, then `i`, then `{` |
| `vi(` | Select inside parentheses | Normal | Press `v`, then `i`, then `(` |
| `va{` | Select around curly braces | Normal | Press `v`, then `a`, then `{` |
| `va(` | Select around parentheses | Normal | Press `v`, then `a`, then `(` |
| `o` | Move to other end of selection | Visual | Press key directly |
| `>` | Indent selected text | Visual | Press `>` |
| `<` | Outdent selected text | Visual | Press `<` |

## Deletion Operations

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `x` | Delete character under cursor | Normal | Press key directly |
| `X` | Delete character before cursor | Normal | Press `Shift+x` |
| `dd` | Delete line | Normal | Press `d` twice |
| `D` | Delete from cursor to end of line | Normal | Press `Shift+d` |
| `d0` | Delete from cursor to beginning of line | Normal | Press `d`, then `0` |
| `dw` | Delete from cursor to end of word | Normal | Press `d`, then `w` |
| `db` | Delete from cursor to beginning of word | Normal | Press `d`, then `b` |
| `dG` | Delete from cursor to end of file | Normal | Press `d`, then `Shift+g` |
| `dgg` | Delete from cursor to beginning of file | Normal | Press `d`, then `gg` |
| `d}` | Delete until next paragraph | Normal | Press `d`, then `}` |
| `d{` | Delete until previous paragraph | Normal | Press `d`, then `{` |
| `di"` | Delete inside double quotes | Normal | Press `d`, then `i`, then `"` |
| `di'` | Delete inside single quotes | Normal | Press `d`, then `i`, then `'` |
| `di{` | Delete inside curly braces | Normal | Press `d`, then `i`, then `{` |
| `di(` | Delete inside parentheses | Normal | Press `d`, then `i`, then `(` |
| `dap` | Delete around paragraph | Normal | Press `d`, then `a`, then `p` |
| `cc` | Change entire line | Normal | Press `c` twice |
| `cw` | Change word | Normal | Press `c`, then `w` |
| `ciw` | Change inside word | Normal | Press `c`, then `i`, then `w` |
| `ggVGd` | Delete entire file content | Normal | Press `gg`, then `Shift+v`, then `Shift+g`, then `d` |
| `:%d` | Delete all lines in file | Command | Type `:%d` and press `Enter` |

## Project Management

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `<Space>pf` | Project find files | Normal | Press `Space`, then `p`, then `f` |
| `<Space>ps` | Project search text | Normal | Press `Space`, then `p`, then `s` |
| `<Space>pc` | Project config | Normal | Press `Space`, then `p`, then `c` |
| `<Space>pp` | Switch project | Normal | Press `Space`, then `p`, then `p` |
| `<Space>pn` | Create new project | Normal | Press `Space`, then `p`, then `n` |
| `<Space>pa` | Add folder to workspace | Normal | Press `Space`, then `p`, then `a` |

## Code Editing

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `i` | Enter insert mode | Normal | Press key directly |
| `a` | Enter insert mode after cursor | Normal | Press key directly |
| `I` | Insert at beginning of line | Normal | Press `Shift+i` |
| `A` | Insert at end of line | Normal | Press `Shift+a` |
| `o` | Insert new line below | Normal | Press key directly |
| `O` | Insert new line above | Normal | Press `Shift+o` |
| `dd` | Delete line | Normal | Press `d` twice |
| `yy` | Yank (copy) line | Normal | Press `y` twice |
| `p` | Paste after cursor | Normal | Press key directly |
| `P` | Paste before cursor | Normal | Press `Shift+p` |
| `u` | Undo | Normal | Press key directly |
| `Ctrl+r` | Redo | Normal | Hold `Ctrl` and press `r` |
| `<<` | Shift line left (decrease indent) | Normal | Press `<` twice |
| `>>` | Shift line right (increase indent) | Normal | Press `>` twice |
| `gd` | Go to definition | Normal | Press `g`, then `d` |
| `gr` | Go to references | Normal | Press `g`, then `r` |
| `K` | Show documentation | Normal | Press `Shift+k` |
| `<Space>ca` | Code action | Normal | Press `Space`, then `c`, then `a` |
| `<Space>cf` | Format code | Normal | Press `Space`, then `c`, then `f` |
| `<Space>cr` | Rename symbol | Normal | Press `Space`, then `c`, then `r` |
| `J` | Join line below with current line | Normal | Press `Shift+j` |
| `C` | Change to end of line | Normal | Press `Shift+c` |
| `~` | Toggle case of character under cursor | Normal | Press `~` |
| `g~iw` | Toggle case of word | Normal | Press `g`, then `~`, then `i`, then `w` |
| `gUiw` | Make word uppercase | Normal | Press `g`, then `Shift+u`, then `i`, then `w` |
| `guiw` | Make word lowercase | Normal | Press `g`, then `u`, then `i`, then `w` |
| `>iB` | Indent code block | Normal | Press `>`, then `i`, then `Shift+b` |
| `<iB` | Outdent code block | Normal | Press `<`, then `i`, then `Shift+b` |
| `=iB` | Auto-indent code block | Normal | Press `=`, then `i`, then `Shift+b` |
| `gg=G` | Auto-indent entire file | Normal | Press `gg`, then `=`, then `Shift+g` |

## Code Navigation

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `Ctrl+]` | Go to definition | Normal | Hold `Ctrl` and press `]` |
| `Ctrl+t` | Go back from definition | Normal | Hold `Ctrl` and press `t` |
| `<Space>ls` | Document symbols | Normal | Press `Space`, then `l`, then `s` |
| `<Space>lS` | Workspace symbols | Normal | Press `Space`, then `l`, then `Shift+s` |
| `gd` | Go to definition | Normal | Press `g`, then `d` |
| `gr` | Go to references | Normal | Press `g`, then `r` |
| `gD` | Go to declaration | Normal | Press `g`, then `Shift+d` |
| `gi` | Go to implementation | Normal | Press `g`, then `i` |
| `<Space>lj` | Next diagnostic | Normal | Press `Space`, then `l`, then `j` |
| `<Space>lk` | Previous diagnostic | Normal | Press `Space`, then `l`, then `k` |
| `]}` | Jump to next function | Normal | Press `]`, then `}` |
| `[{` | Jump to previous function | Normal | Press `[`, then `{` |

## Search and Replace

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `/` | Search forward | Normal | Press `/`, type search, press `Enter` |
| `?` | Search backward | Normal | Press `?`, type search, press `Enter` |
| `n` | Next search result | Normal | Press key directly |
| `N` | Previous search result | Normal | Press `Shift+n` |
| `*` | Search word under cursor | Normal | Press `*` |
| `#` | Search word under cursor backwards | Normal | Press `#` |
| `:%s/old/new/g` | Replace all occurrences | Command | Type `:%s/old/new/g` and press `Enter` |
| `:%s/old/new/gc` | Replace with confirmation | Command | Type `:%s/old/new/gc` and press `Enter` |
| `<Space>s` | Search in project | Normal | Press `Space`, then `s` |
| `<Space>sr` | Search and replace in project | Normal | Press `Space`, then `s`, then `r` |

## JavaScript/TypeScript Specific

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `<Space>li` | Organize imports | Normal | Press `Space`, then `l`, then `i` |
| `<Space>lf` | Fix current | Normal | Press `Space`, then `l`, then `f` |
| `<Space>lv` | Extract variable | Normal | Press `Space`, then `l`, then `v` |
| `<Space>lm` | Extract method | Normal | Press `Space`, then `l`, then `m` |
| `]f` | Next function | Normal | Press `]`, then `f` |
| `[f` | Previous function | Normal | Press `[`, then `f` |
| `]c` | Next class | Normal | Press `]`, then `c` |
| `[c` | Previous class | Normal | Press `[`, then `c` |
| `<Space>lt` | Run current test | Normal | Press `Space`, then `l`, then `t` |
| `<Space>cj` | Create JavaScript file | Normal | Press `Space`, then `c`, then `j` |
| `<Space>ct` | Create TypeScript file | Normal | Press `Space`, then `c`, then `t` |

## React Specific

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `<Space>cr` | Create React component | Normal | Press `Space`, then `c`, then `r` |
| `<Space>ch` | Create React hook | Normal | Press `Space`, then `c`, then `h` |
| `<Space>cc` | Create React context | Normal | Press `Space`, then `c`, then `c` |
| `rafce` + `Tab` | Create functional component with arrow function (snippet) | Insert | Type `rafce` and press `Tab` |
| `rfc` + `Tab` | Create functional component (snippet) | Insert | Type `rfc` and press `Tab` |
| `rcc` + `Tab` | Create class component (snippet) | Insert | Type `rcc` and press `Tab` |
| `<Space>lp` | Toggle React prop types | Normal | Press `Space`, then `l`, then `p` |
| `<Space>le` | Extract React component | Normal | Press `Space`, then `l`, then `e` |
| `]r` | Next React component | Normal | Press `]`, then `r` |
| `[r` | Previous React component | Normal | Press `[`, then `r` |

## MongoDB Operations

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `<Space>dmc` | Create MongoDB connection | Normal | Press `Space`, then `d`, then `m`, then `c` |
| `<Space>dmq` | Query MongoDB | Normal | Press `Space`, then `d`, then `m`, then `q` |
| `<Space>dms` | MongoDB schema snippets | Normal | Press `Space`, then `d`, then `m`, then `s` |
| `mngsm` + `Tab` | Create MongoDB schema (snippet) | Insert | Type `mngsm` and press `Tab` |
| `mngq` + `Tab` | Create MongoDB query (snippet) | Insert | Type `mngq` and press `Tab` |
| `mngc` + `Tab` | Create MongoDB connection (snippet) | Insert | Type `mngc` and press `Tab` |

## Express API Development

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `<Space>der` | Create Express route | Normal | Press `Space`, then `d`, then `e`, then `r` |
| `<Space>dec` | Create Express controller | Normal | Press `Space`, then `d`, then `e`, then `c` |
| `<Space>dem` | Create Express middleware | Normal | Press `Space`, then `d`, then `e`, then `m` |
| `expr` + `Tab` | Express route snippet | Insert | Type `expr` and press `Tab` |
| `expc` + `Tab` | Express controller snippet | Insert | Type `expc` and press `Tab` |
| `expm` + `Tab` | Express middleware snippet | Insert | Type `expm` and press `Tab` |
| `<Space>lep` | Express project setup | Normal | Press `Space`, then `l`, then `e`, then `p` |

## Git Operations

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `<Space>gg` | Open Git status | Normal | Press `Space`, then `g`, then `g` |
| `<Space>gc` | Git commit | Normal | Press `Space`, then `g`, then `c` |
| `<Space>gp` | Git push | Normal | Press `Space`, then `g`, then `p` |
| `<Space>gl` | Git pull | Normal | Press `Space`, then `g`, then `l` |
| `<Space>gb` | Git blame | Normal | Press `Space`, then `g`, then `b` |
| `<Space>gd` | Git diff | Normal | Press `Space`, then `g`, then `d` |
| `<Space>gh` | Git history | Normal | Press `Space`, then `g`, then `h` |
| `<Space>gr` | Git reset | Normal | Press `Space`, then `g`, then `r` |
| `<Space>gs` | Git stage file | Normal | Press `Space`, then `g`, then `s` |
| `<Space>gS` | Git stage all | Normal | Press `Space`, then `g`, then `Shift+s` |
| `<Space>gC` | Git checkout | Normal | Press `Space`, then `g`, then `Shift+c` |
| `<Space>gB` | Git create branch | Normal | Press `Space`, then `g`, then `Shift+b` |

## Terminal Integration

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `<Space>tt` | Toggle terminal | Normal | Press `Space`, then `t`, then `t` |
| `<Space>tn` | New terminal | Normal | Press `Space`, then `t`, then `n` |
| `<Space>th` | Terminal horizontal split | Normal | Press `Space`, then `t`, then `h` |
| `<Space>tv` | Terminal vertical split | Normal | Press `Space`, then `t`, then `v` |
| `<Space>tr` | Run current file | Normal | Press `Space`, then `t`, then `r` |
| `<Space>tp` | Run previous command | Normal | Press `Space`, then `t`, then `p` |
| `<Esc>` | Exit terminal mode | Terminal | Press `Escape` |
| `Ctrl+\, Ctrl+n` | Exit terminal mode (alternative) | Terminal | Hold `Ctrl` and press `\`, then hold `Ctrl` and press `n` |

## Debugging

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `<Space>dd` | Start debugging | Normal | Press `Space`, then `d`, then `d` |
| `<Space>db` | Toggle breakpoint | Normal | Press `Space`, then `d`, then `b` |
| `<Space>dc` | Continue debugging | Normal | Press `Space`, then `d`, then `c` |
| `<Space>di` | Step into | Normal | Press `Space`, then `d`, then `i` |
| `<Space>do` | Step over | Normal | Press `Space`, then `d`, then `o` |
| `<Space>dO` | Step out | Normal | Press `Space`, then `d`, then `Shift+o` |
| `<Space>dr` | Restart debugging | Normal | Press `Space`, then `d`, then `r` |
| `<Space>dt` | Terminate debugging | Normal | Press `Space`, then `d`, then `t` |
| `<Space>dl` | Run last debugging configuration | Normal | Press `Space`, then `d`, then `l` |
| `<Space>de` | Evaluate expression | Normal | Press `Space`, then `d`, then `e` |
| `<Space>dw` | Watch expression | Normal | Press `Space`, then `d`, then `w` |

## Deployment

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `<Space>pd` | Deploy project | Normal | Press `Space`, then `p`, then `d` |
| `<Space>pb` | Build project | Normal | Press `Space`, then `p`, then `b` |
| `<Space>pc` | Project configuration | Normal | Press `Space`, then `p`, then `c` |
| `<Space>pD` | Docker commands | Normal | Press `Space`, then `p`, then `Shift+d` |
| `<Space>ph` | Heroku commands | Normal | Press `Space`, then `p`, then `h` |
| `<Space>pv` | Vercel commands | Normal | Press `Space`, then `p`, then `v` |
| `<Space>pa` | AWS commands | Normal | Press `Space`, then `p`, then `a` |
| `<Space>pm` | MongoDB Atlas commands | Normal | Press `Space`, then `p`, then `m` |
| `<Space>pe` | Environment variable management | Normal | Press `Space`, then `p`, then `e` |
| `<Space>pi` | CI/CD integration | Normal | Press `Space`, then `p`, then `i` |

## LazyVim Configuration

| Shortcut | Description | Mode | How to Press |
|----------|-------------|------|-------------|
| `<Space>Lc` | Edit LazyVim config | Normal | Press `Space`, then `Shift+l`, then `c` |
| `<Space>Lp` | Edit plugin config | Normal | Press `Space`, then `Shift+l`, then `p` |
| `<Space>Lr` | Reload configuration | Normal | Press `Space`, then `Shift+l`, then `r` |
| `<Space>Li` | Install plugins | Normal | Press `Space`, then `Shift+l`, then `i` |
| `<Space>Lu` | Update plugins | Normal | Press `Space`, then `Shift+l`, then `u` |
| `<Space>Lss` | Select colorscheme | Normal | Press `Space`, then `Shift+l`, then `s`, then `s` |
| `<Space>Lsf` | Select font | Normal | Press `Space`, then `Shift+l`, then `s`, then `f` |
| `<Space>Lk` | Edit keymaps | Normal | Press `Space`, then `Shift+l`, then `k` |
| `<Space>Ll` | Open lazyvim.log | Normal | Press `Space`, then `Shift+l`, then `l` |
| `<Space>Ls` | LazyVim status | Normal | Press `Space`, then `Shift+l`, then `s` |
| `<Space>LS` | LazyVim sync | Normal | Press `Space`, then `Shift+l`, then `Shift+s` |
| `<Space>Lt` | Toggle autoformat | Normal | Press `Space`, then `Shift+l`, then `t` |
| `<Space>LC` | LazyVim clean | Normal | Press `Space`, then `Shift+l`, then `Shift+c` |
| `<Space>L?` | Show LazyVim help | Normal | Press `Space`, then `Shift+l`, then `?` |
