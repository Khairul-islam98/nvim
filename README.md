# 📖 Vim Essentials Cheatsheet

Welcome to the ultimate Vim Cheatsheet! This guide provides the essential Vim commands you need to navigate, edit, and master the Vim text editor. 💡

---

## Table of Contents
- [Changing Vim Modes](#changing-vim-modes)
- [Exiting](#exiting)
- [Moving Around](#moving-around)
- [Editing Text](#editing-text)
- [Undo & Redo](#undo--redo)
- [Search & Replace](#search--replace)
- [Indentation](#indentation)

---

## 📝 Changing Vim Modes

| Command   | Description                                              |
|-----------|----------------------------------------------------------|
| `i`       | Enter **INSERT** mode                                    |
| `a`       | Enter **INSERT** mode after the cursor (append)          |
| `A`       | Enter **INSERT** mode at the end of the line             |
| `o`       | Open new line below cursor and enter **INSERT** mode     |
| `O`       | Open new line above cursor and enter **INSERT** mode     |
| `v`       | Enter **VISUAL** mode                                    |
| `Ctrl-v`  | Enter **VISUAL-BLOCK** mode                              |
| `:`       | Enter **COMMAND-LINE** mode                              |
| `R`       | Enter **REPLACE** mode                                   |
| `ESC`     | Go back to **NORMAL** mode                               |

---

## 🚪 Exiting

| Command       | Description                                      |
|---------------|--------------------------------------------------|
| `:w`          | Write (save) file without exiting                |
| `:wa`         | Write (save) all open files without exiting      |
| `:q`          | Quit but fail if unsaved changes exist           |
| `:q!`         | Quit and discard unsaved changes                 |
| `:wq` or `:x` | Write (save) and quit                            |
| `:wqa`        | Write and quit all open files                    |

---

## 🚀 Moving Around Within Vim

### Basic Arrow Movements
| Command | Description                   |
|---------|-------------------------------|
| `h`     | Move cursor left              |
| `j`     | Move cursor down              |
| `k`     | Move cursor up                |
| `l`     | Move cursor right             |

### Movements Within a Line
| Command | Description                                |
|---------|--------------------------------------------|
| `$`     | Move cursor to the end of the line         |
| `0`     | Move cursor to the beginning of the line   |
| `^`     | Move cursor to first non-blank character   |

> **Tip:** Use **`;`** and **`,`** to repeat `f`, `F`, `t`, or `T` movements forward or backward.

---

## ✂️ Editing Text

### Deleting
| Command      | Description                                                        |
|--------------|--------------------------------------------------------------------|
| `d{motion}`  | Delete text moved over by `{motion}` and copy into register        |
| `dd`         | Delete whole current line and copy into register                   |
| `D`          | Delete from cursor to end of line                                  |

> **Examples:**
> - `dw`: Delete to the start of next word.
> - `de`: Delete to the end of the current word.
> - `dG`: Delete to the end of file.

### Changing Text
| Command       | Description                                                        |
|---------------|--------------------------------------------------------------------|
| `c{motion}`   | Delete text moved over by `{motion}`, copy into register, and enter insert mode |
| `cc`          | Delete whole line, copy into register, and enter insert mode       |
| `C`           | Delete from cursor to end of line, copy into register, and enter insert mode |

---

## 🔄 Undo & Redo

| Command    | Description                    |
|------------|--------------------------------|
| `u`        | Undo last change               |
| `Ctrl-R`   | Redo changes undone with `u`   |

---

## 🔍 Search & Replace

| Command              | Description                                                   |
|----------------------|---------------------------------------------------------------|
| `:s/old/new/g`       | Replace all occurrences of `old` with `new` in the file       |
| `:s/old/new/gc`      | Replace all occurrences with confirmation                     |
| `:s/old/new/gi`      | Replace all occurrences, ignoring case                        |
| `/pattern`           | Search forward for `pattern`                                  |
| `?pattern`           | Search backward for `pattern`                                 |

> **Tip:** Use `:nohl` to temporarily turn off search highlights.

---

## ⬆️ Indentation

| Command        | Description                                 |
|----------------|---------------------------------------------|
| `>{motion}`    | Indent text moved over by `{motion}` to the right  |
| `>>`           | Indent whole current line to the right      |

> **Example:** `2>>` indents the current line and the line below it.

---

## 📚 Additional Resources

For more detailed Vim commands and advanced configurations, refer to [Vim Documentation](https://www.vim.org/docs.php).

---

Happy Vimming! ✨

