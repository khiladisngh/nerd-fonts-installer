<h1 style="text-align: center;">Nerd Fonts Installer</h1>

<div style="display:flex;justify-content:center">

 <img src="https://img.shields.io/github/license/Ileriayo/markdown-badges?style=for-the-badge" alt="Licence" /> 
 <img src="https://img.shields.io/badge/Debian-D70A53?style=for-the-badge&logo=debian&logoColor=white" alt="Debian" /> 
 <img src="https://img.shields.io/badge/bash_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white" alt="Bash Script" />
 <img src="https://img.shields.io/badge/PowerShell-%235391FE.svg?style=for-the-badge&logo=powershell&logoColor=white" alt="PowerShell" />
 <img src="https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Windows" />

</div>

---

The Nerd Fonts installer provides cross-platform scripts to easily install Nerd Fonts from the command line. It includes a bash script for Linux and macOS systems, and a PowerShell script for Windows systems.

## Features

### ✨ Cross-Platform Support
- **Linux/macOS**: Bash script (`install.sh`) with system-wide font installation
- **Windows**: PowerShell script (`install.ps1`) with user-level font installation

### 🎯 Easy to Use
- Interactive menu with all 51+ Nerd Fonts
- Colored output for better user experience
- Input validation and error handling
- Automatic cleanup of temporary files

### 🔧 Platform-Specific Installation
- **Linux/macOS**: Installs to `~/.fonts/` and refreshes font cache
- **Windows**: Installs to `%LOCALAPPDATA%\Microsoft\Windows\Fonts` and registers with system

### 📦 Font Support
- Supports both `.ttf` and `.otf` font files
- Downloads latest versions from GitHub releases
- Handles font extraction and installation automatically

## Demo
![DEMO](/media/install-nerd-font.gif "install nerd font")

## Install Nerd fonts

### Linux and macOS (Bash)
Download or install the Nerd Fonts with the Nerd Fonts Installer script. To install Nerd Fonts, run the following script.

```bash
bash -c  "$(curl -fsSL https://raw.githubusercontent.com/officialrajdeepsingh/nerd-fonts-installer/main/install.sh)"
```

### Windows (PowerShell)
For Windows users, use the PowerShell version of the installer:

```powershell
# Run in PowerShell (requires PowerShell Core 6+ or Windows PowerShell 5.1+)
iex "& { $(iwr -useb 'https://raw.githubusercontent.com/officialrajdeepsingh/nerd-fonts-installer/main/install.ps1') }"
```

Or download and run locally:
```powershell
# Download the script
Invoke-WebRequest -Uri 'https://raw.githubusercontent.com/officialrajdeepsingh/nerd-fonts-installer/main/install.ps1' -OutFile 'install.ps1'

# Run the script
.\install.ps1
```

After selecting your nerd font, it starts downloading into the system. The PowerShell version installs fonts to the user's local fonts directory and attempts to register them with Windows.
