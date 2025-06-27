# Ensure history is saved
export HISTFILE=~/.bash_history
export HISTSIZE=10000
export HISTFILESIZE=20000
shopt -s histappend
PROMPT_COMMAND="history -a; history -n"
# Enable colors for ls
alias ls='ls --color=auto'
alias grep='grep --color=auto'
alias fgrep='fgrep --color=auto'
alias egrep='egrep --color=auto'
# PS1 for colorful prompt
export PS1="\[\e[32;1m\]\u@\h\[\e[0m\]:\[\e[34;1m\]\w\[\e[0m\]\$ "
# PS1 with time and colors
export PS1="\[\e[33m\]\D{%H:%M}\[\e[0m\] \[\e[32;1m\]\u@\h\[\e[0m\]:\[\e[34;1m\]\w\[\e[0m\]\$ "
# PS1 with emoji (requires font support)
export PS1="\[\e[32;1m\]\u@Termux \[\e[34m\]\w \[\e[36m\]\$ \[\e[0m\]"
