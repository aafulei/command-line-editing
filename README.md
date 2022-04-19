# Command-Line Editing Cheatsheet

> *For Bash. Compatible with most other shells.*

- Get the PDF version [`here`](https://github.com/aafulei/command-line-editing/raw/main/command-line-editing-cheatsheet.pdf)

## Move

| Key Binding                     | Action                                           |
| ------------------------------- | ------------------------------------------------ |
| <kbd>Ctrl</kbd> + <kbd>A</kbd>  | Move to Line Begin                               |
| <kbd>Ctrl</kbd> + <kbd>E</kbd>  | Move to Line End                                 |
| <kbd>Ctrl</kbd> + <kbd>B</kbd>  | Move Back One Character                          |
| <kbd>Meta</kbd> + <kbd>B</kbd>  | Move Back One Word                               |
| <kbd>Ctrl</kbd> + <kbd>F</kbd>  | Move Forward One Character                       |
| <kbd>Meta</kbd> + <kbd>F</kbd>  | Move Forward One Word                            |

## Delete

| Key Binding                    | Action                                            |
| ------------------------------ | ------------------------------------------------- |
| <kbd>Ctrl</kbd> + <kbd>H</kbd> | Delete One Character Before Cursor                |
| <kbd>Ctrl</kbd> + <kbd>D</kbd> | Delete One Character At Cursor                    |

## Kill & Yank

| Key Binding                    | Action                                            |
| ------------------------------ | ------------------------------------------------- |
| <kbd>Ctrl</kbd> + <kbd>U</kbd> | Kill from Cursor to Line Begin                    |
| <kbd>Ctrl</kbd> + <kbd>K</kbd> | Kill from Cursor to Line End                      |
| <kbd>Ctrl</kbd> + <kbd>W</kbd> | Kill from Cursor to Previous Whitespace           |
| <kbd>Meta</kbd> + <kbd>Backspace</kbd> | Kill from Cursor to Word Begin            |
| <kbd>Meta</kbd> + <kbd>D</kbd> | Kill from Cursor to Word End                      |
| <kbd>Ctrl</kbd> + <kbd>Y</kbd> | Yank - Put Killed Text Back at Cursor             |
| <kbd>Meta</kbd> + <kbd>Y</kbd> | Yank-pop - Rotate Kill-Ring, and Put Back New Top |

## History

| Key Binding                    | Action                                            |
| ------------------------------ | ------------------------------------------------- |
| <kbd>Ctrl</kbd> + <kbd>R</kbd> | Reverse History Search                            |
| <kbd>Ctrl</kbd> + <kbd>S</kbd> | Forward History Search                            |
| <kbd>Ctrl</kbd> + <kbd>G</kbd> | Abort History Search, and Restore                 |

## Others

| Key Binding                    | Action                                            |
| ------------------------------ | ------------------------------------------------- |
| <kbd>Ctrl</kbd> + <kbd>-</kbd> | Undo                                              |
| <kbd>Ctrl</kbd> + <kbd>X</kbd> &nbsp; <kbd>Ctrl</kbd> + <kbd>U</kbd> | Undo        |
| <kbd>Ctrl</kbd> + <kbd>C</kbd> | Send `SIGINT` (Cancel)                            |
| <kbd>Ctrl</kbd> + <kbd>D</kbd> | Send `EOF`                                        |
| <kbd>Ctrl</kbd> + <kbd>J</kbd> | Send `Line Feed`                                  |
| <kbd>Ctrl</kbd> + <kbd>L</kbd> | Clear Screen, and Reprint Current Line            |

## FAQ

### How to invoke <kbd>Meta</kbd>?

Press <kbd>Alt</kbd> or <kbd>Option</kbd>. Alternatively, press <kbd>Esc</kbd> first, and then press the key it modifies.

This is usually configurable. For example, in `iTerm2`, a macOS terminal, from `Preferences > Profiles > Keys`, you have the option to configure how the left and right <kbd>Option</kbd> keys would behave, among

- Normal
- <kbd>Meta</kbd>
- <kbd>Esc</kbd> +

### What is the difference between delete and kill?

If you *delete* something, it's gone. If you *kill* something, it's still possible to get it back -- from the kill-ring, using `yank` and `yank-pop`.

### What is yank?

To `kill` is to cut. To `yank` is to paste. The difference is that `kill` and `yank` are more advanced than the usual cut and paste. With `yank` and `yank-pop` you have access to an entire ring of recently killed text.
