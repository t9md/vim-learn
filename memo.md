# normal
`S`, `cc` same meaning, you can get rid of one of it.  
`f`,`F` find char *forward* and *backword*  
`t`,`T` Till char *forward* and *backword*  
`&` Repeat `:s` substitution.  
`gJ` Join lines without space.  
`;` repeat `tTfF`.  
`"` specify register  
`'` got to mark BOL  
`N|` go to Ncol. `3l` go to col3  
`\` not used! free!  
`Z` quit (free)  
`x` Delete  
`X` Backspace  

# Operator
`=` auto format  
`y` yank  
`d` delete  
`c` cahange  
`<` un-indent  
`>` indent  

# Special
`Z`, `z`, `1-9,0`, `"`, `\`, `g`, 

# Page
`<C-f>`, `<C-b>`
`<C-d>`, `<C-u>`


text-obj とは object なので、目的語になる。
つまり
* textobj →subject(目的語)
* operator →verb(動詞)

y(ヤンクせよ)ae(バッファ全体を)
=(インデントせよ)if(innner functionを)

# TextObj

* 'kana/vim-textobj-function'
function textobj を作るための api を提供
	af	<Plug>(textobj-function-a)
	if	<Plug>(textobj-function-i)

C, vim が実例として定義されている。

* 'kana/vim-textobj-indent'
	ai	<Plug>(textobj-indent-a)
	ii	<Plug>(textobj-indent-i)
	aI	<Plug>(textobj-indent-same-a)
	iI	<Plug>(textobj-indent-same-i)

* 'kana/vim-textobj-line'
    vo	al		<Plug>(textobj-line-a)
    vo	il		<Plug>(textobj-line-i)

* 'kana/vim-textobj-lastpat'
a,iの違いは無い。
	a/	<Plug>(textobj-lastpat-n)
	i/	<Plug>(textobj-lastpat-n)
	a?	<Plug>(textobj-lastpat-N)
	i?	<Plug>(textobj-lastpat-N)

* 'kana/vim-textobj-entire'
vae vie バッファ全体を選択
	ae	<Plug>(textobj-entire-a)
	ie	<Plug>(textobj-entire-i)
* 'kana/vim-textobj-jabraces'
日本語文字の『 とかをASCII文字で選択できるところがミソ

* 'kana/vim-textobj-fold'
	az	<Plug>(textobj-fold-a)
	iz	<Plug>(textobj-fold-i)

* 'kana/vim-textobj-syntax'
	ay	|<Plug>(textobj-syntax-a)|		*ay* *v_ay*
	iy	|<Plug>(textobj-syntax-i)|		*iy* *v_iy*

* 'kana/vim-textobj-diff'

# Operator
* 'kana/vim-operator-user'
* 'kana/vim-operator-replace'
