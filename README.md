# Active-Directory-Cheat-Sheet
some enum commands for AD
# Domain Enumeration with PowerView

Get Current domain : 
Get-NetDomain

Get object of another domain: 
Get-NetDomain -Domain thinc.local

Get domain policy for the current domain : 
Get-DomainPolicy 
show details for a specific policy : 
(Get-DomainPolicy)."system access"

Get domain controller details : 
Get-NetDomainController

Get a list of users in the current domain:
Get-NetUser
Get-NetUser -Username sazouki

Get list of all properties for users in the current domain
Get-UserProperty
Get-UserProperty -Properties pwdlastset

Get a list of computers in the current domain:
Get-NetComputer

Get list of groups in the current domain:
Get-NetGroup -FullData
Get-NetGroupMember -GroupName 'Domain Admins' // this will show all the members in the domain admins group
