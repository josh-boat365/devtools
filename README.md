# devtools
This is  a collection of the dev tools I use 

![](./powershel%20prompt.PNG)

> ## Terminal Propmt Design
This is a terminal prompt design on windows 10 and above...

***From Microsoft Store:***
1. install windows terminal 
2. install powershell 7.2.5 ( latest as of now..)
3. install oh-my-posh

***Installing using powershell:***
> ## Manual Installation:
``` 
Set-ExecutionPolicy Bypass -Scope Process -Force; Invoke-Expression ((New-Object System.Net.WebClient).DownloadString('https://ohmyposh.dev/install.ps1'))
```
> ## Installation using winget:
```
winget install JanDeDobbeleer.OhMyPosh -s winget
```
 ## To Use:
1. A powershell folder will be created in your documents dir, copy and paste the contents of the folder  ` config_files_ohmyposh`
2. After installing oh-my-posh, copy the contents in the folder `ohmyposh_themes` and paste it in this path `C:\Users\PC_NAME\AppData\Local\oh-my-posh`
3. run this command to configure/start [Ohmyposh](https://ohmyposh.dev/docs/installation/windows):
```
oh-my-posh prompt init --config C:\Users\PC_NAME\AppData\Local\oh-my-posh\config.omp.json | Invoke-Expression
```
4. goto [Nerdfonts](https://www.nerdfonts.com/font-downloads) then download this font `FantasqueSanaMono Nerd Font` which has glyphs to help your terminal look like this:
![](./powershell_prompt.PNG)
5. after downloading the `Nerd Font` :
```
Press the Windows Button + R on the keyboard
Type:
C:\Windows\Fonts
Hit Enter on the keyboard
Extract the Nerd Fonts, copy the fonts and paste them in the fonts window to install the fonts.
```
6. click on the arrow point down then select setting from the dropdown:

![](./1.PNG)

7. after clicking on setting, navigate to `Appearance` in the `Windows Terminal ` downloaded from `Microsoft store` , then choose `font face` and select `FantasqueSanaMono NF`
8. Run this command to install [Terminal icons](https://github.com/devblackops/Terminal-Icons):
```
Install-Module -Name Terminal-Icons -Repository PSGallery
```
Usage (Terminal icons):
```
Import-Module -Name Terminal-Icons
```
9. Run this command to install [posh git](https://computingforgeeks.com/posh-git-powershell-environment-for-git/):
```
PowerShellGet\Install-Module posh-git -Scope CurrentUser -Force

Install-Module PowershellGet -Force
```
To change an ohmyposh theme:

change/replace the file `config.omp.json` in 
```
oh-my-posh prompt init --config C:\Users\PC_NAME\AppData\Local\oh-my-posh\config.omp.json | Invoke-Expression
```
with your choice of themes in the folder ` C:\Users\PC_NAME\AppData\Local\oh-my-posh\config.omp.json` 