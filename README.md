# cpp-vscode-windows

VSCode settings that I use to write and debug C/C++ code on Windows 10.

## Shell script:

`script.bat` clones the settings into a folder named by the command line argument and removes everything except the settings.

To create a [doskey macro](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/doskey) that does the same, use:

```cmd
doskey pc=git clone https://github.com/Wahaj404/cpp-vscode-windows.git $1 $t rmdir /s /q $1\.git $t del $1\README.md $t %1\script.bat
```

Usage: `pc my-cpp-project`
