---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
ms.assetid: F9A652D0-26D9-4F3F-A365-285B05AA7C0B
schema: 2.0.0
updated_at: '03/11/2017 23:03 PM'
ms.date: 03/11/2017
content_git_url: 'https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v3.5.0/Get-AzureRmSiteRecoverySite.md'
original_content_git_url: 'https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v3.5.0/Get-AzureRmSiteRecoverySite.md'
gitcommit: 'https://github.com/Azure/azure-docs-powershell/blob/bc71000aa3c7f754b95442dcc415a7324626a15c'
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: 'powershell, cmdlet'
---

# Get-AzureRmSiteRecoverySite

## SYNOPSIS
Gets the Hyper-V sites from the Site Recovery vault.

## SYNTAX

### Default (Default)
```
Get-AzureRmSiteRecoverySite [<CommonParameters>]
```

### ByName
```
Get-AzureRmSiteRecoverySite -Name <String> [<CommonParameters>]
```

### ByFriendlyName
```
Get-AzureRmSiteRecoverySite -FriendlyName <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmSiteRecoverySite** cmdlet gets the Hyper-V sites in the Azure Site Recovery vault.

## EXAMPLES

## PARAMETERS

### -Name
Specifies the name of the site.

```yaml
Type: String
Parameter Sets: ByName
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FriendlyName
Specifies the friendly name of the site.

```yaml
Type: String
Parameter Sets: ByFriendlyName
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureRmSiteRecoverySite](./New-AzureRmSiteRecoverySite.md)

[Remove-AzureRmSiteRecoverySite](./Remove-AzureRmSiteRecoverySite.md)
