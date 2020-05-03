# bootstrap

A script to setup a new `bash` VPS/servers with defaults I like.

Can be run repeatedely to update from newly pushed changes to this repo.

Run:

```
bash -c "$(curl -fsSL https://raw.githubusercontent.com/seanbreckenridge/bootstrap/master/bootstrap)"
```

### Requires:

- `curl`
- `git`
- `nvim`

### Features:

- Sets some default environment variables:
  - Color/Language Options
  - `PS1` (prompt)
- Sets some basic aliases (`ls`/`ll`/git related aliases/`e` to `nvim`)
- sets lots of `nvim` defaults (at `~/.config/nvim/init.vim`)
- installs [`vim-plug`](https://github.com/junegunn/vim-plug) (`vim` plugin manager)
- prompts user to set global name, username and sets default editor for `git`
- Installs fzf using vimscript, add sets up fzf integration into vim and terminal (Ctrl+T,Ctrl+R)
