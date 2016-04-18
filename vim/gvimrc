set number                  " Turn on line numbers
syntax enable               " Enable syntax highlighting
set scrolloff=10            " Set number of lines always visible above/below cursor
set t_Co=256                " Set number of colors
colorscheme zenburn         " Set colorscheme

set tw=80                   " Set number of text columns
set lines=40 columns=100    " Set default window size

" Put backup files in /tmp instead of the local directory
set backupdir=~/.tmp/vimtemp

" Hide the menu/tool bars. Press F2 to show/hide
set guioptions-=m
set guioptions-=T
map <silent> <F2> :if &guioptions =~# 'T' <Bar>
\set guioptions-=T <Bar>
\set guioptions-=m <bar>
\else <Bar>
\set guioptions+=T <Bar>
\set guioptions+=m <Bar>
\endif<CR>


set guioptions-=r
set guioptions-=R
set guioptions-=l
set guioptions-=L

set guitablabel=%t

set showmatch

set autoindent
"set smartindent
"set cindent

set tabstop=2
set softtabstop=2
set shiftwidth=2
set expandtab

"" [un]comment out blocks of text in Vim
"map ,% :s/^/%/<CR>
"map ,c :s/^\/\/\\|^--\\|^> \\|^[#"%!;]//<CR>

""filetype plugin on

""" Python-specific options
""autocmd FileType python set complete+=k~/.vim/syntax/python.vim isk+=.,(
""" These should be modified so that this mapping only works on .py files
""map <buffer> <F5> :w<CR>:!python % <CR>
""map <buffer> <F4> :w<CR>:!pep8 % <CR>
""let g:pydiction_location = '/home/bdol/.vim/ftplugin/pydiction/complete-dict'

"" Latex-specific options
""let g:tex_flavor='latex'
""let g:Tex_DefaultTargetFormat='pdf'
""filetype indent on
""call IMAP('`B', '$\Beta$', 'tex')
""call IMAP('`o', '$\Omega$', 'tex')
""call IMAP('FHR', "\\fighere{<++>}{<++>}{%\<CR><++>\<CR>}", 'tex')
""call IMAP('FRF', 'Figure~\ref{<++>}<++>', 'tex')

" Set copy/paste to behave like Windows
source $VIMRUNTIME/mswin.vim
behave mswin

" LaTeX (rubber) macro for compiling
nnoremap <leader>c :w<CR>:!rubber --pdf --warn all %<CR>

" View PDF macro; '%:r' is current file's root (base) name.
nnoremap <leader>v :!xdg-open %:r.pdf &<CR><CR>

