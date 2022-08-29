# Terminal commands

!> This page is **under construction**, expect frequent major updates and
corrections until this banner is removed.

## Beginner commands

| Command                   | Description                                                                                                  |
| ------------------------- | ------------------------------------------------------------------------------------------------------------ |
| Ctrl+c                    | Keyboard Interrupt - close/cancel running task                                                               |
| Ctrl+d                    | Exit shell, log out                                                                                          |
| Ctrl+u                    | Clear input                                                                                                  |
| Ctrl+z                    | Suspend actively running task and send to background (use when ctrl+c doesn't work)                          |
| sudo [command]            | Run [command] as admin                                                                                       |
| ls                        | List files and directories (same as dir in Windows)                                                          |
| cd [directory]            | Change directory to [directory]. If none supplied, will return to home directory (`/home/deck`)              |
| rm [filename]             | Remove (delete) [filename] (Warning: cannot be undone)                                                       |
| rm -r [directory]         | Remove (delete) entire directory, and all files/directories inside (Warning: cannot be undone)               |
| ./[filename]              | Run/execute [filename]                                                                                       |
| top                       | Terminal task manager                                                                                        |
| htop                      | More modern/advanced terminal task manager                                                                   |
| kill [Process ID]         | kill [Process ID] with default signal (sigterm, close politely)                                              |
| kill -9 [Process ID]      | kill [Process ID] with signal 9 (most aggressive, killed in scheduler directly in kernel)                    |
| killall [Process Name]    | kill all instances of [Process Name] with default signal (sigterm, close politely)                           |
| killall -9 [Process Name] | kill all instances of [Process Name] with signal 9 (most aggressive, killed in scheduler directly in kernel) |
| nano                      | Terminal text editor, much easier to use than vi                                                             |

## Basic usage

| Command                | Description                                                                                                                                               |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| !!                     | Copy of last command e.g. when you forget to use sudo `sudo !!`                                                                                           |
| chmod +x [filename]    | Give file permission to be executed (files must have permission to be executed)                                                                           |
| man [command]          | Manual page (help) for [command]                                                                                                                          |
| [command] -h or --help | Help for [command] (another way to get help)                                                                                                              |
| ip addr                | Get IP address                                                                                                                                            |
| grep [pattern]         | Filter output to only contain what matches [pattern]                                                                                                      |
| [command] \| less      | Make text scrollable with arrow keys (alternatives: `more`, `most`). i.e. dmesg \| less                                                                   |
| kill %1                | kill job #1                                                                                                                                               |
| pacman -Syu            | Perform upgrade of all installed software (Not recommended on Steam Deck! But it won't necessarily cause harm, just know what you're doing)               |
| pacman -S [package]    | Install [package] from pacman. i.e. `pacman -S neofetch`. Note that packages installed by pacman get reset each update. flatpak (discovery) is preferred. |

## Advanced usage

| Command                  | Description                                                                                                   |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| [command1] \| [command2] | Pipe, feed output (STDOUT) of [command1] into input of [command2] (STDIN). Used a lot for filtering/searching |
| touch [filename]         | Create a new empty file [filename], or update the last modified time of [filename]                            |
| who                      | Get info on all sessions logged in                                                                            |
| dmesg                    | Kernel boot messages. Useful for diagnosing                                                                   |
| vim                      | Vi Improved - famously difficult to use text editor (newbies best to avoid)                                   |
| fg %1                    | Bring job #1 to the foreground                                                                                |
| bg %2                    | Resume job #2, but keep running in background                                                                 |
| [command] &              | Start [command] in background (suspended) as job #1                                                           |
| [command1] && [command2] | run [command1], then [command2] when it's finished                                                            |

## Shell scripting

| Command             | Description                                                                                                           |
| ------------------- | --------------------------------------------------------------------------------------------------------------------- |
| #![executable]      | She-bang, used for shell scripting. This is what tells the Linux shell the shell to be used when executing this file. |
| whoami              | Your username (useful for writing scripts)                                                                            |
| echo                | Prints a blank line to the terminal (sometimes useful for spacing purposes)                                           |
| echo "hello, world" | Prints "hello, world" to the terminal                                                                                 |
| echo $([command])   | Take output of [command] and place as parameter to `echo`.                                                            |
