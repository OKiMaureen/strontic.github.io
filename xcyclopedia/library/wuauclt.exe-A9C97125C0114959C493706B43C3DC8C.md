﻿---
title: wuauclt.exe | Windows Update
---

# wuauclt.exe 

* File Path: `C:\windows\system32\wuauclt.exe`
* Description: Windows Update

## Hashes

Type | Hash
-- | --
MD5 | `A9C97125C0114959C493706B43C3DC8C`
SHA1 | `9F02F926440E40F49A342EC4535F65BF422555ED`
SHA256 | `CC855323B6AB7259C92BD1310211DD95174E43BE2F46C828E38F0060DD2E4488`
SHA384 | `781CDC21628D2D9122352374AD52BEF0535D3EA22EA59E37490A9E3DA60C39A0DA2F71163261FD3E76FA389766AF8DF9`
SHA512 | `DA7A8004A3D5F643288CC19C0F8A14D4307E697FFA0D4034A392D75791714484D7EDA06B7165117B6E18DF6024CAF4CC0320B2774D744666148CFF2E94C51F6F`
SSDEEP | `768:ah2S//Mvy1sxCf1eQAqTE0OVJzOH/K4FVQcqj5fCuKAEXOaEnw1BulMWZqy4Z95h:6//Skra/ylerKD7gYlBRdV9pP`

## Signature

* Status: Signature verified.
* Serial: `3300000266BD1580EFA75CD6D3000000000266`
* Thumbprint: `A4341B9FD50FB9964283220A36A1EF6F6FAA7840`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: wuauclt.exe
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.17763.1 (WinBuild.160101.0800)
* Product Version: 10.0.17763.1
* Language: Language Neutral
* Legal Copyright:  Microsoft Corporation. All rights reserved.


## Possible Misuse

*The following table contains possible examples of `wuauclt.exe` being misused. While `wuauclt.exe` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[signature-base](https://github.com/Neo23x0/signature-base) | [apt_putterpanda.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/apt_putterpanda.yar) | 		$x0 = "WUAUCLT.EXE" fullword wide /* PEStudio Blacklist: strings */ /* score: '20.01' */ | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)



MIT License. Copyright (c) 2020 Strontic.


