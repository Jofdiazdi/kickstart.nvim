# Neovim Keymaps

This file documents all the keymaps configured in this Neovim setup. The `<leader>` key is set to `Space`.

## Global & Core

### Editor Behavior

| Mode | Keybinding      | Description                               |
| :--- | :-------------- | :---------------------------------------- |
| `n`  | `<Esc>`         | Clear search highlights                   |
| `i`  | `jk`            | Exit insert mode                          |
| `t`  | `<Esc><Esc>`    | Exit terminal mode                        |
| `n`  | `<leader>+`     | Increment number                          |
| `n`  | `<leader>-`     | Decrement number                          |
| `n`  | `<leader>l`     | Trigger linting for current file          |
| `n`  | `<leader>mp`    | Format file or range with Prettier        |
| `v`  | `<leader>mp`    | Format file or range with Prettier        |

### Window & Tab Management

| Mode | Keybinding      | Description                               |
| :--- | :-------------- | :---------------------------------------- |
| `n`  | `<C-h>`         | Move focus to the left window             |
| `n`  | `<C-l>`         | Move focus to the right window            |
| `n`  | `<C-j>`         | Move focus to the lower window            |
| `n`  | `<C-k>`         | Move focus to the upper window            |
| `n`  | `<leader>sv`    | Split window vertically                   |
| `n`  | `<leader>sh`    | Split window horizontally                 |
| `n`  | `<leader>se`    | Make splits equal size                    |
| `n`  | `<leader>sx`    | Close current split                       |
| `n`  | `<leader>sm`    | Maximize/minimize a split                 |
| `n`  | `<leader>to`    | Open new tab                              |
| `n`  | `<leader>tx`    | Close current tab                         |
| `n`  | `<leader>tn`    | Go to next tab                            |
| `n`  | `<leader>tp`    | Go to previous tab                        |
| `n`  | `<leader>tf`    | Open current buffer in new tab            |

## LSP, Diagnostics & Code

| Mode | Keybinding      | Description                               |
| :--- | :-------------- | :---------------------------------------- |
| `n`  | `gD`            | Go to declaration                         |
| `n`  | `gd`            | Show LSP definitions (via Telescope)      |
| `n`  | `gi`            | Show LSP implementations (via Telescope)  |
| `n`  | `gt`            | Show LSP type definitions (via Telescope) |
| `n`  | `gR`            | Show LSP references (via Telescope)       |
| `n`  | `K`             | Show documentation for item under cursor  |
| `n`  | `<leader>d`     | Show line diagnostics                     |
| `n`  | `<leader>D`     | Show buffer diagnostics (via Telescope)   |
| `n`  | `<leader>q`     | Open diagnostic quickfix list             |
| `n`  | `<leader>rn`    | Smart rename                              |
| `n`  | `<leader>rs`    | Restart LSP                               |
| `n`  | `<leader>vca`   | See available code actions                |
| `v`  | `<leader>vca`   | See available code actions for selection  |
| `i`  | `<C-h>`         | Show signature help                       |

## Searching (Telescope)

| Mode | Keybinding        | Description                                  |
| :--- | :---------------- | :------------------------------------------- |
| `n`  | `<leader><leader>`| Find existing buffers                        |
| `n`  | `<leader>/`       | Fuzzily search in current buffer             |
| `n`  | `<leader>s.`      | Search Recent Files                          |
| `n`  | `<leader>s/`      | Search in Open Files                         |
| `n`  | `<leader>sc`      | Find colorscheme                             |
| `n`  | `<leader>sd`      | Search Diagnostics                           |
| `n`  | `<leader>sf`      | Search Files                                 |
| `n`  | `<leader>sg`      | Search by Grep (Live Grep)                   |
| `n`  | `<leader>sh`      | Search Help                                  |
| `n`  | `<leader>sk`      | Search Keymaps                               |
| `n`  | `<leader>sn`      | Search Neovim config files                   |
| `n`  | `<leader>sr`      | Resume last Telescope search                 |
| `n`  | `<leader>ss`      | Select a Telescope picker                    |
| `n`  | `<leader>st`      | Find todos                                   |
| `n`  | `<leader>sw`      | Search for current Word under cursor         |

## Git (Gitsigns)

