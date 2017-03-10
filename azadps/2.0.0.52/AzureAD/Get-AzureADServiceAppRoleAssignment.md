---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
ms.assetid: D1D9AB94-8FEE-44D9-A4A3-F023905A5717
schema: 2.0.0
updated_at: '02/04/2017 08:02 AM'
ms.date: 02/04/2017
content_git_url: 'https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADServiceAppRoleAssignment.md'
original_content_git_url: 'https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADServiceAppRoleAssignment.md'
gitcommit: 'https://github.com/Azure/azure-docs-powershell-azuread/blob/3c958c260fe07ce8f34599794f089c4b3c1b8115'
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: 'powershell, cmdlet'
---

# Get-AzureADServiceAppRoleAssignment

## SYNOPSIS
Gets a service principal application role assignment.

## SYNTAX

```
Get-AzureADServiceAppRoleAssignment -ObjectId <String> [-All <Boolean>] [-Top <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureADServiceAppRoleAssignment** cmdlet gets a role assignment for a service principal application in Azure Active Directory (AD).

## EXAMPLES

### Example 1: Retrieve the application role assignments for a service principal
```
PS C:\> $ServicePrincipalId = (Get-AzureADServicePrincipal -Top 1).ObjectId
PS C:\> Get-AzureADServiceAppRoleAssignment -ObjectId $ServicePrincipalId
```

The first command gets the ID of a service principal by using the [Get-AzureADServicePrincipal](./Get-AzureADServicePrincipal.md) cmdlet. 
The command stores the ID in the $ServicePrincipalId variable.

The second command gets the application role assignments for the service principal in identified by $ServicePrincipalId. 

## PARAMETERS

### -All
If true, return all application role assignments. If false, return the number of objects specified by the Top parameter

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -ObjectId
Specifies the ID of a service principal in Azure AD.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Top
The maximum number of records to return.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureADServicePrincipal](./Get-AzureADServicePrincipal.md)

[New-AzureADServiceAppRoleAssignment](./New-AzureADServiceAppRoleAssignment.md)

[Remove-AzureADServiceAppRoleAssignment](./Remove-AzureADServiceAppRoleAssignment.md)
