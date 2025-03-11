---
external help file: Microsoft.Teams.Policy.Administration.Cmdlets.Core.dll-Help.xml
Module Name: MicrosoftTeams
online version:
schema: 2.0.0
---

# Get-CsTeamsBYODAndDesksPolicy

## SYNOPSIS
The CsTeamsMeetingPolicy cmdlets enables administrators to control the device data collection done for BYOD rooms and hotdesking scenarios.

## SYNTAX

### Identity (Default)
```
Get-CsTeamsBYODAndDesksPolicy [[-Identity] <String>] [<CommonParameters>]
```

### Filter
```
Get-CsTeamsBYODAndDesksPolicy [-Filter <String>] [<CommonParameters>]
```

## DESCRIPTION
The BYOD Rooms and Bookable desks in Microsoft Teams use peripheral data crowdsourced from the Teams desktop client running on the users' laptops to discover peripherals as well as understand when those desk pools they are associated to are used. No personally identifiable data is collected, but should you feel this data collection is inappropriate for your tenant or a group of users in your tenant, you may use the following PowerShell cmdlets to configure the policy appropriately.

## EXAMPLES

### Example 1
```powershell
PS C:\> Get-CsTeamsBYODAndDesksPolicy

Identity      DeviceDataCollection
--------      --------------------
Global        Disabled
Tag:DeskUsers Enabled
```

Fetches all the policy instances currently available.

### Example 2
```powershell
PS C:\> Get-CsTeamsBYODAndDesksPolicy -Identity DeskUsers

Identity      DeviceDataCollection
--------      --------------------
Tag:DeskUsers Enabled
```

Fetches the policy instances available for the specified identity.

## PARAMETERS

### -Filter
{{ Fill Filter Description }}

```yaml
Type: String
Parameter Sets: Filter
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Identity
{{ Fill Identity Description }}

```yaml
Type: String
Parameter Sets: Identity
Aliases:

Required: False
Position: 1
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
