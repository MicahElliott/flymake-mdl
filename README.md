# flymake-mdl, a markdown linter for Emacs

Lint your markdown files with
[flymake](https://www.gnu.org/software/emacs/manual/html_node/flymake/index.html)
(built into Emacs)
and the best markdown linter,
[markdownlint](https://github.com/markdownlint/markdownlint), AKA `mdl` (the
ruby version that's easy to install and configure).

But note that `mdl` is a little slow, so you might want to
[only run flymake on save](https://stackoverflow.com/questions/6110691/is-there-a-way-to-make-flymake-to-compile-only-when-i-save).

## Usage

```lisp
(add-hook 'markdown-mode-hook #'flymake-mode)
(require 'flymake-mdl)
(add-hook 'markdown-mode-hook 'flymake-mdl-setup)
```
