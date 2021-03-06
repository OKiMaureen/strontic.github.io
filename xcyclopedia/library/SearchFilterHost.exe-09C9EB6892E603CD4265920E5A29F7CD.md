﻿---
title: SearchFilterHost.exe | Microsoft Windows Search Filter Host
---

# SearchFilterHost.exe 

* File Path: `C:\windows\SysWOW64\SearchFilterHost.exe`
* Description: Microsoft Windows Search Filter Host

## Hashes

Type | Hash
-- | --
MD5 | `09C9EB6892E603CD4265920E5A29F7CD`
SHA1 | `6884B7744572DC42301CF23EF36C3945DEB33701`
SHA256 | `BFEB65FEAFE356A44F6CC24D1962317C772ABC58A847A200F93C5DB69C93E98B`
SHA384 | `BD3C8EFC23081BDE652918B6894018E97C23D7646E5CF9EBE943F94BF901449435C384C2239CBAA7D2E3A740F16BB373`
SHA512 | `FCA6E6BD3B4A3B2CE3C7BAC569B0D48EF4FBBB6879A3FBDF8ED5D2C9DFCD37D7EFFA4A113A47BE5FB82C19E7C1DCFBE05C9A1806588AD1CC5125F0EDE6289504`
SSDEEP | `6144:coazi+tA/bnO7ttZnrdwGrkR10efUKVyg:coYiCADnmZdwGQztfjz`

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
* File Version: 7.0.17763.1098 (WinBuild.160101.0800)
* Product Version: 7.0.17763.1098
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.

## File Similarity (ssdeep match)

File | Score
-- | --
[C:\WINDOWS\system32\SearchFilterHost.exe](SearchFilterHost.exe-2296B4F9F71EFB1FCC195C85B8EA3ED9.md) | 41
[C:\Windows\system32\SearchFilterHost.exe](SearchFilterHost.exe-32070FD581B3C13740432169F764F066.md) | 38
[C:\Windows\system32\SearchFilterHost.exe](SearchFilterHost.exe-334E8E996B23216667D9538CE40D68B5.md) | 41
[C:\Windows\system32\SearchFilterHost.exe](SearchFilterHost.exe-673511D54A34319446EAD0B820D083A6.md) | 38
[C:\WINDOWS\system32\SearchProtocolHost.exe](SearchProtocolHost.exe-2EF0A0531B2566153D9A3DF4160F650B.md) | 36
[C:\Windows\system32\SearchProtocolHost.exe](SearchProtocolHost.exe-9350D231BEDC8A957F8CAA50E83BC446.md) | 33
[C:\Windows\system32\SearchProtocolHost.exe](SearchProtocolHost.exe-C4D33CE329ADDA42557420034702BDB4.md) | 30
[C:\Windows\SysWOW64\SearchFilterHost.exe](SearchFilterHost.exe-98CAC0FEB32500C7CC15B6FE83F6068D.md) | 49
[C:\WINDOWS\SysWOW64\SearchFilterHost.exe](SearchFilterHost.exe-BDCF47F408DA7D42D97763D27405B773.md) | 43
[C:\Windows\SysWOW64\SearchFilterHost.exe](SearchFilterHost.exe-D332D4C07B7289696EE7EE8D656100B0.md) | 40
[C:\Windows\SysWOW64\SearchProtocolHost.exe](SearchProtocolHost.exe-3F2C5E10BCC7A67751F042FE148C1B0F.md) | 38
[C:\WINDOWS\SysWOW64\SearchProtocolHost.exe](SearchProtocolHost.exe-E318AF6C41ABF3FB889EC89164A36A37.md) | 35
[C:\Windows\SysWOW64\SearchProtocolHost.exe](SearchProtocolHost.exe-E503AEEC8FA45CF5A5B530E41B7E1156.md) | 33
[C:\Windows\SysWOW64\SearchProtocolHost.exe](SearchProtocolHost.exe-EDDF12939FEF7AE88C2C2DA5B12E90B2.md) | 29

## Possible Misuse

*The following table contains possible examples of `SearchFilterHost.exe` being misused. While `SearchFilterHost.exe` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[sigma](https://github.com/Neo23x0/sigma) | [win_apt_winnti_mal_hk_jan20.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_apt_winnti_mal_hk_jan20.yml) | `        Image\|endswith: '\SearchFilterHost.exe'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)



MIT License. Copyright (c) 2020 Strontic.


