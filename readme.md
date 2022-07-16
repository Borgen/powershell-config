Info about Powershell Profile: https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_powershell_config?view=powershell-7.2


1. Install a NerdFont
2. Get cross-platform Powershell from Windows Store
3. Set it as default profile in Windows Terminal

4. Check your powershell profile path:

`$PROFILE.CurrentUserCurrentHost`

5. This must be the file in the repo: Microsoft.Powershell_profile.ps1
6. This file points to the custom configuration script.
7. Create the custome configuration script file. For example:
`C:\Users\test\.config\user_profile.ps1`

8. Install the requirements
    - Oh My Posh `winget install JanDeDobbeleer.OhMyPosh -s winget`
	- Scoop `iwr -useb get.scoop.sh |iex` 
	- `Install-Module posh-git -Scope CurrentUser`
	- `Install-Module -Name Terminal-Icons -Repository PSGallery`
	- `Install-Module -Name z -Force`
	- `Install-Module -Name PSReadLine -AllowPrerelease -Scope CurrentUser`
	- `scoop install fzf`
	- `Install-Module -Name PSFzf -Scope CurrentUser`

9. Copy the `omp.json` file to the `$env:POSH_THEMES_PATH` directory
