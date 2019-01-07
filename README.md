# Set up Windows with Chocolatey

> Use Chocolatey, the Windows package manager to download, install, update, and manage software on Windows.

- [Webpage](https://denisecase.github.io/get-setup-with-chocolatey/)
- [Source](https://github.com/denisecase/get-setup-with-chocolatey)

## Recommended Prerequisites

- [Windows Setup for Developers](https://github.com/denisecase/windows-setup)
- [Windows File Management](https://github.com/denisecase/windows-file-management)

## Install Chocolatey

Install Chocolatey, Windows Package Manager from <https://chocolatey.org/>.

## Browse Available Packages

Explore at <https://chocolatey.org/packages>.

## Common Tools for Web Development

Web browsers

- Google Chrome
- Mozilla Firefox

Editors

- Notepad++
- Visual Studio Code (VS Code)

Version Control

- Git for Windows (comes with Git Bash)
- TortoiseGit

JavaScript without a Browser

- Node.js (includes npm, the Node package manager)

All recommended tools are free.

## Install With Chocolatey

Open a command window (or PowerShell) as administrator in your documents folder.

Using the -y flag is optional and will automatically answer 'yes' to install questions.

The following are suggested commands for installing new software - there is no need to install software you already have (e.g., typically Chrome is already installed). You can find additional information by going to the specific link from <https://chocolatey.org/packages>.

```Powershell
choco install googlechrome -y
choco install firefox -y
choco install notepadplusplus -y
choco install vscode -y
choco install git -y
choco install tortoisegit -y
choco install nodejs -y
```

## Verify Installation

Programs may be installed in different locations on your machine. 
The default location is generally something like 'C:\ProgramData\chocolatey' or for earlier installations, 'c:\chocolatey'.

## Upgrade All

To upgrade your versions, periodically run choco upgrade.

```Powershell
choco upgrade all
```

## Installing Without Chocolatey

Alternatively, each tool can be installed in the traditional manner. Just go to the website for the software and follow instructions to download, install, and configure tools using provided installers.

## Terms

- Chocolatey
- editor
- package manager
- upgrade (get the latest version)
- Windows (operating system)

## Next Steps

Configure Git distributed version control system

- See [Git Started With Windows](https://github.com/denisecase/git-started-windows)
