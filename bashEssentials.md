# .bash_aliases:

# Reload this file:
alias bash='source ~/.bash_profile'

# Enable programmable completion features.
if [ -f /etc/bash_completion ]; then
    source /etc/bash_completion
fi

# GLOBAL ALIASES
alias ll='ls -lFGa'
alias wget='curl -O'

# show hiden files:ed
alias shf='defaults write com.apple.finder AppleShowAllFiles TRUE;killall Finder'
# hide hiden files:
alias hhf='defaults write com.apple.finder AppleShowAllFiles FALSE;killall Finder'

# .bash_profile:

# Alias definitions:
if [ -f ~/.bash_aliases ]; then
    . ~/.bash_aliases
fi

export GOROOT=/usr/local/go
export GOPATH=~/go
export GOREPOSITOY=~/go/bin
export PATH=$PATH:$GOPATH/bin

C_DEFAULT="\[\033[m\]"
C_CYAN="\[\033[36m\]"
C_BLUE="\[\033[34m\]"

export PS1="$C_CYAN\u@$C_BLUE\h $C_CYAN\w\n$> $C_DEFAULT"