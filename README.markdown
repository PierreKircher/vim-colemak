vim-colemak
===========

Colemak key mappings for Vim. Trimmed and modified version of [Shai Coleman's configuration](http://colemak.com/pub/vim/colemak.vim).

Install
-------

1. Use [vim-plug](https://github.com/PierreKircher/vim-plug).
2. Add to `.vimrc`: `Plug 'PierreKircher/vim-colemak'`
3. Run `vim +PlugInstall`
4. You probably want to load vim-colemak last. Reload the plugin at the bottom of your Vim configuration.

    ```
    " Reload vim-colemak to remap any overridden keys
    silent! source "$HOME/.vim/bundle/vim-colemak/plugin/colemak.vim"
    ```

    *Note: You might be using `~/.vim/plugged`.*


Key mappings
------------

```
Colemak layout:                  |                 QWERTY layout:
`12345 67890-=     Move around:  |  (instead of)   `12345 67890-=
 qwfpg jluy;[]\         e        |       k          qwert yuiop[]\
 arstd HNEIo'         h   i      |     h   l        asdfg HJKL;'
 zxcvb km,./            n        |       j          zxcvb nm,./

(  novx)  h = h (Left)     i = l (Right)     e = k (Up)     n = j (Down)

(  novx)  l = b (Back word)            L = B (Back WORD)
(  novx)  y = w (Forward word)         Y = W (Forward WORD)
(  novx)  u = e (Forward end of word)  U = E (Forward end of WORD)

(c     )  <C-L> = <C-Left> (Back WORD)
(c     )  <C-Y> = <C-Right> (Seems to equal forward WORD minus 1 character)

(  n  x)  a = v (Visual)   A = V (Visual line)
(  n   )  r = r (Replace)  R = R (Replace)
(  n   )  s = i (Insert)   S = I (Insert before first non-blank of line)
(  n   )  t = a (Append)   T = A (Append at end of line)
(  n   )  w = c (Change)   W = C (Change to end of line)  ww = cc (Change line)

(  n  x)  z = u (Undo)    Z = <C-R> (Redo)  gz = U (Undo all latest changes on line)
(  n  x)  x = x (Cut)     X = dd (Cut line)
(  n  x)  c = y (Copy)    C = yy (Copy line)
(  n  x)  v = p (Paste)   V = P (Paste)
(  n  x)  gv = gp (Paste) gV = gP (Paste)

(   o  )  r = i (Example: dip -> drp (Delete inner paragraph))

(  no x)  p = t{char} (Before next {char})  P = T{char} (After previous {char})
(  no x)  b = ; (Repeat latest f or t)  B = , (Repeat latest f or t reversed)
(  no x)  k = n (Repeat latest / or ?)  K = N (Repeat latest / or ? reversed)

(  n  x)  j = z
(  n  x)  jn = zj (Next fold) [Also jj = zj]
(  n  x)  je = zk (Previous fold) [Also jk = zk]

(  n   )  ga = gv (Reselect last visual selection)
(  n  x)  gK = K (Lookup)
(  n  x)  gL = L (To line [count] from bottom of window)

(  n  x)  <C-W>h = <C-W>h (Window left)
(  n  x)  <C-W>n = <C-W>j (Window down)
(  n  x)  <C-W>e = <C-W>k (Window up)
(  n  x)  <C-W>i = <C-W>l (Window right)

Lost:
(  n  x)  H (To line [count] from top of window)
(  n  x)  s (Substitute [count] characters) [Use wi = cl]
(  n  x)  S (Substitute [count] lines) [Use ww = cc]
(  n  x)  X (Cut [count] characters backwards) [Use dh = dh]
(  n   )  Z (Quit)
(  n  x)  <C-W>n (Window down) [Use <C-W><C-N> = <C-W><C-N>]
(  n  x)  <C-W>i (Window down) [Use <C-W><C-I> = <C-W><C-I>]

Legend:
<C-X>     Ctrl-X
(c     )  Command-line mode
( i    )  Insert mode
(  n   )  Normal mode
(   o  )  Operator pending
(    v )  Visual+Select mode
(     x)  Visual mode
```

