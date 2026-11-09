---
tags: [command, linux]
---
# Linux Commands

> ✅ = learned in [[DevOps Pre-Requisite Course]] · others = coming later

## Shell
| Command | What it does |
|---|---|
| ✅ `echo $SHELL` | Show which shell I'm using (e.g. `/bin/bash`) |
| ✅ `echo Hi` | Print text to the screen |
| ✅ `cmd1; cmd2; cmd3` | Run multiple commands one after the other |

## Directories
| Command | What it does |
|---|---|
| ✅ `pwd` | Print Working Directory — where am I? |
| ✅ `ls` | List files and folders |
| ✅ `cd my_dir1` | Change directory (go into a folder) |
| ✅ `mkdir new_directory` | Make a directory |
| ✅ `mkdir -p /tmp/asia/india/bangalore` | Make a whole directory hierarchy at once (parents too) |
| ✅ `rm -r /tmp/my_dir1` | Remove a directory and everything inside (careful — no recycle bin!) |
| ✅ `cp -r my_dir1 /tmp/my_dir1` | Copy a directory with its contents |
| `ls -la` | Detailed list, including hidden files |
| `cd ..` | Go up one folder |
| `cd ~` | Go to my home folder |

## Files
| Command | What it does |
|---|---|
| ✅ `touch new_file.txt` | Create a new, empty file |
| ✅ `cat > new_file.txt` | Write text into a file → type the text, then press **Ctrl + D** to save and exit |
| ✅ `cat new_file.txt` | View the contents of a file |
| ✅ `cp new_file.txt copy_file.txt` | Copy a file |
| ✅ `mv new_file.txt sample_file.txt` | Move or rename a file |
| ✅ `rm new_file.txt` | Remove (delete) a file |
| `cat >> new_file.txt` | **Add** text to the end of a file (`>` overwrites, `>>` appends) |

## Permissions *(later)*
| Command | What it does |
|---|---|
| `chmod 755 file` | Change permissions |
| `chown user:group file` | Change owner |
| `sudo command` | Run as admin (root) |

## Processes and services *(later)*
| Command | What it does |
|---|---|
| `ps aux` | List running processes |
| `systemctl status nginx` | Service status |
| `journalctl -u nginx` | Service logs |

## 💡 Patterns
- `-r` = **recursive** → "the folder AND everything inside it" (used with `rm`, `cp`)
- `-p` = **parents** → "create the missing parent folders too" (used with `mkdir`)
- Paths starting with `/` are **absolute** (from the root: `/tmp/asia`); without `/` they are **relative** (from where I am: `my_dir1`)

Topic: [[Linux]]
