# Basic Tools for Web Development

> Download, install, update, and manage basic software tools on Windows.

- [Webpage](https://denisecase.github.io/basic-tools-for-webdev/)
- [Source](https://github.com/denisecase/basic-tools-for-webdev)

## Recommended Prerequisites

- [Windows Setup for Developers](https://github.com/denisecase/windows-setup)
- [Windows File Management](https://github.com/denisecase/windows-file-management)

## Read about Windows Software Automation

Installing software on Windows can be done by typing simple commands with [Chocolatey](https://chocolatey.org/), a software automation tool for Windows. 

## Read about Common Tools for Web Development

If you don't have these tools installed (or even if you do), we recommend using Chocolately to install them. 
Chocolatey makes it easy to keep your software up-to-date. 

Web browsers

- Google Chrome
- Mozilla Firefox

Editors

- Notepad++
- Visual Studio Code (VS Code) - FIRST TIME DO THIS THE TYPICAL WAY

JavaScript without a Browser

- Node.js (includes npm, the Node package manager)

Web Utilities

- cURL - data transfer utility
- Wget - file retrieval utility (request HTTP, HTTPS, and FTP from scripts
- Postman - Web API Development Environment

Version Control

- Git for Windows (comes with Git Bash, a little bit of Linux on Windows :) ) - FIRST TIME DO THIS THE TYPICAL WAY
- TortoiseGit (integrates with Windows File Manager) -- FIRST TIME DO THIS THE TYPICAL WAY

Utilities

- PuTTY - terminal emulator, includes PuTTYGen for generating SSH public-private key pairs used with Git repos

All recommended tools are free.


## Install Chocolatey

Use powerful automation tools to make installing software easier. Install Chocolatey, the Windows Package Manager from <https://chocolatey.org/> by following the directions on the website.

## Install Software with Chocolatey

Right-click in your Documents folder, and select 'Open PowerShell as Administrator'. 
If you don't have this option, see [Windows Setup for Developers](https://github.com/denisecase/windows-setup).

Using the -y flag is optional and will automatically answer 'yes' to install questions.

It's safe to install software you already have (e.g., typically Chrome is already installed). You can find additional information by going to the specific link from <https://chocolatey.org/packages>.

All at once:

```PowerShell
choco install googlechrome notepadplusplus (add all packages as desired) -y
```

Refresh environment variables if they have been modified.

```PowerShell
refreshenv
```

Or one at a time:

```PowerShell
choco install googlechrome -y
choco install notepadplusplus -y
choco install vscode -y
choco install nodejs -y
choco install curl -y
choco install wget -y
choco install git -y
choco install tortoisegit -y
choco install putty -y
choco install postman -y
```

### Optional: Browse Chocolatey Software Packages

Explore at <https://chocolatey.org/packages>.

### Optional: Verify Installation

1. View list of locally-installed programs. Open PowerShell here as Admin and run:

```PowerShell
choco list -local
```

1. Inspect the downloaded software - the default location is 'C:\ProgramData\chocolatey' (or for earlier installations, 'c:\chocolatey').

1. Inspect your updated Windows environment variables. Hit Win key and type env. Select "Edit System Environment Variables". From System Properties window Advanced tab, click "Environment Variables".

### Periodically: Upgrade All

To upgrade your versions, periodically run choco upgrade. You can [automate this script](https://github.com/denisecase/windows-daily-software-upgrade) to make it even easier. 

```Powershell
choco upgrade chocolatey -y
choco upgrade all -y
refreshenv
```

## Installing Without Chocolatey

Alternatively, each tool can be installed in the traditional manner. Just go to the website for the software and follow instructions to download, install, and configure tools using provided installers.

## Installation Issues with VS Code and TortoiseGit

Important!

- Ensure VS Code installs right-click 'Open with Code' on folder context menus. If not, reinstall using traditional methods.
- Ensure full TortoiseGit context menus are available. If not, reinstall using traditional methods. 

## Optional

Firefox Add-ons

- Firefox Multi-Account Containers (limit access across apps)
- uBlockOrigin (blocker) ensure name includes "Origin"
- HTTPS Everywhere (requires encryption)

Ruby + Dev kit (for Jekyll, etc.)

```Powershell
choco install ruby -y
refreshenv
choco install ruby2.devkit -y
refreshenv
```

Ananconda3 (for Python)

```Powershell
choco install anaconda3 -y
```

Professional Java Development

```PowerShell
choco install openjdk -y
choco install eclipse -y
choco install gradle -y
choco install maven -y
```

## Terms

- automation tools
- web browser
- Chocolatey
- editor
- environment variables
- package manager
- upgrade (get the latest version)
- Windows (operating system)

## Next Steps

Configure Git distributed version control system and automate software upgrades

- See [Git Started With Windows](https://github.com/denisecase/git-started-windows)
- [Automate daily choco upgrades](https://github.com/denisecase/windows-daily-software-upgrade)

## See Also

- [Setting Up for Professional Software Development](https://github.com/denisecase/pro-dev-list)
