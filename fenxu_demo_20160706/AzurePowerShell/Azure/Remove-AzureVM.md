---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
---

# Remove-AzureVM
## SYNOPSIS
Removes an Azure virtual machine.

## SYNTAX

```
Remove-AzureVM [-Name] <String> [-DeleteVHD] [-ServiceName] <String> [-Profile <AzureSMProfile>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf] [-Confirm]
```

## DESCRIPTION
The Remove-AzureVM cmdlet deletes an Azure virtual machine.
This process does not delete the underlying .vhd files of the disks mounted on that virtual machine.

## EXAMPLES

### --------------------------  Example 1: Remove a virtual machine from a service  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\>Remove-AzureVM -ServiceName "ContosoService03" -Name "VirtualMachine03"
```

This command removes the virtual machine named VirtualMachine03 that runs in the ContosoService03 service.

### --------------------------  Example 2: Remove a virtual machine and delete the .vhd files  --------------------------
@{paragraph=PS C:\\\>}

```
PS C:\>Remove-AzureVM -ServiceName "ContosoService03" -Name "VirtualMachine04" -DeleteVHD
```

This command removes the VirtualMachine04 virtual machine that runs in the ContosoService03 service, and specifies to remove the .vhd files using the DeleteVHD parameter.

## PARAMETERS

### -Name
Specifies the name of the virtual machine being removed.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DeleteVHD
Specifies whether this cmdlet removes the virtual machine and the underlying disk blobs.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceName
Specifies the name of the Azure service from which the virtual machine is being removed.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

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

### -WhatIf
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureVM]()

[New-AzureVMConfig]()

[Restart-AzureVM]()

[Start-AzureVM]()

[Stop-AzureVM]()

[Update-AzureVM]()

