# WHAT I LEARNED
I have gone throught a computer science degree in CEGEP so I didn't learn much here,

If anything, it was a refresher
and helped me install and configure git on my linux distro

please include these instead of linking github docs because you know students will ChatGPT it instead of clicking and reading the links you provided

Install git: 
[Windows](https://git-scm.com/install/windows), 
[Mac](https://git-scm.com/install/macos) or 
[Linux](https://git-scm.com/install/linux)

## MacOS
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew install git
```

## Windows
[install it from here](https://git-scm.com/install/windows)

if you want to so this entirely with commands, copy this into PowerShell and run it
```bash
$progressPreference = 'silentlyContinue'
Write-Host "Installing WinGet PowerShell module from PSGallery..."
Install-PackageProvider -Name NuGet -Force | Out-Null
Install-Module -Name Microsoft.WinGet.Client -Force -Repository PSGallery | Out-Null
Write-Host "Using Repair-WinGetPackageManager cmdlet to bootstrap WinGet..."
Repair-WinGetPackageManager -AllUsers
Write-Host "Done."
```

then 
```bash
 winget install --id Git.Git -e --source winget 
```

## Set up

Then set up git to start using it to push, pull, fetch, etc...
ere's how to set up git on your laptop: 
[First time git setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)

```git
git config --global user.name "test"
git config --global user.email "test@stuff.ca"
```

this is more about helping students set up their coding environments up with git then hand holding them (which you're not doing either)