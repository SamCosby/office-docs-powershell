---
external help file: sharepoint.xml
online version: http://technet.microsoft.com/EN-US/library/2a074a5a-0af0-48fd-aa1f-edc875f93335(Office.15).aspx
schema: 2.0.0
---

# New-SPEnterpriseSearchServiceApplicationProxy

## SYNOPSIS
Adds a new search application proxy to a farm.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
New-SPEnterpriseSearchServiceApplicationProxy [[-Name] <String>]
 -SearchApplication <SearchServiceApplicationPipeBind> [-AssignmentCollection <SPAssignmentCollection>]
 [-Confirm] [-MergeWithDefaultPartition] [-Partitioned] [-WhatIf]
```

### UNNAMED_PARAMETER_SET_2
```
New-SPEnterpriseSearchServiceApplicationProxy [[-Name] <String>] -Uri <String>
 [-AssignmentCollection <SPAssignmentCollection>] [-Confirm] [-MergeWithDefaultPartition] [-Partitioned]
 [-WhatIf]
```

## DESCRIPTION
This cmdlet contains more than one parameter set.
You may only use parameters from one parameter set, and you may not combine parameters from different parameter sets.
For more information about how to use parameter sets, see Cmdlet Parameter Sets (http://go.microsoft.com/fwlink/?LinkID=187810).

This cmdlet creates a proxy for a search service application.
The search service application proxy can be used by a web application or another service consumer to use the functionality that is provided by the search application.

This cmdlet contains more than one parameter set.
You may only use parameters from one parameter set, and you may not combine parameters from different parameter sets.
For more information about how to use parameter sets, see Cmdlet Parameter Sets (http://msdn.microsoft.com/en-us/library/dd878348(VS.85).aspx).

For permissions and the most current information about Windows PowerShell for SharePoint Products, see the online documentation at http://go.microsoft.com/fwlink/p/?LinkId=251831 (http://go.microsoft.com/fwlink/p/?LinkId=251831).

## EXAMPLES

### ------------------EXAMPLE------------------ (SharePoint Server 2013)
```
New-SPEnterpriseSearchServiceApplicationProxy -Name MyNewProxy -SearchApplication MySSA
```

This example adds a search service application proxy to a search service application named MySSA.

### ------------------EXAMPLE------------------ (SharePoint Server 2016)
```
C:\PS>New-SPEnterpriseSearchServiceApplicationProxy -Name MyNewProxy -SearchApplication MySSA
```

This example adds a search service application proxy to a search service application named MySSA.

## PARAMETERS

### -Name
Specifies the display name of the search application proxy to create.

The type must be a valid string, for example, SearchAppProxy1.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SearchApplication
Specifies the URI to the search application to use for search.

The type must be a valid URI, in the form file:\\\\server_name\searchapp.

```yaml
Type: SearchServiceApplicationPipeBind
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Uri
Specifies the URI to the search application to use for search.

The type must be a valid URI, in the form file:\\\\server_name\searchapp.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AssignmentCollection
Manages objects for the purpose of proper disposal.
Use of objects, such as SPWeb or SPSite, can use large amounts of memory and use of these objects in Windows PowerShell scripts requires proper memory management.
Using the SPAssignment object, you can assign objects to a variable and dispose of the objects after they are needed to free up memory.
When SPWeb, SPSite, or SPSiteAdministration objects are used, the objects are automatically disposed of if an assignment collection or the Global parameter is not used.

When the Global parameter is used, all objects are contained in the global store.
If objects are not immediately used, or disposed of by using the Stop-SPAssignment command, an out-of-memory scenario can occur.

```yaml
Type: SPAssignmentCollection
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before executing the command.
For more information, type the following command: get-help about_commonparameters

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -MergeWithDefaultPartition
Merges the index partition for the proxy with the default index partition collection for the search service application.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Partitioned
Specifies that the search service application must use web-hosted mode.
web-hosted mode segregates results for a given hosted subscription.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Displays a message that describes the effect of the command instead of executing the command.
For more information, type the following command: get-help about_commonparameters

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Online Version](http://technet.microsoft.com/EN-US/library/2a074a5a-0af0-48fd-aa1f-edc875f93335(Office.15).aspx)
