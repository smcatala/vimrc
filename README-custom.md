# Customized Awesome Vimrc
## dependencies
requires `nvim >= 0.4.3`, as per [nvim installation instructions](https://github.com/neoclide/coc.nvim/wiki/Install-coc.nvim).

also, some of the plugins require the following dependencies:
```bash
sudo apt install libxext-dev # optionally required by ueberzug
pip3 install ranger-fm pynvim ueberzug # required by rnvimr
```

additionally, [bat](https://github.com/sharkdp/bat) is a useful cat clone and pager,
complementary to nvim in the terminal.
```bash
sudo apt install batcat # ubuntu 20.04
echo "alias bat='batcat --tabs=2'" >> ~./bash_aliases
```

## installation
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
* rnvimr
* tagbar
* vim-fahrenheit
* vim-farout (default colorscheme)
* vim-floaterm
* vim-jsx-pretty
* vim-startify (`<leader>;`)

