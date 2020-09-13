---
title: "Config oh-my-posh on Windows 10"
date: 2020-09-08T07:05:30Z
draft: true
---

[oh-my-posh](https://github.com/JanDeDobbeleer/oh-my-posh), as an alternative of oh-my-zsh in *nix-based system, is a beautiful theme engine for Powershell in Windows Terminal.
## Prerequisites
1. [Windows Terminal](https://github.com/microsoft/terminal)
2. [Git](https://git-scm.com/)
3. [Powerline fonts](https://github.com/powerline/fonts) (at least one font is needed to be installed)

## Installation
Using the following commands to install the oh-my-posh in your Windows Terminal:
```powershell
Install-Module posh-git -Scope CurrentUser  
Install-Module oh-my-posh -Scope CurrentUser
```
Now the oh-my-posh is successfully installed on your computer, the following commands are used to enable the prompt:
```powershell
Set-ExecutionPolicy -ExecutionPolicy Bypass 
# This is a must unless you have already modified the Execuation Policy of the Powershell to a proper option 
# See https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-7 for details
Set-prompt
Set-theme Agnoster # Optional, Agnoster is one of the fancy themes
```
Now the installation process is finished and if no error occurs, you will see the new prompt. Please visit [here](https://github.com/JanDeDobbeleer/oh-my-posh) if you want to get some in-depth knowledge of it. 

## Enable at startup
If you want to use oh-my-posh when the Windows Terminal starts, you need to finish the following procedures:
1. Open the Settings of the Windows Terminal by clicking the triangle on the top of the windows.
2. Find the block with **"name": "Windows PowerShell"** and change the value of property **commandline** as **"powershell.exe -NoExit -Command & {Set-Theme Agnoster}"**
3. Add property **fontFace** with value which is the font name you want to use, for me, it is **"fontFace": "Roboto Mono for Powerline"**
4. Restart the Windows Terminal to see what will happen!