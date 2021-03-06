﻿---
title: tsdiscon.exe | Session Disconnection Utility
---

# tsdiscon.exe 

* File Path: `C:\windows\SysWOW64\tsdiscon.exe`
* Description: Session Disconnection Utility

## Hashes

Type | Hash
-- | --
MD5 | `0AB55415F17FAB49F9EC2053B37498E4`
SHA1 | `F44BDFC145C4239CC001772E2B194714502839CC`
SHA256 | `E46C156D2116416C1C27EB47B46E891EC7BC12522B73F646D576477B71AA69BA`
SHA384 | `D8D526D8F3A4BBAC5C2DC5D890DF4538E52F6BFBA15EDEE01D2C06162A3CBF1A5367EF0EC62851527F42CC8FC8EBC3D1`
SHA512 | `A72009017666D8BC3A736CD76E2B7A4323F2EB77C536783C85A77FC97D35E845ECB46F5484DAE5243E76C18F8DB88E632E89E177BDDA3C731930EE49669F3DFD`
SSDEEP | `384:CKKO+SJ/I9io3wZBkFBRakXhUTh5piWbG4uQWMnWW:CnSJYNq5XuY`

## Signature

* Status: The file C:\windows\SysWOW64\tsdiscon.exe is not digitally signed. You cannot run this script on the current system. For more information about running scripts and setting execution policy, see about_Execution_Policies at http://go.microsoft.com/fwlink/?LinkID=135170
* Serial: ``
* Thumbprint: ``
* Issuer: 
* Subject: 

## File Metadata

* Original Filename: tsdiscon.exe.mui
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 6.3.9600.16384 (winblue_rtm.130821-1623)
* Product Version: 6.3.9600.16384
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.



## Additional Info*

**The information below is copied from [MicrosoftDocs](https://github.com/MicrosoftDocs/windowsserverdocs), which is maintained by [Microsoft](https://opensource.microsoft.com/codeofconduct/). Available under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.*

---
## tsdiscon

> Applies to: Windows Server (Semi-Annual Channel), Windows Server 2019, Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

Disconnects a session from a Remote Desktop Session Host server.



> [!NOTE]
> In Windows Server 2008 R2, Terminal Services was renamed Remote Desktop Services. To find out what's new in the latest version, see [What s New in Remote Desktop Services in Windows Server 2012](/previous-versions/orphan-topics/ws.11/hh831527(v=ws.11)) in the Windows Server TechNet Library.

### Syntax
```
tsdiscon [<SessionID> | <SessionName>] [/server:<ServerName>] [/v]
```

#### Parameters

|Parameter|Description|
|-------|--------|
|\<SessionId>|Specifies the ID of the session to disconnect.|
|\<SessionName>|Specifies the name of the session to disconnect.|
|/server:\<ServerName>|Specifies the terminal server that contains the session that you want to disconnect. Otherwise, the current rd Session Host server is used.|
|/v|Displays information about the actions being performed.|
|/?|Displays help at the command prompt.|

### Remarks
-   You must have Full Control permission or Disconnect special access permission to disconnect another user from a session.
-   if no session ID or session name is specified, **tsdiscon** disconnects the current session.
-   Any applications that were running when you disconnected the session are automatically running when you reconnect to that session with no loss of data. Use **reset session** to end the running applications of the disconnected session, but be aware that this might result in loss of data at the session.
-   The **/server** parameter is required only if you use **tsdiscon** from a remote server.
-   The console session cannot be disconnected.

### Examples
- To disconnect the current session, type:
  ```
  tsdiscon
  ```
- To disconnect session 10, type:
  ```
  tsdiscon 10
  ```
- To disconnect the session named TERM04, type:
  ```
  tsdiscon TERM04
  ```
  ## Additional References
  - [Command-Line Syntax Key](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/command-line-syntax-key.md)
  [Remote Desktop Services (Terminal Services) Command Reference](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/remote-desktop-services-terminal-services-command-reference.md)

---



MIT License. Copyright (c) 2020 Strontic.


