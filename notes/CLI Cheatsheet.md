# System (Shell): Commands

## Shell Identification

| **Token (Input)** | **Classification (Type)** | **Function (Behaviour)** |
| --- | --- | --- |
| `echo` `$SHELL` | Environment variable check | Outputs default login shell (e.g. `/bin/zsh`) |
| `echo` `$0` | Shell process check | Shows currently running shell (e.g. `zsh`) |
| `ps` `-p $$` | Process inspection | Displays current shell process; check `CMD` column |

## Prompt Symbols

| **Token** | **Classification (Type)** | **Function (Behaviour)** |
| --- | --- | --- |
| `%` | Shell prompt | zsh default user prompt |
| `$` | Shell prompt | standard user prompt |
| `#` | Shell prompt | root user prompt |

## Keyboard Shortcuts

| **Token (Input)** | **Classification (Type)** | **Function (Behaviour)** |
| --- | --- | --- |
| `⌃`  `C` (ctrl) | Signal (SIGINT) | Interrupt current foreground process |
| `⌃`  `C` (ctrl) | EOF signal | Exit shell if line is empty |
| `⌃`  `Z` | Signal (SIGTSTP) | Suspend current process (resume with `fg`) |
| `⌃`  `A` | Readline shortcut | Move cursor to start of line |
| `⌃`  `E` | Readline shortcut | Move cursor to end of line |
| `⌃`  `U` | Readline shortcut | Delete from cursor to start of line |
| `⌃`  `K` | Readline shortcut | Delete from cursor to end of line |
| `⌃`  `W` | Readline shortcut | Delete previous word |
| `↑` | Readline/history | Cycle backward through command history |
| `⌃`  `R` | Readline/history | Reverse search command history |
| `⌃`  `L` | Readline shortcut | Clear (terminal) screen (same effect as `clear`) |

## Shell Builtins

| **Token (Input)** | **Classification (Type)** | **Function (Behaviour)** |
| --- | --- | --- |
| `cd` | Shell builtin | Change current directory |
| `cd ..` | Shell builtin | Move to parent directory |
| `cd ~` | Shell builtin + tilde expansion | Go to home directory |
| `pwd` | Shell builtin/external | Print working directory |
| `echo` | Shell builtin | Print arguments to **stdout** |
| `history` | Shell builtin | List command history |
| `exit` | Shell builtin | Exit shell |
| `export` | Shell builtin | Set environment variables |
| `unset` | Shell builtin | Remove environment variables |
| `alias` | Shell builtin | Create command shortcuts |
| `unalias` | Shell builtin | Remove aliases |
| `source` | Shell builtin | Reload shell config (e.g. `.zshrc`) |

## External Commands

| **Token (input)** | **Classification (type)** | **Function (behaviour)** |
| --- | --- | --- |
| `ls` | External command | List directory contents |
| `ls -la` | External command + options | List detailed contents including hidden files |
| `cat`  | External command | Output file contents |
| `less` | External command | View file interactively (paged) |
| `touch` | External command | Create empty file or update timestamp |
| `mkdir` | External command | Create directory |
| `rmdir` | External command | Remove empty directory |
| `cp` | External command | Copy files/directories |
| `mv`  | External command | Move or rename files |
| `rm` | External command | Remove files |
| `rm -r` | External command + option | Remove directories recursively |
| `grep` | External command | Search text patterns in files |
| `find` | External command | Locate files/directories |
| `head` | External command | Show first lines of file |
| `tail` | External command | Show last lines of file |
| `chmod` | External command | Change file permissions |
| `chown` | External command | Change file ownership |
| `whoami` | External command | Print current user |
| `curl` | External command | Transfer data via URLs |
| `ping` | External command | Test network reachability |
| `ssh` | External command | Connect to remote system |
| `man` | External command | Display manual pages |
| `clear` | External command | Clear terminal (alt to ⌃L) |
| `open` (macOS)
`xdg-open` (Linux) | External command | Open fileURL/directory/app
open filename.txt
open https://example.com
open .
open -1 “AppName” file.txt |
| `which` | External command | Show command path |
| `where` 
(or `which` `-a`) | External command | Show all matches |
| `env` | External command | List environment variables |
| `top` | External command | System processes viewer |
| `kill` | External command | Terminate process |
| `df` | External command | Disk usage (filesystem) |
| `du` | External command | Directory/file size |
| `tar` | External command | Archive/extract files |
| `zip/unzip` | External command | Compress/extract |

