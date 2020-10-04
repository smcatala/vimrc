# Customized Awesome Vimrc
## installation
requires `nvim >= 0.4.3`, as per [nvim installation instructions](https://github.com/neoclide/coc.nvim/wiki/Install-coc.nvim).

```bash
git checkout custom
git submodule update --init --recursive
```
note that submodule remotes are `git:github.com` urls,
which require ssh access to github.

`yarn` is required by `coc.nvim`:
```bash
npm i -g yarn
```

on the first launch of `vi`, initialize `coc.nvim`
and add typical extensions:
```vi
:call coc#util#install()
:CocInstall coc-json coc-yaml coc-html coc-css coc-tsserver coc-jedi coc-java coc-go
```

## features
adds the following plugins:
* auto-pairs
* coc.nvim
* gitsession
* nerdtree-git-plugin
* tagbar
* vim-fahrenheit
* vim-farout (default colorscheme)
* vim-jsx-pretty
* vim-startify (`<leader>;`)

