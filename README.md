
# 🐚 Custom Shell

## Introduction
Welcome to minishell, a minimalist yet powerful Unix shell written in C. This shell is designed to handle standard shell commands, redirections, pipes, and a variety of built-in commands. It also supports advanced features such as expansions, open quotes, and open pipes, all while aiming to closely mimic the behavior of Bash.

## Features



- Shell Commands: Execute standard shell commands seamlessly.
- Redirections: Handle
    - `>`
    - `<`
    - `>>`
    - `<<`
- Pipes: Utilize pipes `|` for command chaining.
- Built-in Commands: Includes essential commands like:
    - `echo`
    - `cd`
    - `pwd`
    - `export`
    - `unset`
    - `exit`
    - `env`

Expansions: Supports variable expansions with `$`.

Signal Handling: Mimics Bash behavior for `Ctrl+C`, `Ctrl+D`, and `Ctrl+\`.

Open `Quotes` & `Pipes`: Implements advanced features for open quotes and pipes.
## Usage
**To install and set up the shell, follow these steps:**

Clone the Repository:
```bash
git clone https://github.com/ciusca42/Minishell.git
cd Minishell
```
**Build the project** with `make` and run it with `./minishell`
### Suppression
The functions `readline()` & `add_history()` have **memory leaks**

using `make sup` will create a file called `ignore_readline.supp` and will run the program supressing the leaks for those functions

## Examples
Some commands that you can try on minishell
```bash
ls -la | grep ".c" > c_files.txt
```
```bash
export MY_VAR="Hello"
echo $MY_VAR
```
```bash
cat file.txt | grep "pattern"
```


## Contributing

Contributions are always welcome!

Feel free to open an issue if you find something that does not work


