﻿---
title: ktmutil.exe | Kernel Transaction Management Utility
---

# ktmutil.exe 

* File Path: `C:\Windows\system32\ktmutil.exe`
* Description: Kernel Transaction Management Utility

## Hashes

Type | Hash
-- | --
MD5 | `C9D776B6A4BC22B5B9A0985AB9CD6101`
SHA1 | `FC72D96DF9D0E61A0458280290B27165258D735C`
SHA256 | `81765113B2DF32F13EF09FC96645C183F6064B27FCF4F3A3575088F016BBB5A5`
SHA384 | `056E17A1962F58322DFE61CDF94A7882A2397E981BDEDDD1C84A40BD94F97A1FC9DBE704FC8D49B497C2D86C2D50B9ED`
SHA512 | `E5080ECEEAB1C3A430A93F3B42CC09A295A02F3D3EFA538965AEA19EAE77F870A9191104D92BC373F7E806A2245B507D1D231BFF71CDE5684DD634CA82D75141`
SSDEEP | `384:Pqsz66pGvFTnOVsFkxaHtywf+DgY2+WjjW:Pc68F6hx1VUBD`

## Runtime Data

### Usage (stdout):
```Batchfile
--help is an invalid parameter.
---- Commands Supported ----

tx     Commands related to transactions
tm     Commands related to transaction managers

```

## Signature

* Status: Signature verified.
* Serial: `3300000266BD1580EFA75CD6D3000000000266`
* Thumbprint: `A4341B9FD50FB9964283220A36A1EF6F6FAA7840`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: ktmutil.exe.mui
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.19041.1 (WinBuild.160101.0800)
* Product Version: 10.0.19041.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.



## Additional Info*

**The information below is copied from [MicrosoftDocs](https://github.com/MicrosoftDocs/windowsserverdocs), which is maintained by [Microsoft](https://opensource.microsoft.com/codeofconduct/). Available under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.*

---

## ktmutil

Starts the Kernel Transaction Manager utility. If used without parameters, **ktmutil** displays available subcommands.

### Syntax

```
ktmutil list tms
ktmutil list transactions [{TmGUID}]
ktmutil resolve complete {TmGUID} {RmGUID} {EnGUID}
ktmutil resolve commit {TxGUID}
ktmutil resolve rollback {TxGUID}
ktmutil force commit {GUID}
ktmutil force rollback {GUID}
ktmutil forget
```

### Examples


To force an Indoubt transaction with GUID 311a9209-03f4-11dc-918f-00188b8f707b to commit, type:

```
ktmutil force commit {311a9209-03f4-11dc-918f-00188b8f707b}
```

### Additional References

- [Command-Line Syntax Key](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/command-line-syntax-key.md)

---



MIT License. Copyright (c) 2020 Strontic.


