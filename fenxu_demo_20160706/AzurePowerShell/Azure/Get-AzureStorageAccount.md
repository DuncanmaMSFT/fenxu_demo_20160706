---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
---

# Get-AzureStorageAccount
## SYNOPSIS
Gets the storage accounts for the current Azure subscription.

## SYNTAX

```
Get-AzureStorageAccount [[-StorageAccountName] <String>] [-Profile <AzureSMProfile>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## DESCRIPTION
The Get-AzureStorageAccount cmdlet returns an object containing information about the storage accounts for the current subscription.
If the StorageAccountName parameter is specified, then only information about the specified storage account is returned.

## EXAMPLES

### --------------------------  Example 1: Return all storage accounts  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\>Get-AzureStorageAccount
```

This command returns an object with all the storage accounts associated with the current subscription.

### --------------------------  Example 2: Return account information for a specified account  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\>Get-AzureStorageAccount -StorageAccountName "ContosoStore01"
```

This command returns an object with only the ContosoStore01 account information.

### --------------------------  Example 3: Display a table of storage accounts  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\>Get-AzureStorageAccount | Format-Table -AutoSize -Property @{Label="Name";Expression={$_.StorageAccountName}},"Label","Location"
```

This command returns an object with all the storage accounts associated with the current subscription, and outputs them as a table showing the account name, the account label, and the storage location.

## PARAMETERS

### -StorageAccountName
Specifies the name of a storage account.
If specified, this cmdlet returns only the specified storage account object.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
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

### ManagementOperationContext

## NOTES
Type help node-dev to get help on Node.js development-related cmdlets.
Type help php-dev to get help on PHP development-related cmdlets.

## RELATED LINKS

[New-AzureStorageAccount]()

[Set-AzureStorageAccount]()