| Mode | Keybinding      | Description                         |
| :--- | :-------------- | :---------------------------------- |
| `n`  | `]c`            | Jump to next git change             |
| `n`  | `[c`            | Jump to previous git change         |
| `n`  | `<leader>hb`    | Git blame line                      |
| `n`  | `<leader>hD`    | Git diff against last commit        |
| `n`  | `<leader>hd`    | Git diff against index              |
| `n`  | `<leader>hp`    | Git preview hunk                    |
| `n`  | `<leader>hR`    | Git reset buffer                    |
| `n`  | `<leader>hr`    | Git reset hunk                      |
| `n`  | `<leader>hS`    | Git stage buffer                    |
| `n`  | `<leader>hs`    | Git stage hunk                      |
| `v`  | `<leader>hs`    | Git stage hunk                      |
| `v`  | `<leader>hr`    | Git reset hunk                      |
| `n`  | `<leader>hu`    | Git undo stage hunk                 |
| `n`  | `<leader>tb`    | Toggle git blame line               |
| `n`  | `<leader>tD`    | Toggle inline git diff              |
| `o,x`| `ih`            | Select hunk text object             |

## Plugin Keymaps

### Debugger (nvim-dap)

| Mode | Keybinding      | Description                         |
| :--- | :-------------- | :---------------------------------- |
| `n`  | `<F1>`          | Debug: Step Into                    |
| `n`  | `<F2>`          | Debug: Step Over                    |
| `n`  | `<F3>`          | Debug: Step Out                     |
| `n`  | `<F5>`          | Debug: Start/Continue               |
| `n`  | `<F7>`          | Debug: See last session result      |
| `n`  | `<leader>b`     | Debug: Toggle Breakpoint            |
| `n`  | `<leader>B`     | Debug: Set Conditional Breakpoint   |

### File Explorer (Neo-tree)

| Mode | Keybinding      | Description                         |
| :--- | :-------------- | :---------------------------------- |
| `n`  | `<leader>ee`    | Toggle file explorer                |
| `n`  | `<leader>ef`    | Reveal current file in explorer     |

### Lazygit & LazyDocker

| Mode | Keybinding      | Description                         |
| :--- | :-------------- | :---------------------------------- |
| `n`  | `<leader>lg`    | Open LazyGit                        |
| `n`  | `<leader>ld`    | Open Lazydocker                     |

### Substitute

| Mode | Keybinding      | Description                         |
| :--- | :-------------- | :---------------------------------- |
| `n`  | `s`             | Substitute with motion              |
| `n`  | `ss`            | Substitute line                     |
| `n`  | `S`             | Substitute to end of line           |
| `x`  | `s`             | Substitute in visual mode           |

### TODO Comments

| Mode | Keybinding      | Description                         |
| :--- | :-------------- | :---------------------------------- |
| `n`  | `]t`            | Next todo comment                   |
| `n`  | `[t`            | Previous todo comment               |

### Trouble

| Mode | Keybinding      | Description                         |
| :--- | :-------------- | :---------------------------------- |
| `n`  | `<leader>xw`    | Open trouble workspace diagnostics  |
| `n`  | `<leader>xd`    | Open trouble document diagnostics   |
| `n`  | `<leader>xq`    | Open trouble quickfix list          |
| `n`  | `<leader>xl`    | Open trouble location list          |
| `n`  | `<leader>xt`    | Open todos in trouble               |

### Yazi File Manager

| Mode | Keybinding      | Description                                  |
| :--- | :-------------- | :------------------------------------------- |
| `n,v`| `<leader>-`     | Open yazi at the current file                |
| `n`  | `<leader>cw`    | Open yazi in nvim's working directory        |
| `n`  | `<c-up>`        | Resume the last yazi session                 |

### Which-Key Groups

These are not direct actions but prefixes that open the which-key menu.

| Mode | Keybinding      | Group Description |
| :--- | :-------------- | :---------------- |
| `n,x`| `<leader>c`     | [C]ode            |
| `n`  | `<leader>d`     | [D]ocument        |
| `n`  | `<leader>r`     | [R]ename          |
| `n`  | `<leader>s`     | [S]earch          |
| `n`  | `<leader>w`     | [W]orkspace       |
| `n`  | `<leader>t`     | [T]oggle          |
| `n,v`| `<leader>h`     | Git [H]unk        |
