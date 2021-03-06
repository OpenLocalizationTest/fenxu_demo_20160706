---
external help file: RMAzure_Apimanagement.xml
online version: 73f73a6f-470c-4dd6-95c4-a1302fabb0dd
schema: 2.0.0
source_branch: master
source_repo: https://github.com/Visual-Studio-China/azure-powershell-docs-int
---

# Import-AzureRmApiManagementHostnameCertificate
## SYNOPSIS
Imports a certificate in a PFX format for an API Management Service.

## SYNTAX

```
Import-AzureRmApiManagementHostnameCertificate [-PassThru] [-HostnameType] -Name <String> -PfxPassword <String>
 -PfxPath <String> -ResourceGroupName <String>
```

## DESCRIPTION
The **Import-AzureRmApiManagementHostnameCertificate** cmdlet imports a certificate in a PFX format for an API Management Service.
The certificate is to be used for custom hostnames configuration.

## EXAMPLES

### Example 1: Import a API Management hostname certificate
```
PS C:\>Import-AzureRmApiManagementHostnameCertificate -Name "ContosoApi" -ResourceGroupName Contoso -HostnameType "Proxy" -PfxPath "C:\proxycert.pfx" -PfxPassword "CertSecret"
```

This command imports a certificate for a proxy custom hostname.

## PARAMETERS

### -HostnameType
Specifies the host name type that this cmdlet loads the certificate for.

Valid values are: 

-- Proxy
-- Portal

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: Proxy, Portal

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the API Management deployment that this cmdlet imports.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
passthru

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PfxPassword
Specifies the password for the .pfx certificate file.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PfxPath
Specifies the path to a .pfx certificate file.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the of resource group under which the API Management deployment exists.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureRmApiManagementHostnameConfiguration](73f73a6f-470c-4dd6-95c4-a1302fabb0dd)

[Set-AzureRmApiManagementHostnames](dd997f04-b85b-409c-8c69-a5e659c768e3)


