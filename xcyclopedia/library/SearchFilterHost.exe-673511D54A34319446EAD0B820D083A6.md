﻿---
title: SearchFilterHost.exe | Microsoft Windows Search Filter Host
---

# SearchFilterHost.exe 

* File Path: `C:\Windows\system32\SearchFilterHost.exe`
* Description: Microsoft Windows Search Filter Host

## Hashes

Type | Hash
-- | --
MD5 | `673511D54A34319446EAD0B820D083A6`
SHA1 | `C36BA6DB46DD7EB6F90B83B9ABF4D28CA99BFDFB`
SHA256 | `3596CE0D573803E261B0186D986842CB3CA80D40B65392310D13A7557F71C0A5`
SHA384 | `0564E35F5E8D54F8E02532AB5E978ADB807FB051E984D2A9AFF41909BF87900EB1C9E45C03050057AF62AA34E84678C8`
SHA512 | `AD260ECE4D32370A7FAA99973C48B2CE596A39CBACF34EF5DFED752C6F0FA589CE3951F7D0450A4FCFD9E66FA96E16C18F50EAAFE176D65F52E63DAC668F778C`
SSDEEP | `6144:SKbiiKNIy0CXzBNtd2sVi9AUrkR10efUK:SA1KNIytXzBNtTVi9AUQztf`

## Signature

* Status: Signature verified.
* Serial: `3300000266BD1580EFA75CD6D3000000000266`
* Thumbprint: `A4341B9FD50FB9964283220A36A1EF6F6FAA7840`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: SearchFilterHost.exe
* Product Name: Windows Search
* Company Name: Microsoft Corporation
* File Version: 7.0.19041.329 (WinBuild.160101.0800)
* Product Version: 7.0.19041.329
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.

## File Similarity (ssdeep match)

File | Score
-- | --
[C:\WINDOWS\system32\SearchFilterHost.exe](SearchFilterHost.exe-2296B4F9F71EFB1FCC195C85B8EA3ED9.md) | 41
[C:\Windows\system32\SearchFilterHost.exe](SearchFilterHost.exe-32070FD581B3C13740432169F764F066.md) | 38
[C:\Windows\system32\SearchFilterHost.exe](SearchFilterHost.exe-334E8E996B23216667D9538CE40D68B5.md) | 41
[C:\WINDOWS\system32\SearchProtocolHost.exe](SearchProtocolHost.exe-2EF0A0531B2566153D9A3DF4160F650B.md) | 35
[C:\Windows\system32\SearchProtocolHost.exe](SearchProtocolHost.exe-9350D231BEDC8A957F8CAA50E83BC446.md) | 32
[C:\Windows\system32\SearchProtocolHost.exe](SearchProtocolHost.exe-C4D33CE329ADDA42557420034702BDB4.md) | 30
[C:\Windows\SysWOW64\SearchFilterHost.exe](SearchFilterHost.exe-09C9EB6892E603CD4265920E5A29F7CD.md) | 38
[C:\Windows\SysWOW64\SearchFilterHost.exe](SearchFilterHost.exe-98CAC0FEB32500C7CC15B6FE83F6068D.md) | 43
[C:\WINDOWS\SysWOW64\SearchFilterHost.exe](SearchFilterHost.exe-BDCF47F408DA7D42D97763D27405B773.md) | 40
[C:\Windows\SysWOW64\SearchFilterHost.exe](SearchFilterHost.exe-D332D4C07B7289696EE7EE8D656100B0.md) | 36
[C:\Windows\SysWOW64\SearchProtocolHost.exe](SearchProtocolHost.exe-3F2C5E10BCC7A67751F042FE148C1B0F.md) | 38
[C:\WINDOWS\SysWOW64\SearchProtocolHost.exe](SearchProtocolHost.exe-E318AF6C41ABF3FB889EC89164A36A37.md) | 32
[C:\Windows\SysWOW64\SearchProtocolHost.exe](SearchProtocolHost.exe-E503AEEC8FA45CF5A5B530E41B7E1156.md) | 29
[C:\Windows\SysWOW64\SearchProtocolHost.exe](SearchProtocolHost.exe-EDDF12939FEF7AE88C2C2DA5B12E90B2.md) | 30

## Possible Misuse

*The following table contains possible examples of `SearchFilterHost.exe` being misused. While `SearchFilterHost.exe` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[sigma](https://github.com/Neo23x0/sigma) | [win_apt_winnti_mal_hk_jan20.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_apt_winnti_mal_hk_jan20.yml) | `        Image\|endswith: '\SearchFilterHost.exe'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)



MIT License. Copyright (c) 2020 Strontic.


