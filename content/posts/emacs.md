---
draft: true
date: 2025-02-08
title: Emacs
---
Warning: This article is not a guide to learning Emacs. It's just my personal notes on setting it up for myself. I might reference it if I stop using Emacs and decide to try it again.

I'm not really an Emacs user, but I've wanted to try it out for a long time. I don’t know much about Lisp or how Emacs works, but I'll learn as I write this article.

First, I need to install it

```bash
sudo pacman -S emacs
```

As far as I know, the startup file is `~/.config/emacs/init.el`. I'm aware of `~/.emacs`, but I'll keep the config file in the config directory instead.

```lisp
;; MELPA
(require 'package)
(add-to-list 'package-archives '("melpa" . "https://melpa.org/packages/") t)
(package-initialize)
```

The first thing I want to set up is the MELPA repository. I'm not entirely sure if I need it, but I'll keep it for now. As I set up each package, I'll check whether it requires MELPA. If none of them do, I'll remove this block.
