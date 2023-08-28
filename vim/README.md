Let's break down what each line does:

- `set nocompatible`: Turns off compatibility with `vi`, the predecessor to `vim`. This enables `vim`'s extended feature set.
- `filetype on`: Enables file type detection. This allows `vim` to adjust its behavior based on the type of file you're editing.
- `filetype plugin on`: Enables loading of plugins for specific file types.
- `filetype indent on`: Enables automatic indentation based on file type.
- `set tabstop=4`, `set shiftwidth=4`, `set expandtab`: These commands configure `vim` to use spaces instead of tabs for indentation, and to use an indentation level of 4 spaces.
- `set number`: Enables line numbers.
- `set cursorline`: Highlights the line the cursor is on.
- `set ignorecase`: Makes searching case insensitive.
- `set incsearch`: Enables incremental searching, so `vim` starts searching as you type.
- `syntax enable`: Enables syntax highlighting.

## Vim Plugins
Install [Vim-Plug](https://github.com/junegunn/vim-plug)

```bash
$ curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

Then install plugins from [Vim Awesome](https://vimawesome.com/). 

#### Example installing Emmet

Place this in your .vimrc:

```
Plug 'mattn/emmet-vim'
```
… then run the following in Vim:
```
:source %
:PlugInstall
```
