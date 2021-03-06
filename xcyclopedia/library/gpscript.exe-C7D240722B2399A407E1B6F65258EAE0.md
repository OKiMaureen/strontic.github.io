﻿---
title: gpscript.exe | Group Policy Script Application
---

# gpscript.exe 

* File Path: `C:\Windows\system32\gpscript.exe`
* Description: Group Policy Script Application

## Hashes

Type | Hash
-- | --
MD5 | `C7D240722B2399A407E1B6F65258EAE0`
SHA1 | `0935ACA1D24B67D0ACB80258E2C1D049AFBDB7A2`
SHA256 | `6D01F0FBA4F2DF370DFF5C91728C407DF8E364470E1D6776BF25C6248B938212`
SHA384 | `C6D70EA0942727BA2000795ADCAD9A7E6910BB171DF3494F101A343E6B7565F6231E48FC763A2F77E2FBE0D617E83DAE`
SHA512 | `1436D7C9CD5F757DE622701753FC9B6DE330387D46DAE39612C204A6B79500E46DD2EE77DCAECE391F84D2B098C0AD388AF327022C4BBC316157B4D316309480`
SSDEEP | `768:vPx149fDVT7oUke5GZeEyLJ+885rAJl0ex0HslgTdTcgdCtZ7M:XxeDp8k5GZelN+88pa+ex0HfTdTldQM`

## Signature

* Status: Signature verified.
* Serial: `3300000266BD1580EFA75CD6D3000000000266`
* Thumbprint: `A4341B9FD50FB9964283220A36A1EF6F6FAA7840`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: GPSCRIPT.EXE
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.19041.1 (WinBuild.160101.0800)
* Product Version: 10.0.19041.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.


## Possible Misuse

*The following table contains possible examples of `gpscript.exe` being misused. While `gpscript.exe` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Gpscript.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSBinaries/Gpscript.yml) | `Name: Gpscript.exe` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Gpscript.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSBinaries/Gpscript.yml) | `  - Command: Gpscript /logon` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Gpscript.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSBinaries/Gpscript.yml) | `  - Command: Gpscript /startup` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Gpscript.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSBinaries/Gpscript.yml) | `  - Path: C:\Windows\System32\gpscript.exe` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Gpscript.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSBinaries/Gpscript.yml) | `  - Path: C:\Windows\SysWOW64\gpscript.exe` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Gpscript.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSBinaries/Gpscript.yml) | ` - IOC: Execution of Gpscript.exe after logon` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Gpscript.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSBinaries/Gpscript.yml) | `  - Link: https://oddvar.moe/2018/04/27/gpscript-exe-another-lolbin-to-the-list/` | 



MIT License. Copyright (c) 2020 Strontic.


