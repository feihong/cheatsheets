# Spacemacs

## Installation

```
brew tap d12frosted/emacs-plus
brew install emacs-plus
git clone https://github.com/syl20bnr/spacemacs ~/.emacs.d
brew tap caskroom/fonts && brew cask install font-source-code-pro
```

1. Open Emacs
1. Choose default editing style (evil)
1. Choose standard distribution
1. Choose full-featured completion framework (helm)
1. Emacs will automatically download and install packages
1. Open .spacemacs file (SPC f e d)
1. Make sure these lines are present/uncommented under dotspacemacs-configuration-layers:
   
       clojure
       helm
       auto-completion
       better-defaults
       emacs-lisp
       git
       html
       javascript
       markdown
       org
       (shell :variables
              shell-default-height 30
              shell-default-position 'bottom)
       syntax-checking
       version-control
1. The javascript layer expects tern.js to be installed, so to avoid seeing errors on startup you should run `npm install -g tern`.

## Switch to dev branch

      cd ~/.emacs.d
      git checkout develop
      
To update on develop branch

1. Select `[Update Packages]` on start screen
1. Close Emacs
1. `cd ~/.emacs.d; git pull --rebase`

Sources:

- [Beginner's tutorial](https://github.com/syl20bnr/spacemacs/blob/master/doc/BEGINNERS_TUTORIAL.org)
- [Use homebrew to install emacs](https://github.com/syl20bnr/spacemacs#macos)
- [Use homebrew to install source code pro font](https://github.com/adobe-fonts/source-code-pro#font-installation-instructions)
- [How to switch to dev branch?](https://www.reddit.com/r/spacemacs/comments/79xkfa/how_do_i_switch_to_the_dev_branch/)
- [Update on develop branch](https://github.com/syl20bnr/spacemacs#on-develop-branch)
