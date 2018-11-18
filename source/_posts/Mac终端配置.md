---
title: Mac终端配置
date: 2018-10-18 19:15:41
tags:
categories:
- 技术笔记

---

```
# alias
alias ll="ls -lhvG"
alias lla="ls -alhvG"

function git_branch {
      ref=$(git symbolic-ref HEAD 2> /dev/null) || return;
      echo "("${ref#refs/heads/}")";
}

export PS1="[\[\e[31m\]\u@\[\e[32m\]\w\[\033[1;36m\]\$(git_branch)\[\e[0m\]]\$"
```
