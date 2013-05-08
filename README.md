Vim Terminal Colors
==================
It's a collection of colors that can be used in terminal mode, rather than only in GUIs.

Thanks to [gui2term project](http://www.vim.org/scripts/script.php?script_id=2778), I can use my favorite color in terminal(gnome-terminal or kde-konsole).

Fork me to provide your favorite color! Or just tell me the color name.

You can simply add `Bundle 'lufeihaidao/vim-term-color'` to your `.vimrc` file if you choose [vundle](https://github.com/gmarik/vundle) to manage your vim plugins. Then put this code snippet to your `.vimrc` file:

``` bash
" use 256 colors when possible
if &term =~? 'mlterm\|xterm\|screen-256'
	let &t_Co = 256
    colorscheme your-color-scheme_term
else
    colorscheme other-color-scheme
endif

" colors for gvim
if has('gui_running')
    colorscheme your-color-scheme
endif
```
