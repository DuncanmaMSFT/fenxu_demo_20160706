---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
---

# Set-AzureVMBGInfoExtension
## SYNOPSIS
Sets the BGInfo extension for a virtual machine.

## SYNTAX

### SetBGInfoExtension (Default)
```
Set-AzureVMBGInfoExtension [-Disable] [[-ReferenceName] <String>] [[-Version] <String>] -VM <IPersistentVM>
 [-Profile <AzureSMProfile>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

### UninstallBGInfoExtension
```
Set-AzureVMBGInfoExtension [-Uninstall] [[-ReferenceName] <String>] [[-Version] <String>] -VM <IPersistentVM>
 [-Profile <AzureSMProfile>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
```

## DESCRIPTION
The Set-AzureVMBGInfoExtension cmdlet sets the BGInfo extension for a virtual machine.

## EXAMPLES

### --------------------------  Example 1: Set the BGInfo extension for a virtual machine  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\>Set-AzureVMBGInfoExtension -VM $VM
```

This command sets the BGInfo extension for the specified virtual machine as stored in the variable $VM.

## PARAMETERS

### -Disable
Indicates that this cmdlet disables the extension state.

```yaml
Type: SwitchParameter
Parameter Sets: SetBGInfoExtension
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ReferenceName
Specifies the reference name of the BGInfo extension.

This parameter is a user-defined string that can be used to refer to an extension.
It is specified when the extension is added to the virtual machine for the first time.
You can specify the previously used reference name while updating the extension.
The ReferenceName assigned to an extension is returned by the Get-AzureVM cmdlet.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Version
Specifies the version of the BGInfo extension.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VM
Specifies the persistent virtual machine object.

```yaml
Type: IPersistentVM
Parameter Sets: (All)
Aliases: InputObject

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
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

### -Uninstall
Indicates that this cmdlet uninstalls the BGInfo extension.

```yaml
Type: SwitchParameter
Parameter Sets: UninstallBGInfoExtension
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureVMBGInfoExtension]()

[Remove-AzureVMBGInfoExtension]()

