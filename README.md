# Overview

This package provides an interface to xref based on `completing-read`.  It is a shameless clone of [ivy-xref](https://github.com/alexmurray/ivy-xref) that uses `completing-read` instead of ivy. It is intended to work well with [selectrum](https://github.com/raxod502/selectrum).

# Usage

```
(use-package completing-read-xref
  :straight (completing-read-xref :type git :host github :repo "travitch/completing-read-xref.el")
  :commands (completing-read-xref-show-xrefs completing-read-xref-show-xrefs)
  :init
  (setq xref-show-definitions-function 'completing-read-xref-show-defs))
```
