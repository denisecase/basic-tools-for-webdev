# Basic Tools for Web Development

> Download, install, update, and manage basic software tools on Windows.

- [Webpage](https://denisecase.github.io/basic-tools-for-webdev/)
- [Source](https://github.com/denisecase/basic-tools-for-webdev)

## Recommended Prerequisites

- [Windows Setup for Developers](https://github.com/denisecase/windows-setup)
- [Windows File Management](https://github.com/denisecase/windows-file-management)

## Install First

Windows Software automation tool

- [Chocolatey](https://chocolatey.org/) - click "Install" to read and follow the instructions.

Always check the script before running - verify the security and contents of any script before executing it.


## Common Tools for Web Development

If you don't have these tools installed (or even if you do), we recommend using Chocolately to install them. 
Chocolatey makes it easy to keep your software up-to-date. 

Web browsers

- **Mozilla Firefox** (Developer Edition)
- **Google Chrome**

Editors

- **Notepad++**
- **Visual Studio Code (VS Code)**

JavaScript without a Browser

- **Node.js** (includes **npm**, the Node package manager)

Web Utilities

- **cURL** - data transfer utility
- **Wget** - file retrieval utility (request HTTP, HTTPS, and FTP from scripts
- **Postman** - Web API Development Environment

Version Control

- **Git for Windows (comes with Git Bash)**
- **TortoiseGit** (integrates with Windows File Manager)

Utilities

- **Putty** - terminal emulator and PuttyGen for generating SSH public-private key pairs for Git repos

All recommended tools are free.


## Chocolatey Installation

Use powerful automation tools to make installing software easier. Install Chocolatey, the Windows Package Manager from <https://chocolatey.org/>.

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
choco install firefox-dev --pre -y
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

### Browse Chocolatey Software Packages

Explore at <https://chocolatey.org/packages>.

### Verify Installation

1. View list of locally-installed programs. Open PowerShell here as Admin and run:

```PowerShell
choco list -local
```

1. Inspect the downloaded software - the default location is 'C:\ProgramData\chocolatey' (or for earlier installations, 'c:\chocolatey').

1. Inspect your updated Windows environment variables. Hit Win key and type env. Select "Edit System Environment Variables". From System Properties window Advanced tab, click "Environment Variables".

### Upgrade All

To upgrade your versions, periodically run choco upgrade. You can [automate this script](https://github.com/denisecase/windows-daily-software-upgrade) to make it even easier. 

```Powershell
choco upgrade chocolatey -y
choco upgrade all -y
refreshenv
```

## Installing Without Chocolatey

Alternatively, each tool can be installed in the traditional manner. Just go to the website for the software and follow instructions to download, install, and configure tools using provided installers.

## Issues with VS Code and TortoiseGit

Important!

- Ensure VS Code installs right-click 'Open with Code' on folder context menus. If not, reinstall using traditional methods.
- Ensure full TortoiseGit context menus are available. If not, reinstall using traditional methods. 

## Recommended

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

Configure Git distributed version control system

- See [Git Started With Windows](https://github.com/denisecase/git-started-windows)
