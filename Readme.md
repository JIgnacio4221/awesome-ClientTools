# Awesome CLI Tools & Apps — The Ultimate Guide

> The definitive compilation of command-line tools that make the terminal a truly powerful experience. This repository integrates the best from [awesome-shell](https://github.com/alebcay/awesome-shell), [awesome-cli-apps](https://github.com/agarrharr/awesome-cli-apps), and original contributions into an organized, comprehensive, and up-to-date guide with over 700 CLI tools.

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](LICENSE.md)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0--1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

---

## Table of Contents

- [About This Guide](#about-this-guide)
- [How to Read the Tables](#how-to-read-the-tables)
- [Shell & Navigation](#shell--navigation)
- [File & Directory Management](#file--directory-management)
- [Search & Text Processing](#search--text-processing)
- [System Monitoring & Performance](#system-monitoring--performance)
- [Network & Web Tools](#network--web-tools)
- [Downloaders & Media](#downloaders--media)
- [Books & E-books](#books--e-books)
- [Media Processing](#media-processing)
- [Terminal Music & Audio Players](#terminal-music--audio-players)
- [Containers & Orchestration](#containers--orchestration)
- [Git & Development Tools](#git--development-tools)
- [Text Editors](#text-editors)
- [Productivity & Tasks](#productivity--tasks)
- [Research & Science](#research--science)
- [Databases & Data](#databases--data)
- [Security & Privacy](#security--privacy)
- [Terminal Multiplexers](#terminal-multiplexers)
- [Fun & Miscellaneous](#fun--miscellaneous)
- [Command Line Learning](#command-line-learning)
- [Contributing](#contributing)
- [License](#license)

---

## About This Guide

This is **NOT** a list of terminal emulators. It's a comprehensive catalog of **CLI utilities** — tools you run *inside* a terminal that enable extraordinary capabilities: generate QR codes, benchmark HTTP APIs, render images inline, explore JSON interactively, monitor GPU usage, play YouTube music, download from 1000+ sites, manage Kubernetes clusters, and much more.

All tools listed here are free, open-source, or have a significant free tier. Proprietary tools without open-source alternatives in their niche are marked accordingly.

This repository combines and expands three major sources:
- **awesome-shell** by Caleb (alebcay)
- **awesome-cli-apps** by Adam (agarrharr)  
- **Original contributions** and community updates

---

## How to Read the Tables

| Field | Description |
|---|---|
| **Name** | Tool name with link to its homepage or documentation |
| **Summary** | One-line description of what it does |
| **Description** | Key features and typical use cases |
| **OS** | Operating systems where it runs natively |
| **Repository** | Link to source code |
| **Latest Version** | Stable release — dynamic badge where available |
| **License** | Software license |
| **Open Source** | Whether source code is publicly available |

**OS Abbreviations:** `Win` = Windows · `Lin` = Linux · `mac` = macOS · `All` = all three  
**Legend:** ✅ Yes · ❌ No · ⚠️ Partial or source-available but not OSI-approved

> Version badges are fetched live from GitHub Releases. Tools hosted elsewhere show a static version or `—`.

---

## Shell & Navigation

Tools that improve how you navigate the shell, recall history, complete commands, configure your prompt, and manage tool versions.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [fzf](https://github.com/junegunn/fzf) | Interactive fuzzy finder for anything | Pipes any list into an interactive, real-time fuzzy-search selector. Integrates with shell history (`CTRL-R`), file paths (`CTRL-T`), and `cd` (`ALT-C`). Composable with almost every other CLI tool. | All | [junegunn/fzf](https://github.com/junegunn/fzf) | ![GitHub Release](https://img.shields.io/github/v/release/junegunn/fzf?label=) | MIT | ✅ |
| [zoxide](https://github.com/ajeetdsouza/zoxide) | Smarter `cd` that learns your habits | Tracks directories you visit and lets you jump to any with a short fuzzy keyword — `z proj` instead of the full path. Works with bash, zsh, fish, PowerShell, and more. | All | [ajeetdsouza/zoxide](https://github.com/ajeetdsouza/zoxide) | ![GitHub Release](https://img.shields.io/github/v/release/ajeetdsouza/zoxide?label=) | MIT | ✅ |
| [Starship](https://starship.rs/) | Fast, highly customizable cross-shell prompt | Written in Rust. Detects context automatically (git branch, Node version, Python venv, Kubernetes cluster…) and shows only what is relevant. Configured in a single TOML file; works in bash, zsh, fish, PowerShell, and more. | All | [starship-rs/starship](https://github.com/starship-rs/starship) | ![GitHub Release](https://img.shields.io/github/v/release/starship-rs/starship?label=) | ISC | ✅ |
| [atuin](https://atuin.sh/) | Magical shell history with sync | Replaces shell history with a SQLite database, enabling search by exit code, directory, hostname, or duration. Optionally syncs encrypted history across machines. | All | [atuinsh/atuin](https://github.com/atuinsh/atuin) | ![GitHub Release](https://img.shields.io/github/v/release/atuinsh/atuin?label=) | MIT | ✅ |
| [navi](https://github.com/denisidoro/navi) | Interactive cheatsheet tool for the terminal | Opens a searchable interface of shell one-liners and command snippets with input placeholders that prompt for values. Supports importing community cheatsheets with one command. | All | [denisidoro/navi](https://github.com/denisidoro/navi) | ![GitHub Release](https://img.shields.io/github/v/release/denisidoro/navi?label=) | MIT | ✅ |
| [thefuck](https://github.com/nvbn/thefuck) | Corrects your previous console command | Type `fuck` after a failed command and it suggests and applies the most likely fix — wrong sudo, typo, wrong git subcommand, etc. Supports hundreds of app-specific rules. | All | [nvbn/thefuck](https://github.com/nvbn/thefuck) | ![GitHub Release](https://img.shields.io/github/v/release/nvbn/thefuck?label=) | MIT | ✅ |
| [Nushell](https://www.nushell.sh/) | A new kind of shell that understands structured data | Instead of text streams, Nu pipelines pass structured data (tables, records, lists). Every command understands types, making data transformations in the shell composable and type-safe. | All | [nushell/nushell](https://github.com/nushell/nushell) | ![GitHub Release](https://img.shields.io/github/v/release/nushell/nushell?label=) | MIT | ✅ |
| [fish](https://fishshell.com/) | Friendly interactive shell with smart defaults | Autosuggestions (greyed-out completions as you type), syntax highlighting, and smart tab completions out of the box — zero configuration. Not POSIX-compatible by design; cleaner scripting syntax. | Lin/mac | [fish-shell/fish-shell](https://github.com/fish-shell/fish-shell) | ![GitHub Release](https://img.shields.io/github/v/release/fish-shell/fish-shell?label=) | GPL-2.0 | ✅ |
| [direnv](https://direnv.net/) | Load and unload env variables by directory | Automatically sources a `.envrc` file when you `cd` into a directory and unloads it when you leave. Essential for per-project secrets, PATH extensions, and tool version isolation. | Lin/mac | [direnv/direnv](https://github.com/direnv/direnv) | ![GitHub Release](https://img.shields.io/github/v/release/direnv/direnv?label=) | MIT | ✅ |
| [mise](https://mise.jdx.dev/) | Polyglot development tool version manager | Install and switch between versions of Node, Python, Ruby, Go, Rust, and dozens more. Reads `.tool-versions` files. Faster, more ergonomic successor to rtx and asdf. | Lin/mac | [jdx/mise](https://github.com/jdx/mise) | ![GitHub Release](https://img.shields.io/github/v/release/jdx/mise?label=) | MIT | ✅ |
| [mcfly](https://github.com/cantino/mcfly) | Neural network-powered shell history search | Learns from your command history to prioritize search results based on context (directory, exit status, time). Replaces `CTRL-R` with intelligent suggestions. | All | [cantino/mcfly](https://github.com/cantino/mcfly) | ![GitHub Release](https://img.shields.io/github/v/release/cantino/mcfly?label=) | MIT | ✅ |
| [oh-my-posh](https://ohmyposh.dev/) | Prompt theme engine for any shell | Highly customizable prompt with themes for PowerShell, bash, zsh, and more. Features rich segment support and automatic context detection similar to Starship. | All | [JanDeDobbeleer/oh-my-posh](https://github.com/JanDeDobbeleer/oh-my-posh) | ![GitHub Release](https://img.shields.io/github/v/release/JanDeDobbeleer/oh-my-posh?label=) | MIT | ✅ |
| [autojump](https://github.com/wting/autojump) | Fast directory navigator that learns your habits | Similar to zoxide — navigates to most-used directories with partial name matches. Works with bash, zsh, fish, and PowerShell. Older but still widely used. | Lin/mac | [wting/autojump](https://github.com/wting/autojump) | — | GPL-3.0 | ✅ |
| [z](https://github.com/rupa/z) | z is the new j, yo | Jump to frequently used directories with smart frecency algorithm | Lin/mac | [rupa/z](https://github.com/rupa/z) | — | WTFPL | ✅ |
| [z.lua](https://github.com/skywind3000/z.lua) | A fast cd command that helps you navigate faster | 3x faster than fasd and autojump, 10x faster than z | Lin/mac | [skywind3000/z.lua](https://github.com/skywind3000/z.lua) | — | MIT | ✅ |
| [bashmarks](https://github.com/huyng/bashmarks) | Directory bookmarks for the shell | Save and jump to commonly used directories with simple bookmarks | Lin/mac | [huyng/bashmarks](https://github.com/huyng/bashmarks) | — | MIT | ✅ |
| [bd](https://github.com/vigneshwaranr/bd) | Quickly go back to a parent directory | Jump back to a specific directory, without doing `cd ../../..` | Lin/mac | [vigneshwaranr/bd](https://github.com/vigneshwaranr/bd) | — | MIT | ✅ |
| [commacd](https://github.com/shyiko/commacd) | A faster way to move around in Bash | Comma-separated navigation shortcuts for bash | Lin/mac | [shyiko/commacd](https://github.com/shyiko/commacd) | — | MIT | ✅ |
| [enhancd](https://github.com/b4b4r07/enhancd) | A next-generation cd command with an interactive filter | cd with fuzzy-finder powered filter | Lin/mac | [b4b4r07/enhancd](https://github.com/b4b4r07/enhancd) | — | MIT | ✅ |
| [goto](https://github.com/iridakos/goto) | A shell utility for navigation to aliased directories | Directory aliases supporting tab-completion and persistence | Lin/mac | [iridakos/goto](https://github.com/iridakos/goto) | — | MIT | ✅ |
| [jump](https://github.com/gsamokovarov/jump) | Jump helps you navigate faster | Integrates with your shell and learns your habits | Lin/mac | [gsamokovarov/jump](https://github.com/gsamokovarov/jump) | — | MIT | ✅ |
| [lazy-cd](https://github.com/pedramamini/lazy-cd) | Simple bash commands for bookmarked navigation | Minimalist directory bookmarking solution | Lin/mac | [pedramamini/lazy-cd](https://github.com/pedramamini/lazy-cd) | — | MIT | ✅ |
| [up](https://github.com/shannonmoeller/up) | Ascend directories by name or count | Navigate directory hierarchies more efficiently | Lin/mac | [shannonmoeller/up](https://github.com/shannonmoeller/up) | — | MIT | ✅ |
| [shell++](https://github.com/alexst07/shell-plus-plus) | Friendly and modern shell script language | Object-oriented shell scripting language | Lin/mac | [alexst07/shell-plus-plus](https://github.com/alexst07/shell-plus-plus) | — | MIT | ✅ |
| [shenv](https://github.com/shenv/shenv) | Simple shell version management | Manage multiple shell versions | Lin/mac | [shenv/shenv](https://github.com/shenv/shenv) | — | MIT | ✅ |
| [tcsh](https://www.tcsh.org/) | C shell with file name completion and command line editing | Enhanced C-shell with command-line editing | Lin/mac | — | — | BSD | ✅ |
| [xonsh](https://xon.sh) | Python-ish, BASHwards-looking shell language | Shell language combining Python and Bash | All | [xonsh/xonsh](https://github.com/xonsh/xonsh) | — | BSD-2-Clause | ✅ |
| [yash](https://github.com/magicant/yash) | A POSIX-compliant command line shell | POSIX shell with builtin prediction support | Lin/mac | [magicant/yash](https://github.com/magicant/yash) | — | GPL-2.0 | ✅ |
| [zsh](https://www.zsh.org) | Powerful shell with scripting language | Feature-rich shell with powerful completion system | Lin/mac | [zsh-users/zsh](https://github.com/zsh-users/zsh) | — | MIT-like | ✅ |
| [fz](https://github.com/changyuheng/fz) | Seamless fuzzy completion for z | Combines z and fzf for ultimate navigation | Lin/mac | [changyuheng/fz](https://github.com/changyuheng/fz) | — | MIT | ✅ |
| [aliasme](https://github.com/Jintin/aliasme) | alias helper to change directory quickly | Simple tool to create navigation aliases | All | [Jintin/aliasme](https://github.com/Jintin/aliasme) | — | MIT | ✅ |

---

## File & Directory Management

Better alternatives to `ls`, `cat`, `find`, `du`, and `df` — with color, tree views, previews, and human-readable output.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [bat](https://github.com/sharkdp/bat) | `cat` with syntax highlighting and Git integration | Displays file contents with syntax highlighting for hundreds of languages, line numbers, and inline git diff markers. Supports paging and acts as a drop-in replacement for `cat` in most scripts. | All | [sharkdp/bat](https://github.com/sharkdp/bat) | ![GitHub Release](https://img.shields.io/github/v/release/sharkdp/bat?label=) | Apache-2.0/MIT | ✅ |
| [eza](https://eza.rocks/) | Modern, colorful replacement for `ls` | Colorized `ls` with icons, tree view (`--tree`), git status per file, extended attributes, and human-readable output by default. Actively maintained fork of the unmaintained `exa`. | All | [eza-community/eza](https://github.com/eza-community/eza) | ![GitHub Release](https://img.shields.io/github/v/release/eza-community/eza?label=) | EUPL-1.2 | ✅ |
| [fd](https://github.com/sharkdp/fd) | Fast and user-friendly alternative to `find` | Simpler syntax, respects `.gitignore` by default, colorized output, and significantly faster than GNU `find` on most patterns. | All | [sharkdp/fd](https://github.com/sharkdp/fd) | ![GitHub Release](https://img.shields.io/github/v/release/sharkdp/fd?label=) | Apache-2.0/MIT | ✅ |
| [dust](https://github.com/bootandy/dust) | Intuitive disk usage with tree visualization | Shows directory sizes as a weighted tree so you immediately see which subdirectory consumes the most space. No configuration needed for useful output. | All | [bootandy/dust](https://github.com/bootandy/dust) | ![GitHub Release](https://img.shields.io/github/v/release/bootandy/dust?label=) | Apache-2.0 | ✅ |
| [duf](https://github.com/muesli/duf) | Better `df` — disk usage/free with a pretty table | Shows mounted filesystems in a colorized, grouped table with used, free, and total sizes. Groups by type: local drives, network mounts, and special filesystems. | All | [muesli/duf](https://github.com/muesli/duf) | ![GitHub Release](https://img.shields.io/github/v/release/muesli/duf?label=) | MIT | ✅ |
| [broot](https://dystroy.org/broot/) | Interactive directory tree with fuzzy search | Navigate large directory trees interactively. Type to fuzzy-search, press Enter to open files, and run verbs (git diff, rm, cp) without leaving the TUI. | All | [Canop/broot](https://github.com/Canop/broot) | ![GitHub Release](https://img.shields.io/github/v/release/Canop/broot?label=) | MIT | ✅ |
| [ranger](https://ranger.github.io/) | VIM-inspired terminal file manager | Three-column file browser with Vim keybindings, file preview, bulk renaming, and plugin support. Highly scriptable via Python. | Lin/mac | [ranger/ranger](https://github.com/ranger/ranger) | ![GitHub Release](https://img.shields.io/github/v/release/ranger/ranger?label=) | GPL-3.0 | ✅ |
| [yazi](https://yazi-rs.github.io/) | Blazing fast terminal file manager written in Rust | Async I/O, image preview (via Kitty Graphics Protocol/Sixel), archive browsing, a Lua plugin API, and a polished default UI. Modern, faster successor to ranger. | All | [sxyazi/yazi](https://github.com/sxyazi/yazi) | ![GitHub Release](https://img.shields.io/github/v/release/sxyazi/yazi?label=) | MIT | ✅ |
| [lsd](https://github.com/lsd-rs/lsd) | LSDeluxe — another modern `ls` replacement | Colorized directory listing with icons, tree view, and git status integration. Similar to eza/exa but with a different aesthetic and icon set. | All | [lsd-rs/lsd](https://github.com/lsd-rs/lsd) | ![GitHub Release](https://img.shields.io/github/v/release/lsd-rs/lsd?label=) | Apache-2.0 | ✅ |
| [tree](http://mama.indstate.edu/users/ice/tree/) | Display directory structure as a tree | The classic and ubiquitous tool for displaying directory trees | All | — | — | GPL-2.0 | ✅ |
| [vifm](https://vifm.info/) | Vim-like terminal file manager | Two-pane file manager with Vim keybindings and extensive customization | Lin/mac | [vifm/vifm](https://github.com/vifm/vifm) | — | GPL-2.0 | ✅ |
| [nnn](https://github.com/jarun/nnn) | The unorthodox terminal file manager | Minimal, blazingly fast with plugins, context-aware navigation | All | [jarun/nnn](https://github.com/jarun/nnn) | ![GitHub Release](https://img.shields.io/github/v/release/jarun/nnn?label=) | BSD-2-Clause | ✅ |
| [lf](https://github.com/gokcehan/lf) | Terminal file manager written in Go | Fast, lightweight file manager inspired by ranger | All | [gokcehan/lf](https://github.com/gokcehan/lf) | ![GitHub Release](https://img.shields.io/github/v/release/gokcehan/lf?label=) | MIT | ✅ |
| [rsync](https://rsync.samba.org/) | Fast incremental file transfer tool | Efficiently syncs files locally or to remote systems via SSH. The gold standard for backups. | Lin/mac | [RsyncProject/rsync](https://github.com/RsyncProject/rsync) | — | GPL-3.0 | ✅ |
| [parallel](https://www.gnu.org/software/parallel/) | Execute jobs in parallel using one or more CPU cores | Essential for batch processing, runs commands in parallel across multiple cores | All | — | — | GPL-3.0 | ✅ |
| [jc](https://github.com/kellyjonbrazil/jc) | Convert CLI output to JSON | Converts output from common Unix commands (ls, ps, dig, etc.) to structured JSON | All | [kellyjonbrazil/jc](https://github.com/kellyjonbrazil/jc) | ![GitHub Release](https://img.shields.io/github/v/release/kellyjonbrazil/jc?label=) | MIT | ✅ |
| [ncdu](https://dev.yorhel.nl/ncdu) | NCurses Disk Usage | Fast interactive disk usage analyzer with ncurses interface | Lin/mac | — | — | MIT | ✅ |
| [diskonaut](https://github.com/imsnif/diskonaut) | Disk space navigator | Terminal disk usage explorer with intuitive visualization | All | [imsnif/diskonaut](https://github.com/imsnif/diskonaut) | — | MIT | ✅ |
| [dua-cli](https://github.com/Byron/dua-cli) | Disk usage analyzer | View disk space usage and delete unwanted data fast | All | [Byron/dua-cli](https://github.com/Byron/dua-cli) | ![GitHub Release](https://img.shields.io/github/v/release/Byron/dua-cli?label=) | MIT | ✅ |
| [trash-cli](https://github.com/sindresorhus/trash-cli) | Move files and directories to the trash | Safer alternative to rm, moves files to trash | All | [sindresorhus/trash-cli](https://github.com/sindresorhus/trash-cli) | — | MIT | ✅ |
| [renameutils](https://www.nongnu.org/renameutils/) | Mass renaming in your editor | Edit filenames in your favorite text editor | All | — | — | GPL-3.0 | ✅ |
| [entr](https://github.com/eradman/entr) | Run an arbitrary command when files change | Simple file watcher that runs commands on file modifications | Lin/mac | [eradman/entr](https://github.com/eradman/entr) | — | ISC | ✅ |
| [f2](https://github.com/ayoisaiah/f2) | Cross-platform tool for fast, safe batch renaming | Powerful batch renaming with preview and undo | All | [ayoisaiah/f2](https://github.com/ayoisaiah/f2) | ![GitHub Release](https://img.shields.io/github/v/release/ayoisaiah/f2?label=) | MIT | ✅ |

---

## Search & Text Processing

Tools for searching, filtering, transforming, and processing text, JSON, CSV, YAML, and more.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [ripgrep (rg)](https://github.com/BurntSushi/ripgrep) | The fastest `grep` in the world | Recursively searches directories using regex, respects `.gitignore`, written in Rust. Combines the usability of The Silver Searcher with the raw speed of GNU grep. | All | [BurntSushi/ripgrep](https://github.com/BurntSushi/ripgrep) | ![GitHub Release](https://img.shields.io/github/v/release/BurntSushi/ripgrep?label=) | Unlicense/MIT | ✅ |
| [jq](https://jqlang.github.io/jq/) | Lightweight JSON processor and query language | Slice, filter, map, and transform JSON structures with a domain-specific language. Essential for API debugging and shell scripting. | All | [jqlang/jq](https://github.com/jqlang/jq) | — | MIT | ✅ |
| [yq](https://mikefarah.gitbook.io/yq/) | `jq`-compatible processor for YAML, TOML, XML, CSV | Process YAML files the same way jq processes JSON. Invaluable in CI/CD pipelines and config management. | All | [mikefarah/yq](https://github.com/mikefarah/yq) | ![GitHub Release](https://img.shields.io/github/v/release/mikefarah/yq?label=) | MIT | ✅ |
| [fx](https://fx.wtf/) | Interactive JSON viewer and processor | Opens any JSON in a collapsible, interactive tree. Navigate with keyboard, execute JavaScript expressions inline. | All | [antonmedv/fx](https://github.com/antonmedv/fx) | ![GitHub Release](https://img.shields.io/github/v/release/antonmedv/fx?label=) | MIT | ✅ |
| [miller (mlr)](https://miller.readthedocs.io/) | `awk`/`sed`/`cut`/`sort` for CSV, JSON, TSV | SQL-like verbs (select, filter, join, sort, aggregate) with fully streaming I/O. Handles name-indexed data instead of numeric fields. | All | [johnkerl/miller](https://github.com/johnkerl/miller) | — | BSD-2-Clause | ✅ |
| [csvlens](https://github.com/YS-L/csvlens) | Pager and explorer for CSV files | Navigate and search CSV files interactively with vim-like keybindings, column-aware scrolling, and regex filtering. | All | [YS-L/csvlens](https://github.com/YS-L/csvlens) | ![GitHub Release](https://img.shields.io/github/v/release/YS-L/csvlens?label=) | MIT | ✅ |
| [gron](https://github.com/tomnomnom/gron) | Make JSON greppable | Flattens JSON into discrete assignment statements so you can grep it, then transforms it back. | All | [tomnomnom/gron](https://github.com/tomnomnom/gron) | — | MIT | ✅ |
| [sd](https://github.com/chmln/sd) | Intuitive `sed` alternative for find-and-replace | Simpler regex syntax, string literals by default, operates on files or stdin. Modern sed for the rest of us. | All | [chmln/sd](https://github.com/chmln/sd) | ![GitHub Release](https://img.shields.io/github/v/release/chmln/sd?label=) | MIT | ✅ |
| [hexyl](https://github.com/sharkdp/hexyl) | Modern hex viewer for the terminal | Colorized hex dump with ASCII representation, automatic color-coding of NULL bytes, printable ASCII, and non-ASCII. | All | [sharkdp/hexyl](https://github.com/sharkdp/hexyl) | ![GitHub Release](https://img.shields.io/github/v/release/sharkdp/hexyl?label=) | Apache-2.0/MIT | ✅ |
| [grex](https://github.com/pemistahl/grex) | Generate regex automatically from test cases | Feed it example strings and it infers a matching regex pattern. Reverse-engineering regex from examples. | All | [pemistahl/grex](https://github.com/pemistahl/grex) | ![GitHub Release](https://img.shields.io/github/v/release/pemistahl/grex?label=) | Apache-2.0 | ✅ |
| [lnav](https://lnav.org/) | Advanced log file browser with SQL queries | Tail, search, and navigate multiple log files simultaneously. Run SQL queries against your logs. Auto-detects log formats. | Lin/mac | [tstack/lnav](https://github.com/tstack/lnav) | — | BSD-2-Clause | ✅ |
| [ag (The Silver Searcher)](https://geoff.greer.fm/ag/) | Fast code-searching tool, predecessor to ripgrep | Faster than ack, respects .gitignore, searches compressed files | All | [ggreer/the_silver_searcher](https://github.com/ggreer/the_silver_searcher) | — | Apache-2.0 | ✅ |
| [ack](https://beyondgrep.com/) | Grep-like search tool optimized for programmers | Designed for searching codebases, ignores VCS directories by default | All | [beyondgrep/ack3](https://github.com/beyondgrep/ack3) | — | Artistic-2.0 | ✅ |
| [jless](https://jless.io/) | Command-line JSON pager with collapsible trees | Interactive JSON viewer with folding, searching, and keyboard navigation | All | [PaulJuliusMartinez/jless](https://github.com/PaulJuliusMartinez/jless) | — | MIT | ✅ |
| [xsv](https://github.com/BurntSushi/xsv) | Fast CSV command-line toolkit | Index, slice, select columns, search, sort, and join CSV files blazingly fast | All | [BurntSushi/xsv](https://github.com/BurntSushi/xsv) | — | Unlicense/MIT | ✅ |
| [dasel](https://daseldocs.tomwright.me/) | Query and modify structured data | Works with JSON, YAML, TOML, XML, CSV using a single unified syntax | All | [TomWright/dasel](https://github.com/TomWright/dasel) | ![GitHub Release](https://img.shields.io/github/v/release/TomWright/dasel?label=) | MIT | ✅ |
| [dyff](https://github.com/homeport/dyff) | YAML diff tool | Human-friendly diff tool for YAML files | All | [homeport/dyff](https://github.com/homeport/dyff) | ![GitHub Release](https://img.shields.io/github/v/release/homeport/dyff?label=) | MIT | ✅ |
| [q](http://harelba.github.io/q/) | Execution of SQL-like queries on CSV/TSV | Run SQL queries directly on CSV and TSV files | All | [harelba/q](https://github.com/harelba/q) | — | GPL-3.0 | ✅ |
| [figlet](http://www.figlet.org/) | Creates large text out of ASCII characters | Classic ASCII art text generator | Lin/mac | — | — | BSD-3-Clause | ✅ |
| [fselect](https://github.com/jhspetersson/fselect) | Find files with SQL-like queries | Search files using SQL WHERE/GROUP BY syntax | All | [jhspetersson/fselect](https://github.com/jhspetersson/fselect) | — | Apache-2.0/MIT | ✅ |
| [skim](https://github.com/lotabout/skim) | A general fuzzy finder written in Rust | Alternative to fzf, fast and feature-rich | All | [lotabout/skim](https://github.com/lotabout/skim) | — | MIT | ✅ |
| [ast-grep](https://github.com/ast-grep/ast-grep) | A tool for code structural search, linting and rewriting | Search code by AST patterns, not just text | All | [ast-grep/ast-grep](https://github.com/ast-grep/ast-grep) | ![GitHub Release](https://img.shields.io/github/v/release/ast-grep/ast-grep?label=) | MIT | ✅ |
| [visidata](https://github.com/saulpw/visidata) | A terminal spreadsheet multitool | Explore and arrange data in tabular format interactively | All | [saulpw/visidata](https://github.com/saulpw/visidata) | — | GPL-3.0 | ✅ |
| [xmlstarlet](http://xmlstar.sourceforge.net/) | Old but powerful command-line XML tool | Format, filter, and manipulate XML from command line | All | — | — | MIT | ✅ |

---

## System Monitoring & Performance

Tools for monitoring processes, system resources, network, and performance in real-time.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [htop](https://htop.dev/) | The classic interactive process viewer | Colorized, interactive replacement for `top` with tree view, CPU/memory/swap meters, and process management. | Lin/mac | [htop-dev/htop](https://github.com/htop-dev/htop) | — | GPL-2.0 | ✅ |
| [btop++](https://github.com/aristocratos/btop) | Beautiful resource monitor with GPU support | Shows CPU, memory, disk, network, and processes with gorgeous visualization. Modern C++ rewrite of bashtop with GPU metrics. | Lin/mac | [aristocratos/btop](https://github.com/aristocratos/btop) | ![GitHub Release](https://img.shields.io/github/v/release/aristocratos/btop?label=) | Apache-2.0 | ✅ |
| [bottom (btm)](https://clementtsang.github.io/bottom/) | Cross-platform system monitor written in Rust | Genuine Windows support, customizable widgets, multiple process sorting modes, and tree view. | All | [ClementTsang/bottom](https://github.com/ClementTsang/bottom) | ![GitHub Release](https://img.shields.io/github/v/release/ClementTsang/bottom?label=) | MIT | ✅ |
| [glances](https://nicolargo.github.io/glances/) | "Eye on your system" — cross-platform monitoring | Python-based with built-in web UI, exports to InfluxDB/Prometheus, shows CPU/GPU/Network/Disk all at once. | All | [nicolargo/glances](https://github.com/nicolargo/glances) | — | LGPL-3.0 | ✅ |
| [ctop](https://ctop.sh/) | `top`-like TUI for Docker containers | Real-time CPU, memory, and network metrics for containers with interactive management (start/stop/inspect). | Lin/mac | [bcicen/ctop](https://github.com/bcicen/ctop) | — | MIT | ✅ |
| [procs](https://github.com/dalance/procs) | Modern replacement for `ps` | Colorized process list with human-readable sizes, tree view, search, and watch mode. | All | [dalance/procs](https://github.com/dalance/procs) | ![GitHub Release](https://img.shields.io/github/v/release/dalance/procs?label=) | MIT | ✅ |
| [bandwhich](https://github.com/imsnif/bandwhich) | Network utilization broken down by process | Shows which process is using bandwidth in real-time, organized by connection and remote host. | All | [imsnif/bandwhich](https://github.com/imsnif/bandwhich) | — | MIT | ✅ |
| [gotop](https://github.com/xxxserxxx/gotop) | Graphical terminal activity monitor written in Go | Colorful graphs for CPU, memory, disk, network, and temperature sensors. | All | [xxxserxxx/gotop](https://github.com/xxxserxxx/gotop) | — | MIT | ✅ |
| [zenith](https://github.com/bvaisvil/zenith) | Cross-platform system monitor with zoom | Interactive charts with zoom and pan, disk I/O, process tree, and GPU metrics. | Lin/mac | [bvaisvil/zenith](https://github.com/bvaisvil/zenith) | — | MIT | ✅ |
| [iotop](https://github.com/Tomas-M/iotop) | Disk I/O monitor per process | Shows which processes are performing disk reads/writes with bandwidth usage. | Lin | [Tomas-M/iotop](https://github.com/Tomas-M/iotop) | — | GPL-2.0 | ✅ |
| [iftop](http://www.ex-parrot.com/~pdw/iftop/) | Real-time network bandwidth monitor | Shows bandwidth usage per network connection with source and destination. | Lin/mac | — | — | GPL-2.0 | ✅ |
| [atop](https://www.atoptool.nl) | ASCII full-screen performance monitor | Reports activity of all processes, comprehensive system and process metrics, logs to disk. | Lin | — | — | GPL-2.0 | ✅ |
| [bmon](https://github.com/tgraf/bmon) | Real-time network bandwidth monitor and rate estimator | Portable bandwidth monitor with configurable input/output modules. | Lin/mac | [tgraf/bmon](https://github.com/tgraf/bmon) | — | BSD-2-Clause/MIT | ✅ |
| [fastfetch](https://github.com/fastfetch-cli/fastfetch) | Lightning-fast system info with ASCII art | System information tool like neofetch but significantly faster. | All | [fastfetch-cli/fastfetch](https://github.com/fastfetch-cli/fastfetch) | ![GitHub Release](https://img.shields.io/github/v/release/fastfetch-cli/fastfetch?label=) | MIT | ✅ |
| [mtr](https://github.com/traviscross/mtr) | The functionality of 'traceroute' and 'ping' combined | Network diagnostic tool combining ping and traceroute. | Lin/mac | [traviscross/mtr](https://github.com/traviscross/mtr) | — | GPL-2.0 | ✅ |
| [powertop](https://github.com/fenrus75/powertop) | Battery/Power usage and device stats monitoring tool | Diagnose power consumption issues on Linux. | Lin | [fenrus75/powertop](https://github.com/fenrus75/powertop) | — | GPL-2.0 | ✅ |
| [prettyping](https://github.com/denilsonsa/prettyping) | Making the output of `ping` prettier | Wrapper around ping with colorful output and sparklines. | Lin/mac | [denilsonsa/prettyping](https://github.com/denilsonsa/prettyping) | — | MIT | ✅ |

---

## Network & Web Tools

Tools for HTTP testing, networking, file transfer, and web services.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [HTTPie](https://httpie.io/) | Human-friendly HTTP client | Intuitive syntax for crafting HTTP requests with syntax highlighting, JSON support, and session persistence. | All | [httpie/cli](https://github.com/httpie/cli) | ![GitHub Release](https://img.shields.io/github/v/release/httpie/cli?label=) | BSD-3-Clause | ✅ |
| [xh](https://github.com/ducaale/xh) | Fast HTTPie-compatible HTTP client in Rust | Better suited for scripting than HTTPie, with similar syntax and faster execution. | All | [ducaale/xh](https://github.com/ducaale/xh) | ![GitHub Release](https://img.shields.io/github/v/release/ducaale/xh?label=) | MIT | ✅ |
| [posting](https://posting.sh/) | Modern TUI HTTP client | API testing in the terminal with full TUI interface and collections support. | All | [darrenburns/posting](https://github.com/darrenburns/posting) | — | Apache-2.0 | ✅ |
| [curl](https://curl.se/) | The universal URL transfer tool | Pre-installed on virtually all systems. Supports HTTP, HTTPS, FTP, and dozens more protocols. | All | [curl/curl](https://github.com/curl/curl) | — | curl | ✅ |
| [nmap](https://nmap.org/) | Network exploration and security auditing | The most widely used network scanner for discovery, port scanning, and OS detection. | All | [nmap/nmap](https://github.com/nmap/nmap) | — | GPL-2.0 | ✅ |
| [RustScan](https://github.com/RustScan/RustScan) | Find all open ports in seconds | Scans all 65K ports in ~8 seconds, then hands off to nmap for detailed probing. Written in Rust. | All | [RustScan/RustScan](https://github.com/RustScan/RustScan) | ![GitHub Release](https://img.shields.io/github/v/release/RustScan/RustScan?label=) | GPL-3.0 | ✅ |
| [trippy](https://trippy.cli.rs/) | Modern `traceroute` + `ping` TUI | Real-time animated TUI showing latency, packet loss, hop-by-hop metrics with ICMP/UDP/TCP protocols. | All | [fujiapple852/trippy](https://github.com/fujiapple852/trippy) | ![GitHub Release](https://img.shields.io/github/v/release/fujiapple852/trippy?label=) | Apache-2.0 | ✅ |
| [gping](https://github.com/orf/gping) | `ping` with a live graph in the terminal | Visualize ping times as a real-time graph, can ping multiple hosts simultaneously. | All | [orf/gping](https://github.com/orf/gping) | ![GitHub Release](https://img.shields.io/github/v/release/orf/gping?label=) | MIT | ✅ |
| [doggo](https://doggo.mrkaran.dev/) | Modern DNS client with colorized output | Query DNS servers with support for DOH, DOT, DOQ protocols and JSON output. | All | [mr-karan/doggo](https://github.com/mr-karan/doggo) | ![GitHub Release](https://img.shields.io/github/v/release/mr-karan/doggo?label=) | GPL-3.0 | ✅ |
| [oha](https://github.com/hatoo/oha) | HTTP load generator with a real-time TUI | Blazingly fast HTTP benchmarking tool with live statistics display. | All | [hatoo/oha](https://github.com/hatoo/oha) | ![GitHub Release](https://img.shields.io/github/v/release/hatoo/oha?label=) | MIT | ✅ |
| [aria2](https://aria2.github.io/) | Lightweight multi-protocol download utility | Supports HTTP, HTTPS, FTP, BitTorrent with multi-connection downloads and RPC interface. | All | [aria2/aria2](https://github.com/aria2/aria2) | — | GPL-2.0 | ✅ |
| [streamlink](https://streamlink.github.io/) | Stream video from 80+ sites to any local player | Extract video streams from sites and pipe to VLC, mpv, or any player. Alternative to youtube-dl for live streams. | All | [streamlink/streamlink](https://github.com/streamlink/streamlink) | — | BSD-2-Clause | ✅ |
| [termshark](https://termshark.io/) | Terminal UI for tshark | Wireshark in the terminal — full packet capture and analysis with TUI. | Lin/mac | [gcla/termshark](https://github.com/gcla/termshark) | — | MIT | ✅ |
| [wget](https://www.gnu.org/software/wget/) | Non-interactive network downloader | Pre-installed on most Unix systems, perfect for scripting downloads and mirroring sites. | All | — | — | GPL-3.0 | ✅ |
| [wrk](https://github.com/wg/wrk) | Modern HTTP benchmarking tool | Multi-threaded HTTP load generator capable of generating significant load. | Lin/mac | [wg/wrk](https://github.com/wg/wrk) | — | Apache-2.0 | ✅ |
| [hey](https://github.com/rakyll/hey) | HTTP load generator in Go | Simpler alternative to wrk with better out-of-the-box experience. | All | [rakyll/hey](https://github.com/rakyll/hey) | — | Apache-2.0 | ✅ |
| [httpx](https://github.com/projectdiscovery/httpx) | Fast multi-purpose HTTP toolkit | Probes hosts for active HTTP/HTTPS services with screenshot capabilities. | All | [projectdiscovery/httpx](https://github.com/projectdiscovery/httpx) | ![GitHub Release](https://img.shields.io/github/v/release/projectdiscovery/httpx?label=) | MIT | ✅ |
| [websocat](https://github.com/vi/websocat) | Netcat-like tool for WebSockets | Connect to WebSocket servers, send/receive messages, proxy connections. | All | [vi/websocat](https://github.com/vi/websocat) | — | MIT | ✅ |
| [caddy](https://caddyserver.com/) | Fast web server with automatic HTTPS | Modern web server with automatic TLS certificates from Let's Encrypt. | All | [caddyserver/caddy](https://github.com/caddyserver/caddy) | ![GitHub Release](https://img.shields.io/github/v/release/caddyserver/caddy?label=) | Apache-2.0 | ✅ |
| [miniserve](https://github.com/svenstaro/miniserve) | Serve files via HTTP instantly | Single-command file server with upload support, perfect for quick file sharing. | All | [svenstaro/miniserve](https://github.com/svenstaro/miniserve) | ![GitHub Release](https://img.shields.io/github/v/release/svenstaro/miniserve?label=) | MIT | ✅ |
| [croc](https://github.com/schollz/croc) | Securely transfer files between computers | End-to-end encrypted file transfer with relay server support. | All | [schollz/croc](https://github.com/schollz/croc) | ![GitHub Release](https://img.shields.io/github/v/release/schollz/croc?label=) | MIT | ✅ |
| [s3cmd](https://github.com/s3tools/s3cmd) | Fully-Featured S3 client | Command-line tool for Amazon S3 and S3-compatible storage. | All | [s3tools/s3cmd](https://github.com/s3tools/s3cmd) | — | GPL-2.0 | ✅ |
| [curlie](https://github.com/rs/curlie) | A curl frontend with the ease of use of HTTPie | Best of both worlds: curl's power with HTTPie's UX. | All | [rs/curlie](https://github.com/rs/curlie) | — | MIT | ✅ |
| [ATAC](https://github.com/Julien-cpsn/ATAC) | A feature-full TUI API client made in Rust | Full-featured API testing tool in the terminal. | All | [Julien-cpsn/ATAC](https://github.com/Julien-cpsn/ATAC) | — | MIT | ✅ |
| [HTTP Prompt](https://github.com/eliangcs/http-prompt) | Interactive HTTP client with autocomplete | Interactive shell for HTTP with intelligent completions. | All | [eliangcs/http-prompt](https://github.com/eliangcs/http-prompt) | — | MIT | ✅ |
| [gotty](https://github.com/yudai/gotty) | Share your terminal as a web application | Access your terminal via web browser. | All | [yudai/gotty](https://github.com/yudai/gotty) | — | MIT | ✅ |
| [tmate](https://tmate.io/) | Instant terminal (tmux) sharing | Share your terminal session instantly via SSH. | Lin/mac | [tmate-io/tmate](https://github.com/tmate-io/tmate) | — | ISC | ✅ |
| [mosh](https://mosh.org/) | Remote SSH client that allows roaming | SSH replacement that handles intermittent connectivity and roaming. | All | [mobile-shell/mosh](https://github.com/mobile-shell/mosh) | — | GPL-3.0 | ✅ |
| [xxh](https://github.com/xxh/xxh) | Bring your favorite shell wherever you go through SSH | Portable shell environment over SSH. | All | [xxh/xxh](https://github.com/xxh/xxh) | — | BSD-2-Clause | ✅ |
| [sshuttle](https://github.com/sshuttle/sshuttle) | Transparent proxy server that works as a poor man's VPN | VPN over SSH without configuration. | All | [sshuttle/sshuttle](https://github.com/sshuttle/sshuttle) | — | LGPL-2.1 | ✅ |
| [transmission-cli](https://transmissionbt.com) | Torrent client for your command line | Command-line BitTorrent client. | All | [transmission/transmission](https://github.com/transmission/transmission) | — | GPL-2.0 | ✅ |
| [webtorrent-cli](https://github.com/feross/webtorrent-cli) | Streaming torrent client | Stream torrents to your terminal or media player. | All | [webtorrent/webtorrent-cli](https://github.com/webtorrent/webtorrent-cli) | — | MIT | ✅ |

---

## Downloaders & Media

Tools for downloading videos, music, and content from the internet from multiple platforms.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [yt-dlp](https://github.com/yt-dlp/yt-dlp) | Download video and audio from 1000+ sites | The most actively maintained downloader, fork of youtube-dl with additional features and site support. | All | [yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp) | ![GitHub Release](https://img.shields.io/github/v/release/yt-dlp/yt-dlp?label=) | Unlicense | ✅ |
| [annie/lux](https://github.com/iawia002/lux) | Fast video downloader written in Go | Supports YouTube, Bilibili, Twitter, Instagram, and 80+ sites with concurrent downloads. | All | [iawia002/lux](https://github.com/iawia002/lux) | ![GitHub Release](https://img.shields.io/github/v/release/iawia002/lux?label=) | MIT | ✅ |
| [spotdl](https://spotdl.readthedocs.io/) | Download Spotify music with proper metadata | Downloads music from YouTube with Spotify metadata. No Spotify Premium required. | All | [spotDL/spotify-downloader](https://github.com/spotDL/spotify-downloader) | ![GitHub Release](https://img.shields.io/github/v/release/spotDL/spotify-downloader?label=) | MIT | ✅ |
| [gallery-dl](https://github.com/mikf/gallery-dl) | Download image galleries from 200+ sites | Download from DeviantArt, Pixiv, Reddit, Twitter, Instagram, and many more image sites. | All | [mikf/gallery-dl](https://github.com/mikf/gallery-dl) | — | GPL-2.0 | ✅ |
| [you-get](https://you-get.org/) | Download media from a wide range of sites | Covers unique Asian platforms like Bilibili, Youku, and Niconico. | All | [soimort/you-get](https://github.com/soimort/you-get) | — | MIT | ✅ |
| [megatools](https://megatools.megous.com/) | Command-line client for MEGA cloud storage | Download and upload files to MEGA.nz from terminal. | Lin/mac | [megous/megatools](https://github.com/megous/megatools) | — | GPL-2.0 | ✅ |
| [rclone](https://rclone.org/) | Rsync for cloud storage | Sync files to/from 40+ cloud providers (Google Drive, S3, Dropbox, etc.). | All | [rclone/rclone](https://github.com/rclone/rclone) | ![GitHub Release](https://img.shields.io/github/v/release/rclone/rclone?label=) | MIT | ✅ |
| [youtube-dl](https://github.com/ytdl-org/youtube-dl) | Download videos from YouTube.com and other sites | Original downloader, now superseded by yt-dlp but still maintained. | All | [ytdl-org/youtube-dl](https://github.com/ytdl-org/youtube-dl) | — | Unlicense | ✅ |

---

## Books & E-books

Download, manage, read, and convert e-books from the terminal.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [calibre](https://calibre-ebook.com/) | Complete e-book management suite with powerful CLI | The definitive e-book toolkit. CLI includes `ebook-convert` (100+ format conversions: EPUB, MOBI, AZW3, PDF, FB2…), `calibredb` (manage your library from scripts), and `fetch-ebook-metadata` (auto-fill metadata). | All | [kovidgoyal/calibre](https://github.com/kovidgoyal/calibre) | ![GitHub Release](https://img.shields.io/github/v/release/kovidgoyal/calibre?label=) | GPL-3.0 | ✅ |
| [libgen-cli](https://github.com/ciehanski/libgen-cli) | Search and download books from Library Genesis | Search LibGen's catalog by title, author, or ISBN and download EPUB/PDF directly. Supports fiction, non-fiction, and scientific articles. | All | [ciehanski/libgen-cli](https://github.com/ciehanski/libgen-cli) | — | MIT | ✅ |
| [monolith](https://github.com/Y2Z/monolith) | Save complete web pages as a single offline HTML file | Embeds all CSS, images, fonts, and scripts into one self-contained file. Perfect for archiving articles and documentation for offline reading. | All | [Y2Z/monolith](https://github.com/Y2Z/monolith) | ![GitHub Release](https://img.shields.io/github/v/release/Y2Z/monolith?label=) | CC0-1.0 | ✅ |
| [readability-cli](https://gitlab.com/gardenappl/readability-cli) | Extract clean, clutter-free text from any URL | Uses Mozilla's Readability algorithm (same as Firefox Reader View) to strip ads, nav, and clutter — outputs clean text, HTML, or Markdown. | All | [gardenappl/readability-cli](https://gitlab.com/gardenappl/readability-cli) | — | GPL-3.0 | ✅ |
| [epy](https://github.com/wustho/epy) | Feature-rich terminal EPUB/e-book reader | Read EPUB, FB2, Mobi, and AZW3 in-terminal with chapter navigation, bookmarks, highlights, and inline images in supported terminals. | All | [wustho/epy](https://github.com/wustho/epy) | — | GPL-3.0 | ✅ |
| [kepubify](https://pgaskin.net/kepubify/) | Bulk convert EPUB files to Kobo KEPUB format | Fast batch EPUB→KEPUB converter that can process entire libraries at once. Essential for Kobo e-reader users. | All | [pgaskin/kepubify](https://github.com/pgaskin/kepubify) | ![GitHub Release](https://img.shields.io/github/v/release/pgaskin/kepubify?label=) | MIT | ✅ |
| [fb2converter](https://github.com/rupor-github/fb2converter) | Convert FB2 Russian e-book format to EPUB/MOBI | Full-featured FB2 converter popular in Russian and Eastern European digital book ecosystems. Handles embedded images, metadata, and footnotes. | All | [rupor-github/fb2converter](https://github.com/rupor-github/fb2converter) | — | GPL-3.0 | ✅ |

---

## Media Processing

Tools for processing images, videos, audio, QR codes, and other media.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [qrencode](https://fukuchi.org/works/qrencode/) | Generate QR codes in the terminal | Creates QR codes as UTF-8 block characters or image files. | Lin/mac | — | — | LGPL-2.1 | ✅ |
| [FFmpeg](https://ffmpeg.org/) | The Swiss Army knife of audio/video processing | Convert, compress, trim, transcode, extract audio, capture screen, and infinitely more media operations. | All | [FFmpeg/FFmpeg](https://github.com/FFmpeg/FFmpeg) | — | LGPL-2.1/GPL-2.0 | ✅ |
| [ImageMagick](https://imagemagick.org/) | Create, edit, and convert images from the CLI | Batch-process thousands of images — resize, rotate, crop, colorize, apply effects. | All | [ImageMagick/ImageMagick](https://github.com/ImageMagick/ImageMagick) | — | Apache-2.0 | ✅ |
| [chafa](https://hpjansson.org/chafa/) | Render images and video as text art in the terminal | Displays images inline in terminals supporting Sixel, Kitty graphics, or Unicode block art. | Lin/mac | [hpjansson/chafa](https://github.com/hpjansson/chafa) | — | LGPL-3.0 | ✅ |
| [vhs](https://github.com/charmbracelet/vhs) | Record terminal sessions as GIFs from a script | Scriptable terminal recorder — write reproducible demo GIFs as code. | All | [charmbracelet/vhs](https://github.com/charmbracelet/vhs) | ![GitHub Release](https://img.shields.io/github/v/release/charmbracelet/vhs?label=) | MIT | ✅ |
| [asciinema](https://asciinema.org/) | Record and share terminal sessions as text | Records terminal sessions as text (not video) for lightweight, searchable, copyable playback. | Lin/mac | [asciinema/asciinema](https://github.com/asciinema/asciinema) | — | GPL-3.0 | ✅ |
| [timg](https://github.com/hzeller/timg) | View images and video directly in the terminal | Display images and videos inline in terminals supporting Sixel or Kitty graphics protocol. | Lin/mac | [hzeller/timg](https://github.com/hzeller/timg) | — | GPL-2.0 | ✅ |
| [ZBar / zbarimg](https://zbar.sourceforge.net/) | Decode QR codes and barcodes from images or camera | Read QR codes and barcodes from files or webcam. | Lin/mac | — | — | LGPL-2.1 | ✅ |
| [gifski](https://gif.ski/) | Highest-quality GIF encoder | Converts videos to GIFs with incredible quality using pngquant's algorithm. | All | [ImageOptim/gifski](https://github.com/ImageOptim/gifski) | — | AGPL-3.0 | ✅ |
| [jp2a](https://csl.name/jp2a/) | Convert images to ASCII art | JPEG/PNG to ASCII art converter. | Lin/mac | [Talinx/jp2a](https://github.com/Talinx/jp2a) | — | GPL-2.0 | ✅ |
| [Beets](https://github.com/beetbox/beets) | Music library manager and MusicBrainz tagger | Organize and tag your music library with metadata from MusicBrainz. | All | [beetbox/beets](https://github.com/beetbox/beets) | — | MIT | ✅ |
| [imgp](https://github.com/jarun/imgp) | Blazing fast batch image resizer and rotator | Multi-threaded image resizing with smart optimization compression. | All | [jarun/imgp](https://github.com/jarun/imgp) | — | GPL-3.0 | ✅ |
| [editly](https://github.com/mifi/editly) | Declarative video editing | Edit videos programmatically via JSON configuration. | All | [mifi/editly](https://github.com/mifi/editly) | — | MIT | ✅ |

---

## Terminal Music & Audio Players

Music players and audio tools for the terminal.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [mpv](https://mpv.io/) | Minimalist yet powerful video and audio player | Highly scriptable with Lua plugins, hardware acceleration, and extensive format support. | All | [mpv-player/mpv](https://github.com/mpv-player/mpv) | — | GPL-2.0 | ✅ |
| [cmus](https://cmus.github.io/) | Small, fast, and powerful console music player | Lightweight music player with vim-like keybindings and powerful playlist management. | Lin/mac | [cmus/cmus](https://github.com/cmus/cmus) | — | GPL-2.0 | ✅ |
| [musikcube](https://musikcube.com/) | Cross-platform terminal music streaming player | Modern music player with streaming support and intuitive TUI. | All | [clangen/musikcube](https://github.com/clangen/musikcube) | — | BSD-3-Clause | ✅ |
| [termusic](https://github.com/tramhao/termusic) | Terminal music player written in Rust | Features cover art display in supported terminals with album art. | All | [tramhao/termusic](https://github.com/tramhao/termusic) | — | GPL-3.0 | ✅ |
| [ncmpcpp](https://rybczak.net/ncmpcpp/) | Feature-rich MPD client for the terminal | NCurses MPD client with tag editor, playlist editor, and visualization. | Lin/mac | [ncmpcpp/ncmpcpp](https://github.com/ncmpcpp/ncmpcpp) | — | GPL-2.0 | ✅ |
| [mpd](https://github.com/MusicPlayerDaemon/MPD) | Music Player Daemon | Server-based music player with client-server architecture. | Lin/mac | [MusicPlayerDaemon/MPD](https://github.com/MusicPlayerDaemon/MPD) | — | GPL-2.0 | ✅ |
| [moc](https://moc.daper.net/) | Lightweight console audio player | Music On Console - simple and intuitive audio player. | Lin | — | — | GPL-2.0 | ✅ |
| [mps-youtube](https://github.com/mps-youtube/mps-youtube) | YouTube music player and downloader for terminal | Search, stream, and download YouTube music from terminal. | All | [mps-youtube/yewtube](https://github.com/mps-youtube/yewtube) | — | GPL-3.0 | ✅ |
| [cava](https://github.com/karlstav/cava) | Cross-platform audio visualizer for the terminal | Real-time audio spectrum visualizer with configurable colors. | Lin/mac | [karlstav/cava](https://github.com/karlstav/cava) | — | MIT | ✅ |
| [sox](http://sox.sourceforge.net/) | Swiss Army knife of audio processing | Convert audio formats, apply effects, generate tones. | Lin/mac | — | — | LGPL-2.1 | ✅ |
| [spotify-tui](https://github.com/Rigellute/spotify-tui) | Spotify client for the terminal | Control Spotify playback from your terminal (requires spotifyd or Spotify Premium). | All | [Rigellute/spotify-tui](https://github.com/Rigellute/spotify-tui) | — | MIT | ✅ |
| [spotifyd](https://github.com/Spotifyd/spotifyd) | Lightweight Spotify daemon | Spotify Connect daemon that runs in background. | All | [Spotifyd/spotifyd](https://github.com/Spotifyd/spotifyd) | — | GPL-3.0 | ✅ |

---

## Containers & Orchestration

Tools for managing Docker, Kubernetes, and containers.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [lazydocker](https://github.com/jesseduffield/lazydocker) | The lazygit of Docker | Full TUI for containers with logs, stats, and management all in one screen. | All | [jesseduffield/lazydocker](https://github.com/jesseduffield/lazydocker) | ![GitHub Release](https://img.shields.io/github/v/release/jesseduffield/lazydocker?label=) | MIT | ✅ |
| [k9s](https://k9scli.io/) | Kubernetes TUI | Manage clusters from the terminal — navigate pods, logs, deployments interactively. | All | [derailed/k9s](https://github.com/derailed/k9s) | ![GitHub Release](https://img.shields.io/github/v/release/derailed/k9s?label=) | Apache-2.0 | ✅ |
| [dive](https://github.com/wagoodman/dive) | Explore Docker image layers interactively | Inspect each layer's contents and find ways to shrink image size. | All | [wagoodman/dive](https://github.com/wagoodman/dive) | — | MIT | ✅ |
| [kubectx + kubens](https://github.com/ahmetb/kubectx) | Instantly switch Kubernetes contexts and namespaces | Essential productivity tools for multi-cluster Kubernetes workflows. | All | [ahmetb/kubectx](https://github.com/ahmetb/kubectx) | — | Apache-2.0 | ✅ |
| [stern](https://github.com/stern/stern) | Multi-pod log tailing for Kubernetes | Tail logs from multiple pods simultaneously with color-coding per pod. | All | [stern/stern](https://github.com/stern/stern) | ![GitHub Release](https://img.shields.io/github/v/release/stern/stern?label=) | Apache-2.0 | ✅ |
| [kubectl](https://kubernetes.io/docs/reference/kubectl/) | Official Kubernetes command-line tool | The foundational tool for interacting with Kubernetes clusters. | All | [kubernetes/kubectl](https://github.com/kubernetes/kubectl) | — | Apache-2.0 | ✅ |
| [helm](https://helm.sh/) | Package manager for Kubernetes | Deploy complex applications on Kubernetes using charts. | All | [helm/helm](https://github.com/helm/helm) | ![GitHub Release](https://img.shields.io/github/v/release/helm/helm?label=) | Apache-2.0 | ✅ |
| [podman](https://podman.io/) | Daemonless container engine | Docker-compatible container engine that doesn't require a daemon. | Lin/mac | [containers/podman](https://github.com/containers/podman) | — | Apache-2.0 | ✅ |
| [skopeo](https://github.com/containers/skopeo) | Work with container images without a daemon | Inspect, copy, and manage container images across registries. | All | [containers/skopeo](https://github.com/containers/skopeo) | — | Apache-2.0 | ✅ |
| [dockly](https://github.com/lirantal/dockly) | Interactively manage containers | TUI for Docker container management. | All | [lirantal/dockly](https://github.com/lirantal/dockly) | — | MIT | ✅ |

---

## Git & Development Tools

Tools for Git, version control, benchmarking, and development workflows.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [lazygit](https://github.com/jesseduffield/lazygit) | Full-featured TUI for git | Stage, commit, branch, merge, rebase, stash — all with keyboard shortcuts in a beautiful interface. | All | [jesseduffield/lazygit](https://github.com/jesseduffield/lazygit) | ![GitHub Release](https://img.shields.io/github/v/release/jesseduffield/lazygit?label=) | MIT | ✅ |
| [gh](https://cli.github.com/) | Official GitHub CLI | Create and review PRs, manage issues, run workflows, all from your terminal. | All | [cli/cli](https://github.com/cli/cli) | ![GitHub Release](https://img.shields.io/github/v/release/cli/cli?label=) | MIT | ✅ |
| [delta](https://dandavison.github.io/delta/) | Syntax-highlighting pager for `git diff` | Beautiful side-by-side diffs with syntax highlighting and git blame integration. | All | [dandavison/delta](https://github.com/dandavison/delta) | ![GitHub Release](https://img.shields.io/github/v/release/dandavison/delta?label=) | MIT | ✅ |
| [tig](https://jonas.github.io/tig/) | Text-mode interface for git | NCurses-based git repository browser and commit viewer. | Lin/mac | [jonas/tig](https://github.com/jonas/tig) | — | GPL-2.0 | ✅ |
| [hyperfine](https://github.com/sharkdp/hyperfine) | Command-line benchmarking tool | Statistical benchmark analysis with warmup runs and export to multiple formats. | All | [sharkdp/hyperfine](https://github.com/sharkdp/hyperfine) | ![GitHub Release](https://img.shields.io/github/v/release/sharkdp/hyperfine?label=) | Apache-2.0/MIT | ✅ |
| [tokei](https://github.com/XAMPPRocky/tokei) | Count lines of code across a project | Fast code statistics tool showing language breakdown and metrics. | All | [XAMPPRocky/tokei](https://github.com/XAMPPRocky/tokei) | ![GitHub Release](https://img.shields.io/github/v/release/XAMPPRocky/tokei?label=) | Apache-2.0/MIT | ✅ |
| [just](https://just.systems/) | A modern command runner | Simpler than Makefile with better syntax for project task automation. | All | [casey/just](https://github.com/casey/just) | ![GitHub Release](https://img.shields.io/github/v/release/casey/just?label=) | CC0-1.0 | ✅ |
| [glow](https://github.com/charmbracelet/glow) | Render Markdown beautifully in the terminal | Read markdown files with styled rendering directly in your terminal. | All | [charmbracelet/glow](https://github.com/charmbracelet/glow) | ![GitHub Release](https://img.shields.io/github/v/release/charmbracelet/glow?label=) | MIT | ✅ |
| [watchexec](https://watchexec.github.io/) | Execute commands on file system changes | More feature-rich than entr with glob patterns and debouncing. | All | [watchexec/watchexec](https://github.com/watchexec/watchexec) | ![GitHub Release](https://img.shields.io/github/v/release/watchexec/watchexec?label=) | Apache-2.0 | ✅ |
| [ouch](https://github.com/ouch-org/ouch) | Painless compression and decompression | Single tool for all archive formats with intuitive syntax. | All | [ouch-org/ouch](https://github.com/ouch-org/ouch) | ![GitHub Release](https://img.shields.io/github/v/release/ouch-org/ouch?label=) | MIT | ✅ |
| [age](https://age-encryption.org/) | Simple, modern, and secure file encryption | Simpler alternative to GPG for file encryption with small explicit keys. | All | [FiloSottile/age](https://github.com/FiloSottile/age) | — | BSD-3-Clause | ✅ |
| [chezmoi](https://www.chezmoi.io/) | Manage dotfiles across machines securely | Template-driven dotfile manager with machine-specific configuration support. | All | [twpayne/chezmoi](https://github.com/twpayne/chezmoi) | ![GitHub Release](https://img.shields.io/github/v/release/twpayne/chezmoi?label=) | MIT | ✅ |
| [difftastic](https://difftastic.wilfred.me.uk/) | Structural diff tool that understands syntax | AST-based diff that compares code structure rather than just lines. | All | [Wilfred/difftastic](https://github.com/Wilfred/difftastic) | — | MIT | ✅ |
| [gitui](https://github.com/extrawurst/gitui) | Blazing fast terminal UI for git written in Rust | Lightweight alternative to lazygit with incredible performance. | All | [extrawurst/gitui](https://github.com/extrawurst/gitui) | ![GitHub Release](https://img.shields.io/github/v/release/extrawurst/gitui?label=) | MIT | ✅ |
| [onefetch](https://onefetch.dev/) | Git repository information tool with ASCII art | Display project information and statistics with ASCII logo. | All | [o2sh/onefetch](https://github.com/o2sh/onefetch) | ![GitHub Release](https://img.shields.io/github/v/release/o2sh/onefetch?label=) | MIT | ✅ |
| [scc](https://github.com/boyter/scc) | Extremely fast code counter | Count lines of code with accuracy and speed, complexity metrics included. | All | [boyter/scc](https://github.com/boyter/scc) | ![GitHub Release](https://img.shields.io/github/v/release/boyter/scc?label=) | MIT / Unlicense | ✅ |
| [git-cliff](https://git-cliff.org/) | Changelog generator from git history | Highly customizable changelog generator following Conventional Commits. | All | [orhun/git-cliff](https://github.com/orhun/git-cliff) | ![GitHub Release](https://img.shields.io/github/v/release/orhun/git-cliff?label=) | Apache-2.0/MIT | ✅ |
| [act](https://github.com/nektos/act) | Run GitHub Actions locally | Test GitHub Actions workflows on your local machine. | All | [nektos/act](https://github.com/nektos/act) | ![GitHub Release](https://img.shields.io/github/v/release/nektos/act?label=) | MIT | ✅ |
| [pre-commit](https://pre-commit.com/) | Framework for managing git hooks | Run linters, formatters, and tests before committing. | All | [pre-commit/pre-commit](https://github.com/pre-commit/pre-commit) | — | MIT | ✅ |
| [restic](https://restic.net/) | Fast, secure backup program | Modern backup tool with encryption and deduplication. | All | [restic/restic](https://github.com/restic/restic) | ![GitHub Release](https://img.shields.io/github/v/release/restic/restic?label=) | BSD-2-Clause | ✅ |

---

## Text Editors

Powerful text editors for the terminal.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [Neovim](https://neovim.io/) | Hyperextensible Vim-based text editor | Modern fork of Vim with better defaults, async support, and Lua integration. The most modern modal editor. | All | [neovim/neovim](https://github.com/neovim/neovim) | ![GitHub Release](https://img.shields.io/github/v/release/neovim/neovim?label=) | Apache-2.0 | ✅ |
| [Vim](https://www.vim.org/) | The ubiquitous modal text editor | Found on virtually every Unix system. The standard terminal editor. | All | [vim/vim](https://github.com/vim/vim) | — | Vim License | ✅ |
| [Emacs](https://www.gnu.org/software/emacs/) | Extensible, customizable, self-documenting editor | Feature-rich extensible editor with elisp scripting. | All | [emacs-mirror/emacs](https://github.com/emacs-mirror/emacs) | — | GPL-3.0 | ✅ |
| [Helix](https://helix-editor.com/) | Post-modern modal text editor | Inspired by Kakoune with multiple selections and tree-sitter integration. | All | [helix-editor/helix](https://github.com/helix-editor/helix) | ![GitHub Release](https://img.shields.io/github/v/release/helix-editor/helix?label=) | MPL-2.0 | ✅ |
| [nano](https://nano-editor.org/) | Simple, beginner-friendly terminal editor | No learning curve, straightforward keybindings displayed at bottom. | All | — | — | GPL-3.0 | ✅ |
| [micro](https://micro-editor.github.io/) | Modern terminal editor with mouse support | Intuitive keybindings (Ctrl+S, Ctrl+C, Ctrl+V), mouse support, and plugin system. | All | [zyedidia/micro](https://github.com/zyedidia/micro) | ![GitHub Release](https://img.shields.io/github/v/release/zyedidia/micro?label=) | MIT | ✅ |
| [Kakoune](https://kakoune.org/) | Modal editor with multiple selections | Innovative editing model with multi-cursor editing paradigm. | Lin/mac | [mawww/kakoune](https://github.com/mawww/kakoune) | — | Unlicense | ✅ |
| [joe](https://joe-editor.sourceforge.io/) | Joe's Own Editor | WordStar-like keybindings, simple lightweight editor. | Lin/mac | — | — | GPL-2.0 | ✅ |

---

## Productivity & Tasks

Task management, note-taking, calendars, presentations, and productivity tools.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [Taskwarrior](https://taskwarrior.org/) | Powerful command-line task manager | Feature-rich task management with priorities, tags, projects, and sophisticated filtering. | All | [GothenburgBitFactory/taskwarrior](https://github.com/GothenburgBitFactory/taskwarrior) | — | MIT | ✅ |
| [jrnl](https://jrnl.sh/) | Collect your thoughts in a plain-text journal | Simple command-line journaling with tagging and time tracking. | All | [jrnl-org/jrnl](https://github.com/jrnl-org/jrnl) | — | GPL-3.0 | ✅ |
| [todo.txt-cli](http://todotxt.org/) | Plain-text todo list management | Simple, portable, future-proof task tracking. | All | [todotxt/todo.txt-cli](https://github.com/todotxt/todo.txt-cli) | — | GPL-3.0 | ✅ |
| [wtf](https://wtfutil.com/) | Personal information dashboard for the terminal | Terminal dashboard showing calendar, tasks, system metrics, and more. | All | [wtfutil/wtf](https://github.com/wtfutil/wtf) | — | MPL-2.0 | ✅ |
| [slides](https://github.com/maaslalani/slides) | Terminal-based presentation from Markdown | Create and present slides directly in your terminal. | All | [maaslalani/slides](https://github.com/maaslalani/slides) | — | MIT | ✅ |
| [tldr](https://tldr.sh/) | Simplified man pages with practical examples | Community-driven man pages with concise, practical examples. | All | [tldr-pages/tldr](https://github.com/tldr-pages/tldr) | — | MIT | ✅ |
| [calcurse](https://calcurse.org/) | Terminal calendar and scheduling application | Full-featured calendar with todo list and appointment notifications. | Lin/mac | [lfos/calcurse](https://github.com/lfos/calcurse) | — | BSD-2-Clause | ✅ |
| [nb](https://xwmx.github.io/nb/) | Command-line note-taking, bookmarking, and archiving | Powerful note-taking with git-based sync and encryption. | All | [xwmx/nb](https://github.com/xwmx/nb) | — | AGPL-3.0 | ✅ |
| [sc-im](https://github.com/andmarti1424/sc-im) | Terminal spreadsheet with vim-like keybindings | Full-featured spreadsheet calculator in the terminal. | Lin/mac | [andmarti1424/sc-im](https://github.com/andmarti1424/sc-im) | — | BSD-4-Clause | ✅ |
| [pandoc](https://pandoc.org/) | Universal document converter | Convert between dozens of document formats (Markdown, HTML, PDF, Word, LaTeX...). | All | [jgm/pandoc](https://github.com/jgm/pandoc) | — | GPL-2.0 | ✅ |
| [taskell](https://github.com/smallhadroncollider/taskell) | Command-line Kanban board | Interactive Kanban board in your terminal. | All | [smallhadroncollider/taskell](https://github.com/smallhadroncollider/taskell) | — | BSD-3-Clause | ✅ |
| [Buku](https://github.com/jarun/Buku) | Browser-independent bookmark manager | Powerful bookmark management with tagging and full-text search. | All | [jarun/Buku](https://github.com/jarun/Buku) | — | GPL-3.0 | ✅ |
| [Timewarrior](https://github.com/GothenburgBitFactory/timewarrior) | Time tracking utility | Simple stopwatch with calendar-based reporting. | All | [GothenburgBitFactory/timewarrior](https://github.com/GothenburgBitFactory/timewarrior) | — | MIT | ✅ |
| [Watson](https://github.com/TailorDev/Watson) | Time tracking for consultants | Generate reports for clients and manage your time. | All | [TailorDev/Watson](https://github.com/TailorDev/Watson) | — | MIT | ✅ |
| [ledger](https://github.com/ledger/ledger) | Command line accounting | Double-entry accounting system with powerful reporting. | All | [ledger/ledger](https://github.com/ledger/ledger) | — | BSD-3-Clause | ✅ |
| [hledger](https://hledger.org/) | Robust, fast, intuitive plain text accounting | More user-friendly alternative to ledger with better documentation. | All | [simonmichael/hledger](https://github.com/simonmichael/hledger) | — | GPL-3.0 | ✅ |
| [cointop](https://github.com/miguelmota/cointop) | Track cryptocurrencies | Real-time cryptocurrency price tracker. | All | [miguelmota/cointop](https://github.com/ciguelmota/cointop) | — | Apache-2.0 | ✅ |
| [ticker](https://github.com/achannarasappa/ticker) | Stock ticker | Terminal stock market ticker with live updates. | All | [achannarasappa/ticker](https://github.com/achannarasappa/ticker) | — | GPL-3.0 | ✅ |
| [mdp](https://github.com/visit1985/mdp) | A markdown presentation tool | Present Markdown files as slides in the terminal. | All | [visit1985/mdp](https://github.com/visit1985/mdp) | — | GPL-3.0 | ✅ |
| [gcalcli](https://github.com/insanum/gcalcli) | Google calendar client | Access and manage Google Calendar from terminal. | All | [insanum/gcalcli](https://github.com/insanum/gcalcli) | — | MIT | ✅ |

---

## Research & Science

Paper managers, arXiv downloaders, reference tools, and scientific computing in the terminal.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [papis](https://papis.readthedocs.io/) | Powerful CLI document and bibliography manager | The definitive terminal reference manager. Import papers by DOI or arXiv ID, organizes PDFs and BibTeX, searches your library, and exports citations. Highly extensible with plugins. | All | [papis/papis](https://github.com/papis/papis) | ![GitHub Release](https://img.shields.io/github/v/release/papis/papis?label=) | GPL-3.0 | ✅ |
| [arxiv-downloader](https://github.com/braun-steven/arxiv-downloader) | Download papers from arXiv by ID or keyword | Fetch papers from arXiv.org by arXiv ID or keyword search. Automatically names files by author/year/title and handles batch downloads. | All | [braun-steven/arxiv-downloader](https://github.com/braun-steven/arxiv-downloader) | — | MIT | ✅ |
| [doi2bib](https://github.com/bibcure/doi2bib) | Convert a DOI to a BibTeX citation in one command | Enter any DOI and get a properly formatted BibTeX entry. Eliminates the need to visit publisher sites to copy citations. | All | [bibcure/doi2bib](https://github.com/bibcure/doi2bib) | — | MIT | ✅ |
| [betterbib](https://github.com/nschloe/betterbib) | Auto-improve BibTeX files from online databases | Completes and corrects BibTeX entries by querying CrossRef and other academic APIs. Catches wrong titles, missing fields, and formatting issues. | All | [nschloe/betterbib](https://github.com/nschloe/betterbib) | — | MIT | ✅ |
| [cobib](https://gitlab.com/cobib/cobib) | Console-based bibliography manager | Alternative to papis with a TUI interface, vim-inspired keybindings, and full BibTeX/BibLaTeX support. Stores data as plain YAML. | All | [cobib/cobib](https://gitlab.com/cobib/cobib) | — | MIT | ✅ |
| [papermill](https://papermill.readthedocs.io/) | Parameterize and execute Jupyter notebooks from CLI | Run notebooks with different input parameters from scripts or CI pipelines — the standard tool for reproducible research workflows. | All | [nteract/papermill](https://github.com/nteract/papermill) | ![GitHub Release](https://img.shields.io/github/v/release/nteract/papermill?label=) | BSD-3-Clause | ✅ |
| [gnuplot](http://www.gnuplot.info/) | Portable command-line scientific plotting | Plot functions and data in 2D/3D, output to terminal, PNG, SVG, PDF, and more. Decades-old standard for scientific visualization. | All | [gnuplot/gnuplot](https://github.com/gnuplot/gnuplot) | — | gnuplot | ✅ |
| [sc-im](https://github.com/andmarti1424/sc-im) | Spreadsheet calculator in the terminal | Vim-style ncurses spreadsheet with formulas, graphs, and CSV/Excel import. Ideal for quick data analysis without leaving the terminal. | Lin/mac | [andmarti1424/sc-im](https://github.com/andmarti1424/sc-im) | — | BSD-4-Clause | ✅ |
| [units](https://www.gnu.org/software/units/) | Universal unit conversion from the command line | Convert between thousands of units (SI, imperial, historical, currencies). Essential for scientists and engineers. | Lin/mac | — | — | GPL-3.0 | ✅ |
| [qalc](https://qalculate.github.io/) | Powerful multi-purpose calculator with unit support | Interactive calculator handling complex expressions, unit conversions, variables, and plotting. More powerful than `bc` for scientific use. | All | [Qalculate/libqalculate](https://github.com/Qalculate/libqalculate) | — | GPL-2.0 | ✅ |

---

## Databases & Data

Database CLIs with autocompletion and syntax highlighting.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [pgcli](https://www.pgcli.com/) | PostgreSQL CLI with autocompletion and syntax highlighting | Modern PostgreSQL client with intelligent completions and syntax highlighting. | All | [dbcli/pgcli](https://github.com/dbcli/pgcli) | — | BSD-3-Clause | ✅ |
| [mycli](https://www.mycli.net/) | MySQL/MariaDB CLI with autocompletion | Intelligent MySQL client with autocompletion and syntax highlighting. | All | [dbcli/mycli](https://github.com/dbcli/mycli) | — | BSD-3-Clause | ✅ |
| [litecli](https://litecli.com/) | SQLite CLI with autocompletion and syntax highlighting | User-friendly SQLite client with smart completions. | All | [dbcli/litecli](https://github.com/dbcli/litecli) | — | BSD-3-Clause | ✅ |
| [usql](https://github.com/xo/usql) | Universal SQL CLI for multiple database systems | Single CLI for PostgreSQL, MySQL, SQLite, SQL Server, Oracle, and more. | All | [xo/usql](https://github.com/xo/usql) | — | MIT | ✅ |
| [redis-cli](https://redis.io/docs/ui/cli/) | Official Redis command-line client | Standard tool for interacting with Redis databases. | All | [redis/redis](https://github.com/redis/redis) | — | BSD-3-Clause | ✅ |
| [mongosh](https://www.mongodb.com/docs/mongodb-shell/) | Modern MongoDB Shell | JavaScript-based MongoDB shell with improved syntax. | All | [mongodb-js/mongosh](https://github.com/mongodb-js/mongosh) | — | Apache-2.0 | ✅ |
| [sqlc](https://sqlc.dev/) | Generate type-safe code from SQL | Compile SQL queries to type-safe code in Go, Python, and more. | All | [sqlc-dev/sqlc](https://github.com/sqlc-dev/sqlc) | — | MIT | ✅ |
| [dblab](https://github.com/danvergara/dblab) | Interactive database client TUI | TUI for PostgreSQL, MySQL, SQLite with visual query builder. | All | [danvergara/dblab](https://github.com/danvergara/dblab) | — | MIT | ✅ |

---

## Security & Privacy

Password managers, encryption tools, and security utilities.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [pass](https://www.passwordstore.org/) | The standard Unix password manager | GPG-based password manager with git integration. Simple, scriptable, and secure. | Lin/mac | [zx2c4/password-store](https://git.zx2c4.com/password-store) | — | GPL-2.0 | ✅ |
| [gopass](https://www.gopass.pw/) | Password manager for teams | Team-oriented rewrite of pass with more features and better UX. | All | [gopasspw/gopass](https://github.com/gopasspw/gopass) | — | MIT | ✅ |
| [GnuPG (gpg)](https://gnupg.org/) | Complete implementation of OpenPGP standard | Industry-standard encryption and signing tool. | All | — | — | GPL-3.0 | ✅ |
| [ssh-audit](https://github.com/jtesta/ssh-audit) | SSH server security auditing tool | Audit SSH configurations for security issues and compliance. | All | [jtesta/ssh-audit](https://github.com/jtesta/ssh-audit) | — | MIT | ✅ |
| [lynis](https://cisofy.com/lynis/) | Security auditing and hardening tool | Comprehensive security audit for Unix-based systems. | Lin/mac | [CISOfy/lynis](https://github.com/CISOfy/lynis) | — | GPL-3.0 | ✅ |
| [trivy](https://trivy.dev/) | Comprehensive security scanner | Scan containers, filesystems, IaC for vulnerabilities and misconfigurations. | All | [aquasecurity/trivy](https://github.com/aquasecurity/trivy) | ![GitHub Release](https://img.shields.io/github/v/release/aquasecurity/trivy?label=) | Apache-2.0 | ✅ |
| [gitleaks](https://gitleaks.io/) | Find secrets in git repos | Scan git repositories for secrets, API keys, and credentials. | All | [gitleaks/gitleaks](https://github.com/gitleaks/gitleaks) | ![GitHub Release](https://img.shields.io/github/v/release/gitleaks/gitleaks?label=) | MIT | ✅ |
| [hashcat](https://hashcat.net/hashcat/) | Advanced password recovery tool | World's fastest password cracker with GPU support. | All | [hashcat/hashcat](https://github.com/hashcat/hashcat) | — | MIT | ✅ |
| [ots](https://github.com/sniptt-official/ots) | Share secrets with others via a one-time URL | Create self-destructing secret links. | All | [sniptt-official/ots](https://github.com/sniptt-official/ots) | — | Apache-2.0 | ✅ |

---

## Terminal Multiplexers

Session managers that let you run multiple terminal sessions in one window.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [tmux](https://github.com/tmux/tmux) | The industry-standard terminal multiplexer | Persistent sessions, split windows, and detachable execution. Essential for remote work. | Lin/mac/WSL | [tmux/tmux](https://github.com/tmux/tmux) | — | ISC | ✅ |
| [Zellij](https://zellij.dev/) | Modern, user-friendly multiplexer | Written in Rust with sensible defaults, floating panes, and no configuration needed. | Lin/mac/WSL | [zellij-org/zellij](https://github.com/zellij-org/zellij) | ![GitHub Release](https://img.shields.io/github/v/release/zellij-org/zellij?label=) | MIT | ✅ |
| [GNU Screen](https://www.gnu.org/software/screen/) | The original session multiplexer | Classic multiplexer from 1987, still widely used and pre-installed on many systems. | Lin/mac/WSL | — | — | GPL-3.0 | ✅ |
| [byobu](https://www.byobu.org/) | Tmux/Screen wrapper with status bar | Enhanced wrapper around tmux/screen with user-friendly keybindings and status line. | Lin | — | — | GPL-3.0 | ✅ |
| [tmuxinator](https://github.com/tmuxinator/tmuxinator) | Manage complex tmux sessions | Define tmux session layouts in YAML files for quick project restoration. | All | [tmuxinator/tmuxinator](https://github.com/tmuxinator/tmuxinator) | — | MIT | ✅ |

---

## Fun & Miscellaneous

Entertainment, toys, games, and quirky utilities.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [fastfetch](https://github.com/fastfetch-cli/fastfetch) | Lightning-fast system info with ASCII art | Modern neofetch alternative that's significantly faster. | All | [fastfetch-cli/fastfetch](https://github.com/fastfetch-cli/fastfetch) | ![GitHub Release](https://img.shields.io/github/v/release/fastfetch-cli/fastfetch?label=) | MIT | ✅ |
| [neofetch](https://github.com/dylanaraps/neofetch) | Classic system info tool with ASCII art | The original and iconic system information tool. | All | [dylanaraps/neofetch](https://github.com/dylanaraps/neofetch) | — | MIT | ✅ |
| [hollywood](https://github.com/dustinkirkland/hollywood) | Fake busy hacker movie terminal | Fill your terminal with "hacker" output like in movies. | Lin | [dustinkirkland/hollywood](https://github.com/dustinkirkland/hollywood) | — | Apache-2.0 | ✅ |
| [cmatrix](https://github.com/abishekvashok/cmatrix) | The Matrix digital rain in your terminal | Cascading Matrix-style digital rain animation. | Lin/mac | [abishekvashok/cmatrix](https://github.com/abishekvashok/cmatrix) | — | GPL-3.0 | ✅ |
| [pipes.sh](https://github.com/pipeseroni/pipes.sh) | Animated pipe screensaver for the terminal | Colorful animated pipes flowing across your screen. | Lin/mac | [pipeseroni/pipes.sh](https://github.com/pipeseroni/pipes.sh) | — | MIT | ✅ |
| [no-more-secrets](https://github.com/bartobri/no-more-secrets) | Recreate the *Sneakers* decryption effect | "Decrypting" text animation from the movie Sneakers. | Lin/mac | [bartobri/no-more-secrets](https://github.com/bartobri/no-more-secrets) | — | GPL-3.0 | ✅ |
| [sl](https://github.com/mtoyoda/sl) | Steam locomotive crosses your terminal | A train animation that runs when you typo `ls` as `sl`. | Lin/mac | [mtoyoda/sl](https://github.com/mtoyoda/sl) | — | MIT-like | ✅ |
| [cowsay](https://github.com/cowsay-org/cowsay) | A talking cow in your terminal | ASCII cow (or other animals) speaking your message. | Lin/mac | [cowsay-org/cowsay](https://github.com/cowsay-org/cowsay) | — | GPL-3.0 | ✅ |
| [figlet](http://www.figlet.org/) | Large ASCII text banners | Create large ASCII art text banners from any string. | Lin/mac | — | — | BSD-3-Clause | ✅ |
| [lolcat](https://github.com/busyloop/lolcat) | Rainbow-colorize any terminal output | Pipe any text through lolcat for rainbow gradients. | Lin/mac | [busyloop/lolcat](https://github.com/busyloop/lolcat) | — | BSD-3-Clause | ✅ |
| [nyancat](https://github.com/klange/nyancat) | Nyan Cat in your terminal | The iconic animated rainbow cat in ANSI. | Lin/mac | [klange/nyancat](https://github.com/klange/nyancat) | — | NCSA | ✅ |
| [cbonsai](https://gitlab.com/jallbrit/cbonsai) | Grow a bonsai tree in your terminal | Watch an ASCII bonsai tree grow procedurally. | Lin/mac | [jallbrit/cbonsai](https://gitlab.com/jallbrit/cbonsai) | — | GPL-3.0 | ✅ |
| [asciiquarium](https://rya.nc/asciiquarium.html) | Aquarium/sea animation in ASCII art | Animated underwater scene with fish and sea creatures. | Lin/mac | — | — | GPL-2.0 | ✅ |
| [fortune](https://en.wikipedia.org/wiki/Fortune_(Unix)) | Display a random quotation | Classic Unix utility displaying random quotes. | Lin/mac | — | — | BSD-like | ✅ |
| [toilet](http://caca.zoy.org/wiki/toilet) | Display large colorful ASCII art text | Like figlet but with color and more font options. | Lin/mac | — | — | WTFPL | ✅ |
| [genact](https://github.com/svenstaro/genact) | Nonsense activity generator | Pretend to be busy with realistic-looking fake activity. | All | [svenstaro/genact](https://github.com/svenstaro/genact) | — | MIT | ✅ |
| [wttr.in](https://github.com/chubin/wttr.in) | The right way to check the weather | `curl wttr.in` for beautiful weather forecasts. | All | [chubin/wttr.in](https://github.com/chubin/wttr.in) | — | Apache-2.0 | ✅ |
| [mapscii](https://github.com/rastapasta/mapscii) | Terminal Map Viewer | Explore OpenStreetMap in your terminal with zoom and panning. | All | [rastapasta/mapscii](https://github.com/rastapasta/mapscii) | — | MIT | ✅ |
| [emoj](https://github.com/sindresorhus/emoj) | Find relevant emoji from text | Quickly search and copy emoji to clipboard. | All | [sindresorhus/emoj](https://github.com/sindresorhus/emoj) | — | MIT | ✅ |
| [pastel](https://github.com/sharkdp/pastel) | Generate, analyze, convert and manipulate colors | Complete color manipulation toolkit for the terminal. | All | [sharkdp/pastel](https://github.com/sharkdp/pastel) | — | Apache-2.0/MIT | ✅ |
| [The Fuck](https://github.com/nvbn/thefuck) | Magnificent app which corrects your previous console command | Already listed in Shell & Navigation but deserves a mention here too. | All | [nvbn/thefuck](https://github.com/nvbn/thefuck) | ![GitHub Release](https://img.shields.io/github/v/release/nvbn/thefuck?label=) | MIT | ✅ |
| [howdoi](https://github.com/gleitz/howdoi) | Instant coding answers | Get instant answers to coding questions from the command line. | All | [gleitz/howdoi](https://github.com/gleitz/howdoi) | — | MIT | ✅ |
| [yai](https://github.com/ekkinox/yai) | AI powered terminal assistant | ChatGPT-powered assistant for command-line help. | All | [ekkinox/yai](https://github.com/ekkinox/yai) | — | MIT | ✅ |
| [has](https://github.com/kdabir/has) | Checks for the presence of various commands | Quickly verify if specific commands/tools are installed. | All | [kdabir/has](https://github.com/kdabir/has) | — | MIT | ✅ |
| [Ultimate Plumber](https://github.com/akavel/up) | Write Linux pipes with live previews | Interactively build command pipelines with instant feedback. | All | [akavel/up](https://github.com/akavel/up) | — | Apache-2.0 | ✅ |
| [fkill-cli](https://github.com/sindresorhus/fkill-cli) | Simple cross-platform process killer | Interactive process killer with fuzzy search. | All | [sindresorhus/fkill-cli](https://github.com/sindresorhus/fkill-cli) | — | MIT | ✅ |

---

## Command Line Learning

Resources and tools for learning command-line skills.

| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [explainshell](https://www.explainshell.com/) | Type a snippet to see the help text | Web service that explains shell commands by parsing man pages. | All | [idank/explainshell](https://github.com/idank/explainshell) | — | GPL-3.0 | ✅ |
| [cmdchallenge](https://cmdchallenge.com) | Shell challenges with user-submitted solutions | Test and improve your shell skills with interactive challenges. | All | — | — | — | ✅ |
| [howdoi](https://github.com/gleitz/howdoi) | Instant coding answers | Get programming answers from Stack Overflow directly in terminal. | All | [gleitz/howdoi](https://github.com/gleitz/howdoi) | — | MIT | ✅ |
| [tldr](https://tldr.sh/) | Simplified man pages | Community-driven man pages with practical examples. | All | [tldr-pages/tldr](https://github.com/tldr-pages/tldr) | — | MIT | ✅ |

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for contribution guidelines. All contributions are welcome — from adding new tools to fixing bugs or improving descriptions.

Pull requests, suggestions, and feedback are highly appreciated!

---

## License

This work is licensed under [Creative Commons Attribution 4.0 International License](LICENSE.md).

[![CC BY 4.0](https://licensebuttons.net/l/by/4.0/88x31.png)](https://creativecommons.org/licenses/by/4.0/)

**Built with ❤️ by the community.**  
Integrates content from [awesome-shell](https://github.com/alebcay/awesome-shell), [awesome-cli-apps](https://github.com/agarrharr/awesome-cli-apps), and original contributions.

---

**Note:** This is a living document. Tools are continuously updated and new ones added regularly. Star this repo to stay updated!
