# emacs-load-env-vars

[![Build Status](https://travis-ci.org/diasjorge/emacs-load-env-vars.svg?branch=master)](https://travis-ci.org/diasjorge/emacs-load-env-vars)
[![Coverage Status](https://coveralls.io/repos/github/diasjorge/emacs-load-env-vars/badge.svg?branch=improvements)](https://coveralls.io/github/diasjorge/emacs-load-env-vars?branch=improvements)
[![MELPA](http://melpa.milkbox.net/packages/load-env-vars-badge.svg)](http://melpa.milkbox.net/#/load-env-vars)

A package to load environment variable files into emacs

## Installation

If you use use-package.

```elisp
(use-package load-env-vars)
```

## Usage

Just execute `M-x load-env-vars` and point to your env file.

### Programatic usage


`load-env-vars-from-string` can be used to load environment variables from secrets managers or similar tools:


```elisp
;; using some 1Password CLI:
(load-env-vars-from-string (shell-command-to-string "op inject -i ./secrets.env.tmpl"))
```

## Supported Syntax

Check [env.example](env.example) for supported syntax
