
        SIEM-Speak
        Say for Windows - PowerShell
        greg . foss [at] logrhythm . com
        v0.1 -- July, 2017

## [About]

Ever wished that you could have the great OS X 'say' command on your Windows system? Or better yet, other people's Windows systems?
Well, look no further - you can now prank everyone equally! Or, integrate audible alerts with the SIEM, and do real business things with it, or whatever.

Blog => TBD

## [Install]

		Import the SIEM-Speak
			PS C:\> Import-Module .\say.ps1

## [Usage]

		Download and load the say.ps1 script
			PS C:\> IEX (New-Object Net.WebClient).DownloadString('https://gist.githubusercontent.com/gfoss/7b0368bc300e1b4683d090501f7ab6bc/raw/b9f47e559b3c48874343cfc70e363068b29bf165/say.ps1’)

		Test it out
			PS C:\> say “Something”

		Prank others :-D
			PS C:\> Enter-PSSession -ComputerName 10.10.10.10 -Credential Get-Credential; < repeat steps 1 & 2 >

		LogRhythm SIEM Integration
			Add the say.lpi file to LogRhythm, and integrate with alarms

## [License]

Copyright 2017 LogRhythm Inc.   
Licensed under the MIT License. See LICENSE file in the project root for full license information.
