---
title: manage-bde changekey
description: Reference topic for **** - 

ms.prod: windows-server


ms.technology: manage-windows-commands

ms.topic: article
ms.assetid: 69463db9-7e03-47ff-b233-a95d5055725f
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/16/2017
---

# manage-bde: changekey



Modifies the startup key for an operating system drive.

## Syntax

```
manage-bde -changekey [<Drive>] [<PathToExternalKeyDirectory>] [-computername <Name>] [{-?|/?}] [{-help|-h}]
```

#### Parameters

|Parameter|Description|
|---------|-----------|
|\<Drive>|Represents a drive letter followed by a colon.|
|\<PathToExternalKeyDirectory>|Represents the directory location to save the external startup key file that can be used to unlock the drive.|
|-computername|Specifies that Manage-bde.exe will be used to modify BitLocker protection on a different computer. You can also use **-cn** as an abbreviated version of this command.|
|\<Name>|Represents the name of the computer on which to modify BitLocker protection. Accepted values include the computer's NetBIOS name and the computer's IP address.|
|-? or /?|Displays brief Help at the command prompt.|
|-help or -h|Displays complete Help at the command prompt.|

## Examples

To illustrates using the **-changekey** command to create a new startup key on drive E to use with BitLocker encryption on drive C.
```
manage-bde -changekey C: E:\
```

## Additional References

-   - [Command-Line Syntax Key](command-line-syntax-key.md)
-   [Manage-bde](manage-bde.md)
