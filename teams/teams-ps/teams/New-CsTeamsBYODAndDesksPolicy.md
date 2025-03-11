---
external help file: Microsoft.Teams.Policy.Administration.Cmdlets.Core.dll-Help.xml
Module Name: MicrosoftTeams
online version:
schema: 2.0.0
---

# New-CsTeamsBYODAndDesksPolicy

## SYNOPSIS
The CsTeamsMeetingPolicy cmdlets enables administrators to control the device data collection done for BYOD rooms and hotdesking scenarios.

## SYNTAX

```
New-CsTeamsBYODAndDesksPolicy [-DeviceDataCollection <String>] [-Identity] <String> [-Force] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The BYOD Rooms and Bookable desks in Microsoft Teams use peripheral data crowdsourced from the Teams desktop client running on the users' laptops to discover peripherals as well as understand when those desk pools they are associated to are used. No personally identifiable data is collected, but should you feel this data collection is inappropriate for your tenant or a group of users in your tenant, you may use the following PowerShell cmdlets to configure the policy appropriately.

## EXAMPLES

### Example 1
```powershell
PS C:\> New-CsTeamsBYODAndDesksPolicy -Identity DeskUsers -DeviceDataCollection Enabled

Identity      DeviceDataCollection
--------      --------------------
Tag:DeskUsers Enabled
```

Creates a new policy instance with the identity DeskUsers. DeviceDataCollection is set to the value specified in the command.

### Example 1
```powershell
PS C:\> New-CsTeamsBYODAndDesksPolicy -Identity DeskUsers -DeviceDataCollection Disabled

Identity      DeviceDataCollection
--------      --------------------
Tag:DeskUsers Disabled
```

Creates a new policy instance with the identity DeskUsers. DeviceDataCollection is set to the value specified in the command.

## PARAMETERS

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DeviceDataCollection
This setting allows your organisation to collect the peripheral data of the peripherals that are connected to your device. This data is then used for the hotdesking and BYOD rooms scenarios. This gives the tenant an ability to enable or disable the peripheral data collection for the users.

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

### -Force
Suppresses the display of any non-fatal error message that might arise when running the command.

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

### -Identity
Name of the new policy instance to be created.

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

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### TeamsBYODAndDesksPolicy.Cmdlets.TeamsBYODAndDesksPolicy

## NOTES

## RELATED LINKS
