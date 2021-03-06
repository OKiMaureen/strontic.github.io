﻿---
title: wmplayer.exe | Windows Media Player
---

# wmplayer.exe 

* File Path: `C:\Program Files\Windows Media Player\wmplayer.exe`
* Description: Windows Media Player

## Hashes

Type | Hash
-- | --
MD5 | `D86F92A0D66CD72733ECA3BE2B1A412C`
SHA1 | `A351414AF7F811FC69256A30C8A0F107DBB7B060`
SHA256 | `AD4463F1737CE4BB445663515A0CB24A9EA50929E46BE81C803972D326FA7E10`
SHA384 | `855385FCCA868C6B2BA63CF8AE3F240F88CE9AF797B67C9CBE8B9C4B138B6360895BB85615F40D975048925F78C63AFD`
SHA512 | `74E6F327C8C394A1C120C63B3101802D76DC1565B485F3F6F9499E28093BFD9DC499A9A0175B02546F7F284B95ED13F7783A8425A9693E3AE05E8F03F2A71262`
SSDEEP | `3072:TIV3QSwKohYkQr0jeLwJr95rJolNAzyP+msVK0Zi:TIV3cYQqLwhHrWsOP+5VT`

## Runtime Data

### Child Processes:
setup_wm.exe

## Signature

* Status: Signature verified.
* Serial: `3300000266BD1580EFA75CD6D3000000000266`
* Thumbprint: `A4341B9FD50FB9964283220A36A1EF6F6FAA7840`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: wmplayer.exe.mui
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 12.0.19041.1 (WinBuild.160101.0800)
* Product Version: 12.0.19041.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.

## File Similarity (ssdeep match)

File | Score
-- | --
[C:\Program Files (x86)\Windows Media Player\wmpconfig.exe](wmpconfig.exe-4ACC57344531EEAC412463137996B8C1.md) | 60
[C:\Program Files (x86)\Windows Media Player\wmplayer.exe](wmplayer.exe-6AA4614C7ADE4C07F2F6E362D08DCF5A.md) | 88
[C:\Program Files (x86)\Windows Media Player\wmpshare.exe](wmpshare.exe-AA5933CE16373F146EC28DA42A0700B7.md) | 60
[C:\Program Files\Windows Media Player\wmpconfig.exe](wmpconfig.exe-29E52BFB44C74B2E3730F79D04082692.md) | 60
[C:\Program Files\Windows Media Player\wmpshare.exe](wmpshare.exe-275462C97656943B9F1A11F1701861FA.md) | 61

## Possible Misuse

*The following table contains possible examples of `wmplayer.exe` being misused. While `wmplayer.exe` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[sigma](https://github.com/Neo23x0/sigma) | [win_apt_winnti_mal_hk_jan20.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_apt_winnti_mal_hk_jan20.yml) | `        Image\|endswith: '\wmplayer.exe'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)



MIT License. Copyright (c) 2020 Strontic.


