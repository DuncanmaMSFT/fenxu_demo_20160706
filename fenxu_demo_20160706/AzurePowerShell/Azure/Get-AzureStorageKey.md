---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
---

# Get-AzureStorageKey
## SYNOPSIS
Returns the primary and secondary storage account keys for an Azure storage account.

## SYNTAX

```
Get-AzureStorageKey [-StorageAccountName] <String> [-Profile <AzureSMProfile>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## DESCRIPTION
The Get-AzureStorageKey cmdlet returns an object with the Azure Storage account name, the primary account key, and the secondary account key of the specified Azure storage account as properties.

## EXAMPLES

### --------------------------  Example 1: Get an object that contains primary and secondary storage keys  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\>Get-AzureStorageKey -StorageAccountName "ContosoStore01"
```

This command gets an object with the primary and secondary storage keys for the ContosoStore01 storage account.

### --------------------------  Example 2: Get the primary storage account key and store it in a variable  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\>$ContosoStoreKey = (Get-AzureStorageKey -StorageAccountName "ContosoStore01").Primary
```

This command puts the primary storage account key for the ContosoStore01 storage account in the $ContosoStoreKey variable.

## PARAMETERS

### -StorageAccountName
Specifies the storage account name.

```yaml
Type: String
Parameter Sets: (All)
Aliases: ServiceName

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
@{Text=}

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES
To get help with Node.js, use the help node-dev command.
For help with PHP extensions, use the help php-dev command.

## RELATED LINKS

[Get-AzureStorageAccount]()

[New-AzureStorageAccount]()

[New-AzureStorageKey]()

[Remove-AzureStorageAccount]()

[Set-AzureStorageAccount]()

