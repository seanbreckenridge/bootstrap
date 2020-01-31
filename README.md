# bootstrap

A script to setup a new `bash` VPS/servers with defaults I like.

Run:

```
bash -c "$(curl -fsSL https://raw.githubusercontent.com/seanbreckenridge/bootstrap/master/bootstrap)"
```

### Requires:

- `curl`
- `git`
- `vim`

### Features:

- Sets some default environment variables:
  - Color/Language Options
  - `PS1` (prompt)
- Sets some default aliases (`ls`/`ll`/git related aliases)
- `e` to `vim`
- sets lots of `vim` defaults
- installs [`vim-plug`](https://github.com/junegunn/vim-plug) (`vim` plugin manager)
- prompts user to set global name, username and sets default editor for `git`

