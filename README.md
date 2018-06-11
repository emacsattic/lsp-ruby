lsp-ruby
========

Ruby support for lsp-mode using the [language_server gem](https://github.com/mtsmfm/language_server-ruby).

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
```

### Install the server

```
gem install language_server
```
