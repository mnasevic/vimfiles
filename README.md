# vimfiles

Personalized vim configuration.

## Plugins

* https://github.com/tpope/vim-pathogen
* https://github.com/tpope/vim-rails
* https://github.com/tpope/vim-rake
* https://github.com/tpope/vim-bundler
* https://github.com/tpope/vim-fugitive
* https://github.com/tpope/vim-haml
* https://github.com/tpope/vim-surround
* https://github.com/tpope/vim-endwise
* https://github.com/tpope/vim-commentary
* https://github.com/tpope/vim-cucumber
* https://github.com/tpope/vim-markdown
* https://github.com/scrooloose/nerdtree
* https://github.com/corntrace/bufexplorer
* https://github.com/ervandew/supertab
* https://github.com/mnasevic/snipmate.vim
* https://github.com/mnasevic/snipmate-snippets
* https://github.com/vim-ruby/vim-ruby
* https://github.com/mileszs/ack.vim
* https://github.com/altercation/vim-colors-solarized.git
* https://github.com/kien/ctrlp.vim
* https://github.com/benmills/vimux
* https://github.com/skalnik/vim-vroom
* https://github.com/Lokaltog/vim-easymotion
* https://github.com/tpope/vim-ragtag
* https://github.com/pangloss/vim-javascript
* https://github.com/othree/javascript-libraries-syntax.vim
* https://github.com/godlygeek/tabular
* https://github.com/bogado/file-line
* https://github.com/rodjek/vim-puppet
* https://github.com/ekalinin/Dockerfile.vim
* https://github.com/fatih/vim-go
* https://github.com/editorconfig/editorconfig-vim
* https://github.com/prettier/vim-prettier

## Installation

```sh
sudo apt install vim-gtk3 #install vim (replacement for vim-gnome with +clipboard)
sudo apt-get install exuberant-ctags ncurses-term xsel
git clone git@github.com:mnasevic/vimfiles.git ~/.vim
cd ~/.vim
git submodule update --init
echo "source ~/.vim/vimrc" > ~/.vimrc
```

### For vim-prettier plugin only (to make Prettier: executable)
```sh
cd ~/.vim/bundle/vim-prettier
npm install
```

### Adding a new plugin

```
git submodule add https://github.com/<username>/<plugin>.git bundle/<plugin>
```

### Updating plugins

```sh
# Update to newest vimiles
cd ~/.vim
git pull origin master

# Update all submodules
git submodule update --init
git submodule sync
git submodule foreach git pull origin master

# Generate documentations for bundled plugins
:Helptags
```
