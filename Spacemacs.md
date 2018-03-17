# Spacemacs

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
       parinfer
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


Sources:

- [Beginner's tutorial](https://github.com/syl20bnr/spacemacs/blob/master/doc/BEGINNERS_TUTORIAL.org)
- [Use homebrew to install emacs](https://github.com/syl20bnr/spacemacs#macos)
- [Use homebrew to install source code pro font](https://github.com/adobe-fonts/source-code-pro#font-installation-instructions)
