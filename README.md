Introduction
==========
Ruby-Block is an elisp minor-mode designed for use with ruby-mode.
When the cursor is located on or after an 'end' token, Ruby-Block will automatically
show you the corresponding line with the start of the block.

Usage:
==========
To use, simply add this line to your .emacs:
```
(require 'ruby-block)
(ruby-block-mode t)
```
In addition, you can specify whether to either highlight (overlay) or display to the minibuffer with:
```
;; do overlay
(setq ruby-block-highlight-toggle 'overlay)
;; display to minibuffer
(setq ruby-block-highlight-toggle 'minibuffer)
;; display to minibuffer and do overlay
(setq ruby-block-highlight-toggle t)
```
The default is minibuffer.

Version Info
==========

Tested on Emacs 24.3

Note:
A ruby-mode.el or enh-ruby-mode is necessary to use this package.