## Root/Sudo

| **Token (Input)** | **Classification (Type)** | **Function (Behaviour)** |
| --- | --- | --- |
| `sudo` | Privileged command | Run command with elevated privileges (as superuser) |

## **Special Paths/Navigation**

| **Token (Input)** | **Classification (Type)** | **Function (Behaviour)** |
| --- | --- | --- |
| `..` | Special directory | Parent directory |
| `.` | Special directory | Current directory |
| `cd -` | Shell builtin + argument | Switch to previous directory |
| `cd \~` | Command usage + expansion | Go to home directory |
| `cd ..` | Command usage | Move to parent directory |
| `cd ./folder` | Command usage | Access folder relative to current directory |

## **Shell Expansions**

| **Token (Input)** | **Classification (Type)** | **Function (Behaviour)** |
| --- | --- | --- |
| `~` | Tilde expansion | Expands to home directory |
| `$HOME` | Variable expansion | Path to home directory |
| `$PATH` | Variable expansion | Directories shell searches for commands |
| `$(pwd)` | Command substitution | Runs command and inserts output |
| `$((1+2))` | Arithmetic expansion | Evaluates expression |
| `*` | Globbing | Match multiple files |
| `?` | Globbing | Match single character |

## Standard Streams

| **Token (Input)** | **Classification (Type)** | **Function (Behaviour)** |
| --- | --- | --- |
| stdin | Input stream | Data/input into program |
| stdout | Output stream | Normal output |
| stderr | Error stream | Error output/message |

## Shell Features/Operators

| **Token (Input)** | **Classification (Type)** | **Function (Behaviour)** |
| --- | --- | --- |
| `⇥` (tab) | Completion feature | Autocomplete based on context |
| `⇥` `⇥` | Completion feature | List possible completions |
| `|` | Pipe operator | Pass **stdout** to next command |
| `>` | Redirection operator | Redirect **stdout** to file (overwrite) |
| `>>` | Redirection operator | Append **stdout** to file |

## Control Operators

| **Token (Input)** | **Classification (Type)** | **Function (Behaviour)** |
| --- | --- | --- |
| `&&` | Control operator | Run next if previous succeeds |
| `||` | Control operator | Run next if previous fails |
| `;` | Control operator | Run sequentially |
| `&` | Control operator | Run in background |

## Command Examples

| **Token (Input)** | **Classification (Type)** | **Function (Behaviour)** |
| --- | --- | --- |
| `mkdir` `notes`  | Command usage | Create directory named notes |
| `touch` `notes/day1.md` | Command usage | Create file inside directory |
| `ls` `notes/` | Command usage | List contents of notes directory |
| `man` `ls` | Command usage | Open manual for `ls` (macOS) |
| `ls` `-h` | Command option | Human-readable file sizes (if supported) |
| `--help` | Command flag | Show command help (common on Linux) |
| `cd` `~/projects/learning-journal` | Command + expansion | Change to specific path |

# Git: Commands

## Daily Workflow

```bash
git add .
git commit -m "message"
git push
```

## **Core Commands**

| Token (Input) | Classification (Type) | Function (Behaviour) |
| --- | --- | --- |
| `git init` | Git command | Initialize new repository |
| `git clone` | Git command | Copy remote repository locally |
| `git status` | Git command | Show repo state (staged/unstaged)
  • Check changes
  • Good to use if multiple files changed |
