# 42-minishell

![C](https://img.shields.io/badge/Language-C-blue)
![42](https://img.shields.io/badge/School-42_SP-black)
![Status](https://img.shields.io/badge/Status-Finished-brightgreen)

## 📌 About
Minishell is a 42 project that consists of building a simple shell inspired by Bash.
The goal is to understand how a shell works internally — from parsing user input to
executing commands and managing processes.

This project was developed in collaboration with [Pedro Barbosa](https://github.com/PedroHJB).

## ✅ Features
- Display a prompt and wait for user input
- Working command history
- Execute commands using `PATH` or absolute/relative paths
- Handle single `'` and double `"` quotes
- Redirections:
  - `<` — input redirection
  - `>` — output redirection
  - `>>` — append output redirection
  - `<<` — heredoc
- Pipes `|` — output of one command as input of the next
- Environment variables (`$VAR`) and `$?` (exit status of last command)
- `ctrl-C`, `ctrl-D` and `ctrl-\` signals behave like in Bash

## 🔧 Built-in Commands

| Command | Description |
|---|---|
| `echo` | Prints text to stdout (supports `-n` flag) |
| `cd` | Changes current directory |
| `pwd` | Prints current working directory |
| `export` | Sets environment variables |
| `unset` | Removes environment variables |
| `env` | Prints all environment variables |
| `exit` | Exits the shell |

## ▶️ Usage
Clone the repository and compile:
```bash
git clone https://github.com/Zephele/42-minishell.git
cd 42-minishell
make
```

Run the shell:
```bash
./minishell
```

## 🛠️ Technologies
- Language: C
- Libraries: readline
- System calls: `fork`, `execve`, `pipe`, `dup2`, `waitpid`, `signal`

## 📚 What I learned
- How a shell parses and executes commands
- Process creation and management with `fork` and `execve`
- Inter-process communication with pipes
- Signal handling in C
- Collaborative development and code organization in a team project

## Authors
- **Rafael Tanaka** — [GitHub](https://github.com/Zephele) · [LinkedIn](https://www.linkedin.com/in/rafael-tanaka-359232285/)
- **Pedro Barbosa** — [GitHub](https://github.com/PedroHJB)
