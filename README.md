[![MELPA](http://melpa.org/packages/ace-jump-zap-badge.svg)](http://melpa.org/#/ace-jump-zap)
[![MELPA Stable](http://stable.melpa.org/packages/ace-jump-zap-badge.svg)](http://stable.melpa.org/#/ace-jump-zap)

## Ace Jump Zap ##

`ace-jump-zap` provides the functionality of [`zap-to-char`](http://www.emacswiki.org/emacs/ZapToChar) and [`zap-up-to-char`](http://www.emacswiki.org/emacs/ZapUpToChar) using [`ace-jump-mode`](https://github.com/winterTTr/ace-jump-mode). In a nutshell, you may trigger a key-binding to launch `ace-jump-char-mode` to vaporize all characters between the cursor and the selected character.

### Installation ###

Recommended install from [MELPA](melpa.milkbox.net) with `M-x package-install ace-jump-zap`.

### Commands ###

Bind `(ace-jump-zap-to-char)` or `(ace-jump-zap-up-to-char)` to the key-binding of your heart's desire and zap away.

Alternatively, you can bind the helper functions `(ace-jump-zap-to-char-dwim)` and `(ace-jump-zap-up-to-char-dwim)`. Calling them interactively will trigger `(zap-to-char)` and `(zap-up-to-char)` respectively, but with a prefix it will call the `ace-jump-zap` version.

### Variables ###

###### `ajz/zap-function` ######

This is the function used for zapping between point and char. The default is `'delete-region` but it could also be `'kill-region`.

###### `ajz/forward-only` ######

Set to non-nil to choose to only zap forward from the point. Default will zap in both directions from the point in the current window.

###### `ajz/sort-by-closest` ######

Non-nil means sort the zap candidates by proximity to the current point. Set to nil for the default `ace-jump-mode` ordering. Enabled by default as of 0.1.0.

###### `ajz/52-character-limit` ######

Set to non-nil to limit zapping reach to the first 52 characters. This is only really useful with `ajz/sort-by-closest` set to non-nil. Enabled by default as of 0.1.0.

