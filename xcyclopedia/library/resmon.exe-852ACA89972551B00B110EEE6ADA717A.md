﻿---
title: resmon.exe | Resource Monitor
---

# resmon.exe 

* File Path: `C:\Windows\system32\resmon.exe`
* Description: Resource Monitor

## Hashes

Type | Hash
-- | --
MD5 | `852ACA89972551B00B110EEE6ADA717A`
SHA1 | `E1DB406505EC0492825E83D81C9C0274C1ACF1AD`
SHA256 | `4C0BDF906AF0C1FDBC9FA61BF2AF95C708498F5AFE8E05C65E865E99DEAC8716`
SHA384 | `3BECAD8F946B4B7A1D2A16ADC98A4EF7BA372A4086A050C50241E333C7C90EDDAA507FD530380DAF8A7BF63BCBF7708A`
SHA512 | `9E388B1325CFDA2597428D9B44EE48B491D29DBF0840065DEAC7C75F3647757EEFD8AA5D1E8B33AA119C742EB71751FA94B66B47574C9A4F65A5F25025372664`
SSDEEP | `1536:5EZgvhlKBqY3KtrtizIo9plJSs9kYuZJnGZLzOcE6Ls7HXG84PK05Z34g/CO+sH:c6KghtYIo9piswTogiqQKy349`

## Runtime Data

### Child Processes:
perfmon.exe

## Signature

* Status: Signature verified.
* Serial: `330000026551AE1BBD005CBFBD000000000265`
* Thumbprint: `E168609353F30FF2373157B4EB8CD519D07A2BFF`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: resmon.exe
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.19041.1 (WinBuild.160101.0800)
* Product Version: 10.0.19041.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.

## File Similarity (ssdeep match)

File | Score
-- | --
[C:\Windows\system32\perfmon.exe](perfmon.exe-52BC3295597B70B1380FAA6E32BEFAD3.md) | 68
[C:\WINDOWS\system32\perfmon.exe](perfmon.exe-AE3D54BF0D325BDFB785B86511930E37.md) | 72
[C:\windows\system32\perfmon.exe](perfmon.exe-CB1511A4E14C072450E5A61BD74859E3.md) | 79
[C:\Windows\system32\perfmon.exe](perfmon.exe-D38AA59C3BEA5456BD6F95C73AD3C964.md) | 68
[C:\Windows\system32\perfmon.exe](perfmon.exe-D761794B0779B9951349E2F2507B25BC.md) | 69
[C:\windows\system32\resmon.exe](resmon.exe-6C6E586C858BFE1DE453921F67AA9206.md) | 91
[C:\Windows\system32\resmon.exe](resmon.exe-A01AB6C669DCC17E87C84C0C07D2CFAE.md) | 90
[C:\Windows\system32\resmon.exe](resmon.exe-C9221473CE8A3EF5C0FB8ABB912786FA.md) | 91
[C:\WINDOWS\system32\resmon.exe](resmon.exe-FF8CA7D9F879E176A1284F16A05A618C.md) | 93
[C:\WINDOWS\SysWOW64\perfmon.exe](perfmon.exe-14ACB06686DC70FAB341DE0721B71BF1.md) | 74
[C:\Windows\SysWOW64\perfmon.exe](perfmon.exe-6284C86A1AE399794C18FBBC86CC8340.md) | 72
[C:\windows\SysWOW64\perfmon.exe](perfmon.exe-660927A8213F3A9AB378BDFB195E7277.md) | 69
[C:\Windows\SysWOW64\perfmon.exe](perfmon.exe-805F9B64745C730A6BD789083D0EF4E2.md) | 69
[C:\Windows\SysWOW64\perfmon.exe](perfmon.exe-97F73727B423C2FEE513EB7A06E357E5.md) | 69
[C:\windows\SysWOW64\resmon.exe](resmon.exe-0FB8985E4D0F7D37BC366CFD93B73A52.md) | 90
[C:\Windows\SysWOW64\resmon.exe](resmon.exe-29C52C15D2D68A4BBE9A36701D31100E.md) | 93
[C:\Windows\SysWOW64\resmon.exe](resmon.exe-87427E88F06D7C568E3E4A8BD838E380.md) | 93
[C:\WINDOWS\SysWOW64\resmon.exe](resmon.exe-B44E84B38D62E787F5154983A71A864F.md) | 93
[C:\Windows\SysWOW64\resmon.exe](resmon.exe-C182C3463D5E5DFFED8F949D2BB781D3.md) | 91

## Possible Misuse

*The following table contains possible examples of `resmon.exe` being misused. While `resmon.exe` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[sigma](https://github.com/Neo23x0/sigma) | [win_susp_taskmgr_parent.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_susp_taskmgr_parent.yml) | `            - '*\resmon.exe'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)



MIT License. Copyright (c) 2020 Strontic.


