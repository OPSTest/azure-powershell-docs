---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
ms.assetid: D2CCAEB4-E43E-4075-9436-77F2C4FE9463
schema: 2.0.0
updated_at: '03/11/2017 23:03 PM'
ms.date: 03/11/2017
content_git_url: 'https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.7.0/Get-AzureRmVMImageOffer.md'
original_content_git_url: 'https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.7.0/Get-AzureRmVMImageOffer.md'
gitcommit: 'https://github.com/Azure/azure-docs-powershell/blob/bc71000aa3c7f754b95442dcc415a7324626a15c'
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: 'powershell, cmdlet'
---

# Get-AzureRmVMImageOffer

## SYNOPSIS
Gets VMImage offer types.

## SYNTAX

```
Get-AzureRmVMImageOffer -Location <String> -PublisherName <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmVMImageOffer** cmdlet gets the VMImage offer types.

## EXAMPLES

### Example 1: Get offer types for a publisher
```
PS C:\>Get-AzureRmVMImageOffer -Location "Central US" -PublisherName "Fabrikam"
```

This command gets the offer types for the specified publisher in the Central US region.

## PARAMETERS

### -Location
Specifies the location of the VMImage.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PublisherName
Specifies the name of a publisher of a VMImage.
To obtain a publisher, use the Get-AzureRmVMImagePublisher cmdlet.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmVMImage](./Get-AzureRmVMImage.md)

[Get-AzureRmVMImagePublisher](./Get-AzureRmVMImagePublisher.md)

[Get-AzureRmVMImageSku](./Get-AzureRmVMImageSku.md)

[Save-AzureRmVMImage](./Save-AzureRmVMImage.md)


