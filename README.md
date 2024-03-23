# latexkeys
This is a keyboard configuration using [KMonad](https://github.com/kmonad/kmonad)
This branch uses right control for the `com` key.

## Index
The key that switches to the LaTeX configuration is refered to as com and is AltGr by default (you may consider changing this if you are already using AltGr as part of your keyboard layout). Other important keys are shift (either left or right) and g (for greek letters).

| shortcut | description |
| -------- | -------- |
| com+4 | inline math mode |
| com+5 | display math mode |
| com+9 or com+0 | parentheses |
| com+[ or com+] | square brackets |
| com+{ or com+} | braces |
| com+< or com+> | angle brackets |
| com+\| | vertical bar brackets |
| com+f | fraction |
| com+q | square root |
| com+l | limit |
| com+s | series |
| com+i | definite integral |
| com+e | equation environment |
| com+a | align environment |
| com+b | mathbb |
| com+v | mathbf |
| com+r| ref |
| com+c | cite |
| com+g+... | various greek letters |
| com+shift+g+... | various capital greek letters |

## How to Use
See KMonad [installation](https://github.com/kmonad/kmonad/blob/master/doc/installation.md) instructions. Then run (for example)
```bash
git clone https://github.com/tinjano/latexkeys
sudo /home/tinjano/.local/bin/kmonad config.kbd
```
To use it on startup, see `kmonad.service` and place it in `etc/sysyemd/system/`.

## Notes
- in `config.kbd`, change `device-file` to your own keyboard's id
- in `kmonad.service`, change `ExecStart` to your own files' locations
- if you are using Overleaf or a similar environment, consider turning off automatic closing of brackets and similar features where interference may happen
- add shortcuts right for you and send a pull request if they are compatible
