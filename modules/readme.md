List module versions that are available on the system  
`get-module pester -listavailable`  

Install a module named 'Pester' version  
`Install-Module -Name Pester -Force -SkipPublisherCheck`


`.Tests.ps1` is a key word that pester uses to know which files should be executed when running `Invoke-Pester`  

Pester contains the following blocks
- Describe
- Context
- It

When you are writing a pester test, source in the script as follows  
```
. $PSScriptRoot\Get-ServiceProperty.ps1

# pester configuration below
```
