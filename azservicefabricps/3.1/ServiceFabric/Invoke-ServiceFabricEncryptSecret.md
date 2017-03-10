---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
schema: 2.0.0
ms.assetid: FE8B509E-E427-43B4-920D-B6392449788A
updated_at: '11/03/2016 08:11 AM'
ms.date: 11/03/2016
content_git_url: 'https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Invoke-ServiceFabricEncryptSecret.md'
original_content_git_url: 'https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Invoke-ServiceFabricEncryptSecret.md'
gitcommit: 'https://github.com/Azure/azure-docs-powershell-servicefabric/blob/1ee1eb862e0b78a20a656aad5e958efd0f11f85c'
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: 'powershell, cmdlet'
---

# Invoke-ServiceFabricEncryptSecret

## SYNOPSIS
Encrypts text in the cluster manifest by using a certificate.

## SYNTAX

```
Invoke-ServiceFabricEncryptSecret [-CertThumbPrint] <String> [-CertStoreLocation] <String> [-Text] <String>
 [<CommonParameters>]
```

## DESCRIPTION
The **Invoke-ServiceFabricEncryptSecret** cmdlet encrypts text in the Service Fabric cluster manifest by using a certificate.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the [Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md) cmdlet.

## EXAMPLES

### Example 1: Encrypt plain text
```
PS C:\>Invoke-ServiceFabricEncryptSecret -CertThumbPrint "22 5c 58 43 48 50 92 57 2c 22 32 26 ae 67 87 ba c2 f1 cf 24" -CertStoreLocation "MY" -Text "xstore:DefaultEndpointsProtocol=https;AccountName=servicefabricstorage;AccountKey=[StorageAccountKey];Container=clusterupgrade"
```

This command encrypts the specified plain text.
The command specifies the certificate thumbprint and store name.

## PARAMETERS

### -CertStoreLocation
Specifies the location of the certificate in the certificate store.
The default location is MY.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertThumbPrint
Specifies the thumbprint of the certificate to use for encrypting.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Text
Specifies the string to encrypt.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
You cannot pipe input to this cmdlet.

## OUTPUTS

### System.Object
This cmdlet returns the encrypted secret as a **String**.

## NOTES

## RELATED LINKS

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[Get-ServiceFabricClusterConnection](./Get-ServiceFabricClusterConnection.md)