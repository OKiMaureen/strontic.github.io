﻿---
title: perfmon.exe | Resource and Performance Monitor
---

# perfmon.exe 

* File Path: `C:\Windows\system32\perfmon.exe`
* Description: Resource and Performance Monitor
* Comments: 

## Hashes

Type | Hash
-- | --
MD5 | `D38AA59C3BEA5456BD6F95C73AD3C964`
SHA1 | `40170EAB389A6BA35E949F9C92962646A302D9EF`
SHA256 | `5F041CFF346FB37E5C5C9DAB3C1272C76F8B5F579205170E97D2248D04A4EA0C`
SHA384 | `59C1DB08828A483F26E7A71A2019619DB9078603916195EC940611FFA0E6809A9F2F31BFE7EE9E926A204DE144EAECE0`
SHA512 | `59FA552A46E5D6237C7244B03D09D60E9489217B4319A212E822C73FE1F31A81837CB906AE7DA92072BD3D9263FE0B967E073110BA81DA3A90126F25115FFF68`
SSDEEP | `3072:Y0fcuMXJEzBG8IPFThJRoGghtYIo9piswTogiqQKy349:hWZEzBG8SFNJWhqIo9s37iTK24`

## Runtime Data

### Usage (stdout):
```Batchfile
Argument 'help' is unknown.

```

### Usage (stderr):
```Batchfile

```

### Child Processes:


## Signature

* Status: Signature verified.
* Serial: `330000023241FB59996DCC4DFF000000000232`
* Thumbprint: `FF82BC38E1DA5E596DF374C53E3617F7EDA36B06`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: perfmon.exe.mui
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.00
* Product Version: 10.00
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.

## File Similarity (ssdeep match)

File | Score
-- | --
[C:\WINDOWS\system32\perfmon.exe](perfmon.exe-AE3D54BF0D325BDFB785B86511930E37.md) | 58
[C:\Windows\system32\perfmon.exe](perfmon.exe-D761794B0779B9951349E2F2507B25BC.md) | 58
[C:\Windows\system32\resmon.exe](resmon.exe-852ACA89972551B00B110EEE6ADA717A.md) | 68
[C:\Windows\system32\resmon.exe](resmon.exe-C9221473CE8A3EF5C0FB8ABB912786FA.md) | 65
[C:\WINDOWS\system32\resmon.exe](resmon.exe-FF8CA7D9F879E176A1284F16A05A618C.md) | 68
[C:\WINDOWS\SysWOW64\perfmon.exe](perfmon.exe-14ACB06686DC70FAB341DE0721B71BF1.md) | 65
[C:\Windows\SysWOW64\perfmon.exe](perfmon.exe-6284C86A1AE399794C18FBBC86CC8340.md) | 68
[C:\Windows\SysWOW64\perfmon.exe](perfmon.exe-805F9B64745C730A6BD789083D0EF4E2.md) | 65
[C:\Windows\SysWOW64\resmon.exe](resmon.exe-29C52C15D2D68A4BBE9A36701D31100E.md) | 65
[C:\Windows\SysWOW64\resmon.exe](resmon.exe-87427E88F06D7C568E3E4A8BD838E380.md) | 66
[C:\WINDOWS\SysWOW64\resmon.exe](resmon.exe-B44E84B38D62E787F5154983A71A864F.md) | 68


## Additional Info*

**The information below is copied from [MicrosoftDocs](https://github.com/MicrosoftDocs/windowsserverdocs), which is maintained by [Microsoft](https://opensource.microsoft.com/codeofconduct/). Available under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.*

---

## perfmon

Start Windows Reliability and Performance Monitor in a specific standalone mode.

### Syntax

```
perfmon </res|report|rel|sys>
```

#### Parameters

|Parameter|Description|
|---------|-----------|
|/res|Start Resource View.|
|/report|Start the System Diagnostics Data Collector Set and display a report of the results.|
|/rel|Start Reliability Monitor.|
|/sys|Start Performance Monitor.|

### Additional References

[Windows Performance Monitor](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2008-R2-and-2008/cc749154(v%3dws.11))

---



MIT License. Copyright (c) 2020 Strontic.

