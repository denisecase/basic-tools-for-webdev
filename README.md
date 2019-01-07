# Set up Windows with Chocolatey

> Use Chocolatey, the Windows package manager to download, install, update, and manage Windows software tools.

- [Webpage](https://denisecase.github.io/get-setup-with-chocolatey/)
- [Source](https://github.com/denisecase/get-setup-with-chocolatey)

## Recommended Prerequisites

- [Windows Setup for Developers](https://github.com/denisecase/windows-setup)
- [Windows File Management](https://github.com/denisecase/windows-file-management)

## Install Chocolatey

Install Chocolatey, Windows Package Manager from <https://chocolatey.org/>.

## Indentify Desired Tools

Web browsers

- Google Chrome
- Mozilla Firefox

Editors

- Notepad++
- Visual Studio Code (VS Code)

Integrated Development Environment

- Visual Studio Community Edition

Version Control

- Git for Windows (comes with Git Bash)
- TortoiseGit

All recommended tools are free.

## Install With Chocolatey

Open a command window (or PowerShell) as administrator in your documents folder.

Using the -y flag is optional and will automatically answer 'yes' to install questions.

Run the following commands for any software you don't have installed already. Chrome - and maybe more - are likely already installed.  Do not run those commands.

```Powershell
choco install chrome -y
choco install firefox -y
choco install notepadplusplus -y
choco install vscode -y
choco install git -y
choco install tortoisegit -y
```

## Verify Installation

Programs may be installed in different locations on your machine. 
The default location is generally something like 'C:\ProgramData\chocolatey' or for earlier installations, 'c:\chocolatey'.

## Upgrade All

To upgrade your versions, periodically run choco upgrade.

```Powershell
choco upgrade all
```

## Terms

- editor
- integrated development environment
- package manager
- upgrade (get the latest version)
- Windows (operating system)

## Next Steps

Configure Git distributed version control system

- See [Git Started With Windows](https://github.com/denisecase/git-started-windows)
