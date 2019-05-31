# Basic Tools for Web Development

> Download, install, update, and manage basic software tools on Windows.

- [Webpage](https://denisecase.github.io/basic-tools-for-webdev/)
- [Source](https://github.com/denisecase/basic-tools-for-webdev)

## Recommended Prerequisites

- [Windows Setup for Developers](https://github.com/denisecase/windows-setup)
- [Windows File Management](https://github.com/denisecase/windows-file-management)

## Common Tools for Web Development

> Check your machine. If any of these tools are not installed, choose from one of the two installation options listed below.

Web browsers

- Mozilla Firefox
- Google Chrome

Editors

- Notepad++
- Visual Studio Code (VS Code)

Version Control

- Git for Windows (comes with Git Bash)
- TortoiseGit (integrates with Windows File Manager)

JavaScript without a Browser

- Node.js (includes npm, the Node package manager)

All recommended tools are free.

## Chocolatey Installation

Use powerful automation tools to make installing software easier. Install Chocolatey, the Windows Package Manager from <https://chocolatey.org/>.

Right-click in your Documents folder, and select 'Open PowerShell as Administrator'. 
If you don't have this option, see [Windows Setup for Developers](https://github.com/denisecase/windows-setup).

Using the -y flag is optional and will automatically answer 'yes' to install questions.

The following are suggested commands for installing new software - it's even safe to install software you already have (e.g., typically Chrome is already installed). You can find additional information by going to the specific link from <https://chocolatey.org/packages>.

```Powershell
choco install googlechrome -y
choco install firefox -y
choco install notepadplusplus -y
choco install vscode -y
choco install git -y
choco install tortoisegit -y
choco install nodejs -y
```

### Browse Available Packages

Explore at <https://chocolatey.org/packages>.

### Verify Installation

The default location is 'C:\ProgramData\chocolatey' (or for earlier installations, 'c:\chocolatey').

### Upgrade All

To upgrade your versions, periodically run choco upgrade.

```Powershell
choco upgrade chocolatey -y
choco upgrade all
```

## Installing Without Chocolatey

Alternatively, each tool can be installed in the traditional manner. Just go to the website for the software and follow instructions to download, install, and configure tools using provided installers.

## Issues with VS Code and TortoiseGit

Important!

- Make sure VS Code installs right-click 'Open with Code' on folder context menus. If not, reinstall using traditional methods.
- Make sure full TortoiseGit context menus are available. If not, reinstall using traditional methods. 

## Terms

- Chocolatey
- editor
- package manager
- upgrade (get the latest version)
- Windows (operating system)

## Next Steps

Configure Git distributed version control system

- See [Git Started With Windows](https://github.com/denisecase/git-started-windows)
