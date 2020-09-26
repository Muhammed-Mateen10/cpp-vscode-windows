# cpp-vscode

VSCode settings that I use to write and debug C/C++ code on Windows 10.

## Shell script:

This script clones the settings into a folder named by the command line argument and removes .git and README.md.

Remove `@echo off` to view the output from `git clone`.

Remove the last line to not open the folder in vscode immediately.

```cmd
@echo off

git clone https://github.com/Wahaj404/cpp-vscode.git $1
rmdir /s /q $1/.git
del $1/README.md
code $1
```
