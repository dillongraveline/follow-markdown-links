# follow-markdown-links

> Modified to work with Obsidian-like link structures.

This vim plugin enables browsing through your markdown files by using links between them (like a personal wiki). You just have to move the cursor to a link and press SPACE.

Example of links

- `[[Notes]]` will open Notes.md
- `[[sub/Notes]]` will open sub/Notes.md (if `sub` directory does not exist, the plugin will prompt for confirmation and create)

You can press BACKSPACE to navigate to previous file (like "e#").

## Installation

Use your plugin manager of choice.

- [Pathogen](https://github.com/tpope/vim-pathogen)
  - `git clone https://github.com/dillongraveline/follow-markdown-links ~/.vim/bundle/follow-markdown-links`
- [Vundle](https://github.com/gmarik/vundle)
  - Add `Bundle 'https://github.com/dillongraveline/follow-markdown-links'` to .vimrc
  - Run `:BundleInstall`
- [NeoBundle](https://github.com/Shougo/neobundle.vim)
  - Add `NeoBundle 'https://github.com/dillongraveline/follow-markdown-links'` to .vimrc
  - Run `:NeoBundleInstall`
- [vim-plug](https://github.com/junegunn/vim-plug)
  - Add `Plug 'https://github.com/dillongraveline/follow-markdown-links'` to .vimrc
  - Run `:PlugInstall`

## Configuration

Add `autocmd FileType markdown nnoremap <Space> :FollowLink<CR>` to your .vimrc

## Credit
Credits to prashanthellina for creating this plugin.
