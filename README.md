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
Run Windows Command Prompt as administrator

```Shell
mklink <destination> <source>
```