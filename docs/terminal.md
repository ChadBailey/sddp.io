# Terminal Commands

| Command                  | Description                                                                                                                                               |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| #![executable]           | She-bang, used for shell scripting. This is what tells the Linux shell the shell to be used when executing this file.                                     |
| !!                       | Copy of last command e.g. `sudo !!`                                                                                                                       |
| [command1] \| [command2] | Pipe, feed output (STDOUT) of [command1] into input of [command2] (STDIN). Used a lot for filtering/searching                                             |
| ls                       | List files and directories (same as dir in Windows)                                                                                                       |
| cd [directory]           | Change directory to [directory]. If none supplied, will return to home directory (`/home/deck`)                                                           |
| rm [filename]            | Remove (delete) [filename] (Warning: cannot be undone)                                                                                                    |
| rm -r [directory]        | Remove (delete) entire directory, and all files/directories inside (Warning: cannot be undone)                                                            |
| chmod +x [filename]      | Give file permission to be executed (shell scripts must be executable to run)                                                                             |
| ./[filename]             | Run/execute [filename]                                                                                                                                    |
| touch [filename]         | Create a new empty file [filename], or update the last modified time of [filename]                                                                        |
| sudo [command]           | Run [command] as admin                                                                                                                                    |
| pacman -Syu              | Perform upgrade of all installed software (Not recommended on Steam Deck!)                                                                                |
| pacman -S [package]      | Install [package] from pacman. i.e. `pacman -S neofetch`. Note that packages installed by pacman get reset each update. flatpak (discovery) is preferred. |
| whoami                   | Your username (useful for writing scripts)                                                                                                                |
| who                      | Get info on all sessions logged in                                                                                                                        |
| dmesg                    | Kernel boot messages. Useful for diagnosing                                                                                                               |
| [command] \| less        | Make text scrollable with arrow keys (alternatives: `more`, `most`). i.e. dmesg \| less                                                                   |
| top                      | Terminal task manager                                                                                                                                     |
| htop                     | More advanced terminal task manager                                                                                                                       |
| vim                      | Vi Improved - famously difficult to use text editor (newbies best to avoid)                                                                               |
| nano                     | Terminal text editor, much easier to use than vi                                                                                                          |
| man [command]            | Manual page (help) for [command]                                                                                                                          |
| [command] -h or --help   | Help for [command] (second version)                                                                                                                       |
| ip addr                  | Get IP address                                                                                                                                            |
| grep [pattern]           | Filter output to only contain what matches [pattern]                                                                                                      |
| Ctrl+c                   | Keyboard Interrupt (close running task, not guaranteed)                                                                                                   |
| Ctrl+d                   | Exit shell, logging out                                                                                                                                   |
| Ctrl+u                   | Clear input                                                                                                                                               |
| Ctrl+z                   | Suspend actively running task and send to background                                                                                                      |
| kill %1                  | kill job #1                                                                                                                                               |
| fg %1                    | Bring job #1 to the foreground                                                                                                                            |
| bg %2                    | Resume job #2, but keep in the background                                                                                                                 |
| [command] &              | Start [command] in background as job #1                                                                                                                   |
| [command1] && [command2] | run [command1], then [command2] when it's finished                                                                                                        |