| `git add .` | Git command | Stage all changes for commit
• "Hey Git, look at everything I changed" |
| `git add` | Git command | Stage specific file |
| `git commit` | Git command | **Create commit (opens editor)**
  • Saves a snapshot of your files) locally (on your computer)
      ◦ Think of it like saving a version of a document, except it remembers every version forever. If you mess something up in Week 6, you can go back to the exact state of your files from Week 1.
  • Uses staged changes only
  • Does not push to remote (GitHub)
  • Requires manual save/close to finish commit
**Interactive**
    ◦ Opens editor (VS Code) to write commit message there
    ◦ Supports multi-line message and detailed description/body |
| `git commit -m “message”` | Git command | **Create commit with message**
  • Saves a snapshot of your files locally (on your computer)
  • Uses staged changes only
  • Does not push to remote (GitHub)
  • Requires manual save/close to finish commit
**Non-interactive
  •** Skips editor and uses inline message
  • Faster for simple commits (typically single-line message) |
| `git log` | Git command | Show commit history/previous messages
Press `q` to exit the view |
| `git log --oneline` | Git command | Condensed history view
Press `q` to exit the view |

## **Branching**

| Token (Input) | Classification (Type) | Function (Behaviour) |
| --- | --- | --- |
| `git branch` | Git command | List branches |
| `git branch` | Git command | Create new branch |
| `git checkout` | Git command | Switch to branch |
| `git checkout -b` | Git command | Create and switch branch |
| `git switch` | Git command | Switch branch (modern) |
| `git switch -c` | Git command | Create and switch branch |
| `git merge` | Git command | Merge branch into current |

## **Remote Commands**

| Token (Input) | Classification (Type) | Function (Behaviour) |
| --- | --- | --- |
| `git remote -v` | Git command | Show remote repositories |
| `git remote add origin` | Git command | Add remote repository |
| `git push` | Git command | Upload commits to remote (i.e., GitHub)
  • *"Upload this snapshot to GitHub so it's backed up online and visible to the world”* |
| `git push -u origin main` | Git command | Push and set upstream |
| `git pull` | Git command | Fetch and merge latest commits from remote (GitHub) |
| `git fetch` | Git command | Download changes without merging |

## **Undo/Inspect Commands**

| Token (Input) | Classification (Type) | Function (Behaviour) |
| --- | --- | --- |
| `git diff` | Git command | Show unstaged changes |
| `git diff –staged` | Git command | Show staged changes |
| `git restore` | Git command | Discard file changes |
| `git restore –staged` | Git command | Unstage file |
| `git reset` | Git command | Unstage changes |
| `git reset –hard` | Git command | Reset working directory (destructive) |
| `git revert` | Git command | Undo commit safely |

## Stashing Commands

| Token (Input) | Classification (Type) | Function (Behaviour) |
| --- | --- | --- |
| `git stash` | Git command | Save changes temporarily |
| `git stash pop` | Git command | Restore stashed changes |
| `git stash list` | Git command | List stashes |

# Git: Other

## Conventional Commits

feat: new feature
fix: bug fix
docs: documentation/notes
chore: maintenance, config
refactor: restructuring code
test: adding or fixing tests
style: formatting only

### Examples
feat: add user login endpoint
fix: resolve null pointer in auth
docs: add 2026-05-04 shell tools notes
chore: update .gitignore

## Files & Behaviour

**[ Not commands ]**

- `.gitignore`
    - Text file inside your project
    - **Defines files Git should ignore** — *don’t track these files*
        - *You'll learn about `.gitignore` files later when you start building real projects (it keeps things like passwords and temp files out of your repo)*
        - [About ignoring files](https://docs.github.com/get-started/git-basics/ignoring-files)
    - **Read by Git automatically and prevents tracking of:**
        - Secrets (API keys, env files)
        - Temp/system files (logs, cache files)
    - Example:
        - `.gitignore` contains:
            - passwords.txt
        - **Result:**
            - Git will ignore that file
            - It won’t show up in:
                - `git status`
                - commits
    - **Important Rule:**
        - It only works **before** tracking/commits:
            - If file is **not yet added** → `.gitignore` works
            - If file was already committed → `.gitignore` does nothing
        - Does not remove already tracked files
