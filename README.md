### Ace Jump Zap

`ace-jump-zap` provides the functionality of [`zap-to-char`](http://www.emacswiki.org/emacs/ZapToChar) and [`zap-up-to-char`](http://www.emacswiki.org/emacs/ZapUpToChar) using [`ace-jump-mode`](https://github.com/winterTTr/ace-jump-mode). In a nutshell, you may trigger a key-binding to launch `ace-jump-char-mode` to vaporize all characters between the cursor and the selected character.

#### Installation

Install from [MELPA](melpa.milkbox.net) with `package-install ace-jump-zap`, or drop `ace-jump-mode.el` and `ace-jump-zap.el` into your load path.

#### Usage

Bind `(ace-jump-zap-to-char)` or `(ace-jump-zap-up-to-char)` to the key-binding of your heart's desire and zap away.

Alternatively, you can bind the helper functions `ace-jump-zap-to-char-dwim` and `ace-jump-zap-up-to-char-dwim``. These default to their ordinary-but-speedy versions. However, given a prefix argument, they transform into their upgraded, super-powered, ace-jump-amplified variants. Zap away as you please, with haste and/or precision!
