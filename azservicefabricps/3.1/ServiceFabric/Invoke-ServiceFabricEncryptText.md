---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
schema: 2.0.0
ms.assetid: 3DED0AB0-1412-4104-A9A6-94D496E4C054
updated_at: '11/03/2016 08:11 AM'
ms.date: 11/03/2016
content_git_url: 'https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Invoke-ServiceFabricEncryptText.md'
original_content_git_url: 'https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Invoke-ServiceFabricEncryptText.md'
gitcommit: 'https://github.com/Azure/azure-docs-powershell-servicefabric/blob/1ee1eb862e0b78a20a656aad5e958efd0f11f85c'
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: 'powershell, cmdlet'
---

# Invoke-ServiceFabricEncryptText

## SYNOPSIS
Encrypts secrets to include in Service Fabric manifests or configurations.

## SYNTAX

### CertStore
```
Invoke-ServiceFabricEncryptText [-Text] <String> [-AlgorithmOid <String>] [-CertStore] -CertThumbprint <String>
 [-StoreName <String>] [-StoreLocation <StoreLocation>] [-TimeoutSec <Int32>] [<CommonParameters>]
```

### CertFile
```
Invoke-ServiceFabricEncryptText [-Text] <String> [-AlgorithmOid <String>] [-CertFile] -Path <String>
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Invoke-ServiceFabricEncryptText** cmdlet encrypts secrets to include in the Service Fabric cluster manifest, application manifest, or application configurations.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the [Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md) cmdlet.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -AlgorithmOid
Specifies the object identifier of the algorithm for this cmdlet.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertFile
Indicates that this cmdlet uses the CertFile option.

```yaml
Type: SwitchParameter
Parameter Sets: CertFile
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertStore
Indicates that this cmdlet uses the CertStore option.

```yaml
Type: SwitchParameter
Parameter Sets: CertStore
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertThumbprint
Specifies the thumbprint of a certificate.

```yaml
Type: String
Parameter Sets: CertStore
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Path
Specifies a path of a .cert or .pfx file.

```yaml
Type: String
Parameter Sets: CertFile
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StoreLocation
Specifies the location of a certificate store.
Valid values are:

- CurrentUser
- LocalMachine

```yaml
Type: StoreLocation
Parameter Sets: CertStore
Aliases:
Accepted values: CurrentUser, LocalMachine

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StoreName
Specifies the name of a certificate store.

```yaml
Type: String
Parameter Sets: CertStore
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Text
Specifies the text for the cmdlet.

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

### -TimeoutSec
Specifies the time-out period, in seconds, for the operation.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
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
This cmdlet returns encrypted text as a string.

## NOTES

## RELATED LINKS

[Invoke-ServiceFabricDecryptText](./Invoke-ServiceFabricDecryptText.md)

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[Get-ServiceFabricClusterConnection](./Get-ServiceFabricClusterConnection.md)