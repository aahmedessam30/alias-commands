# Alias Commands
This repository contains a list of aliases that I use in PowerShell and Git Bash.

## How to Create an Alias In PowerShell?
To create an alias, first open PowerShell and type the following command:

```powershell
Test-Path $PROFILE
```

If the command returns `False`, you need to create a profile. To create a profile, type the following command:

```powershell
New-Item -Type File -Force $PROFILE
```

After creating the profile, you can open it by typing the following command:

```powershell
notepad $PROFILE
```

In the profile, copy the `powershell-alias.txt` content to this profile and reload the powershell profile by typing the following command:

```powershell
    . $PROFILE
```

After reload the profile verify aliases, for example:

```powershell
    pa # should return `php artisan` commands
```