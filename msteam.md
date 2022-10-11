# msteam config

## check package install

https://learn.microsoft.com/en-us/microsoftteams/teams-powershell-install

````
Install-Module -Name PowerShellGet -Force -AllowClobber

Install-Module -Name MicrosoftTeams -Force -AllowClobber
````

## Login
````
Connect-MicrosoftTeams  <LOGIN>
````
### OR
````
Connect-MicrosoftTeams -UseDeviceAuthentication
````

### for enter code

````
https://microsoft.com/devicelogin
````

## Enabled

````
Set-CsTeamsMeetingPolicy -Identity Global -StreamingAttendeeMode Enabled

````

## Disabled

````
Set-CsTeamsMeetingPolicy -Identity Global -StreamingAttendeeMode Disabled
````


## option

````
Get-ExecutionPolicy

Set-ExecutionPolicy unrestricted

set-executionpolicy remotesigned

Set-ExecutionPolicy -ExecutionPolicy RemoteSigned
````
