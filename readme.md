# Windows powershell (W11)

Prerequisite:

0.Check in MS store if Windows Terminal is installed:

![screenshot](windows-terminal.png)

1.Install a nerd a font:
<https://github.com/ryanoasis/nerd-fonts>

2.Set a nerd font as default for console:

![screenshot](nerd-font.png)

```console
Main steps:

1) Run in powershell:

    winget install JanDeDobbeleer.OhMyPosh -s winget

2) Run in powershell:

    winget upgrade JanDeDobbeleer.OhMyPosh -s winget

3) Run in powershell:

    oh-my-posh init pwsh --config ~/jandedobbeleer.omp.json | Invoke-Expression

4) Run in powershell:

    code $PROFILE

5) Run in powershell (optional):

    if #4 fails, then:
        5.1) New-Item -Path $PROFILE -Type File -Force
        5.2) Repeat #4

6) Add the following lines to the file ($PROFILE):

    6.1) oh-my-posh init pwsh --config 'C:\Users\user\themes\yourtheme.omp.json' | Invoke-Expression

7) Run in powershell (getting icons):

    Install-Module -Name Terminal-Icons -Repository PSGallery
        7.1) Run in powershell
                code $PROFILE
        7.2)  Add the following lines to the file ($PROFILE):
                Import-Module -Name Terminal-Icons

```

## File $profile

![screenshot](profile.png)

## Results

![screenshot](oh-my-posh-askjr-theme.png)

![screenshot](oh-my-posh-askjr-theme-2.png)

![screenshot](icons.png)
