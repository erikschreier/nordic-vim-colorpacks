# nordic-vim-colorpacks
modified colors for nordic-vim

### What is it?
There are two optional surface files to choose for the nordic-vim setup. A Papercolor and a JellyBeans file fully configured and ready to use.

## .vimrc.surface_pc (PaperColor)

<a href="https://i.imgur.com/zWHwTWO.png">
  <img src="https://imgur.com/zWHwTWOl.png" />
</a>


## .vimrc.surface_jb (JellyBeans)

<a href="https://i.imgur.com/pURXtiP.png">
  <img src="https://imgur.com/pURXtiPl.png" />
</a>


### How to install?
If you want to use one of the themes just clone the Repo to your homefolder and move the file inside of your ~/.vim folder.

    $ git clone https://github.com/erikschreier/nordic-vim-colorpacks
    $ mv nordic-vim-colorpacks/.vimrc.surface_jb ~/.vim/
    $ mv nordic-vim-colorpacks/.vimrc.surface_pc ~/.vim/
    $ rm -rf nordic-vim-colorpacks
    
Next step is to add the Colorscheme to your Plugins using Vundle, open your ~/.vim/.vimrc.plugins file and add the plugin right under the nord-vim plugin in the Colorschemes section.

    $ vim ~/.vim/.vimrc.plugins
    
    ...
    40 " Colorschemes
    41 "------------------------------------------------------------------------------
    42 Plugin 'arcticicestudio/nord-vim'      " arctic, north-bluish vim colorscheme
    43 Plugin 'NLKNguyen/papercolor-theme'    " inspired by googles material design    
    44 Plugin 'nanotech/jellybeans.vim'       " a colorful dark colorscheme  
    45 "==============================================================================
    
Last step is to open your ~/.vimrc and replace line 12 with the file you want to use.

    $ vim ~/.vimrc
    
    ...
    11 source ~/.vim/.vimrc.aufiles           " autocommands                           
    12 source ~/.vim/.vimrc.surface_pc        " Colorscheme and Statusbar              
    13 "==============================================================================
