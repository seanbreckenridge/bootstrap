# bootstrap

A script to setup a new `bash` VPS/servers with defaults I like.

Can be run repeatedely to update from newly pushed changes to this repo.

Run:

```
bash -c "$(curl -fsSL https://raw.githubusercontent.com/seanbreckenridge/bootstrap/master/bootstrap)"
```

Or, shorter (just redirects to the link above) in case I need to type it out:

```
bash -c "$(curl -sL sean.fish/s/b)"
```

Any additional bash customization gets put in `~/.bash_ext`

### Requires:

- `curl`
- `git`

On a debian-based server, that can typically be satisfied like: `apt update && apt install curl git`

### Features:

Prompts you to build neovim from scratch (on a debian-like system), which you could also do with:

```
bash -c "$(curl -fsSL https://raw.githubusercontent.com/seanbreckenridge/bootstrap/master/build_neovim)"
```

- Sets some default environment variables:
  - Color/Language Options
  - `PS1` (prompt)
- Sets some basic aliases (`ls`/`ll`/git related aliases/`e` to `nvim`)
- prompts user to set global name, username and sets default editor for `git`
- neovim: clones my dotfiles to ~/.dotfiles and `rsync`s my neovim configuration, adds a `nvim_update_config` function to sync it later
- Installs fzf, sets up fzf integration (Ctrl+T,Ctrl+R)
