# David's Happy Place

## Assumptions and Requirements
- We are using Windows.
- This repository is cloned inside `%USERPROFILE%`.

## Good to Know
On Windows, we can use some of these environment variables for path shortcuts:

```Shell
> echo %USERPROFILE%
C:\Users\dchen

> echo %APPDATA%
C:\Users\dchen\AppData\Roaming
```
More found here: https://stackoverflow.com/questions/39917351/is-there-more-shortcuts-like-appdata

## General Pattern
Run Windows Command Prompt as administrator and run:
```Shell
mklink <destination> <source>
```

## Bash
### .bashrc
```Shell
mklink "%USERPROFILE%\.bashrc" "%USERPROFILE%\dotfiles\bash\.bashrc"
```
### .bash_profile
```Shell
N/A
```

## Git
### .gitconfig
```Shell
mklink "%USERPROFILE%\.gitconfig" "%USERPROFILE%\dotfiles\git\.gitconfig"
```
### .gitignore
```Shell
mklink "%USERPROFILE%\.gitignore" "%USERPROFILE%\dotfiles\git\.gitignore"
```

## Visual Studio Code
### User Settings
```Shell
mklink "%APPDATA%\Code\User\settings.json" "%USERPROFILE%\dotfiles\vscode\user_settings.json"
```
### Workspace Settings
```Shell
N/A
```


