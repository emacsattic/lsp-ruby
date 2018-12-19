# DEPRECATED

You do not need this package anymore! Just use `lsp-mode` directly. Read [the docs](https://github.com/emacs-lsp/lsp-mode/#configuration).

tl;dr:

```
(package-install 'lsp-mode)

(require 'lsp)
(require 'lsp-clients)

(add-hook 'ruby-mode-hook 'lsp)

;; For dropdown autocomplete:
;; (package-install 'company)
;; (package-install 'company-lsp)
;; (require 'company)
;; (require 'company-lsp)
;;
;; For other fancy UI stuff:
;; (package-install 'lsp-ui)
;; (require 'lsp-ui)
```


lsp-ruby
========

Ruby support for lsp-mode using the [solargraph gem](https://github.com/castwide/solargraph).

## News

Note: if you recently started getting an error like `Could not find command "stdio".`, run `gem update solargraph`.

## Installation

### From source

Clone this repository and [lsp-mode](https://github.com/emacs-lsp/lsp-mode) to
suitable paths, and add them to your load path:

```emacs-lisp
(add-to-list 'load-path "<path to lsp-mode>")
(add-to-list 'load-path "<path to lsp-ruby>")
```

### From MELPA

Install the packages:
- `lsp-mode`
- `lsp-ruby`

## Usage
### Enabling `lsp-ruby`

```emacs-lisp
(require 'lsp-ruby)
(add-hook 'ruby-mode-hook #'lsp-ruby-enable)

;; Optional, for short messages on hover:
;; (setq lsp-hover-text-function 'lsp--text-document-signature-help)
```

### Install the server

```
gem install solargraph
```
