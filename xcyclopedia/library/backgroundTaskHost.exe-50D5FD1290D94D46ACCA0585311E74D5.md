﻿---
title: backgroundTaskHost.exe | Background Task Host
---

# backgroundTaskHost.exe 

* File Path: `C:\windows\system32\backgroundTaskHost.exe`
* Description: Background Task Host

## Hashes

Type | Hash
-- | --
MD5 | `50D5FD1290D94D46ACCA0585311E74D5`
SHA1 | `339E4E69D2120B97CE34B9A8D3597FF8E0A73561`
SHA256 | `B8E176FE76A1454A00C4AF0F8BF8870650D9C33D3E333239A59445C5B35C9A37`
SHA384 | `652E1102EDEB000B95F54DDC85BE8C4D7E92001F17AB8E8F6CF0021F0F6EFF087626F40B1C1C357C35E4FF141FA62700`
SHA512 | `A89427027064F3B60948F6CD89D467A9E54A6947B8C73E73F9A252E1608CBA1A144DA77C47D5E36BD991649D878772934D93007A4B8A2AF005A39837851635D6`
SSDEEP | `384:H1dPOeFIR79Mjs0HijWFGWCmXjDBRJWrKudlZp06:PPO6tHimrXj1PWrTzB`

## Signature

* Status: Signature verified.
* Serial: `33000001C422B2F79B793DACB20000000001C4`
* Thumbprint: `AE9C1AE54763822EEC42474983D8B635116C8452`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: backgroundTaskHost.exe
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.17763.1 (WinBuild.160101.0800)
* Product Version: 10.0.17763.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.

## File Similarity (ssdeep match)

File | Score
-- | --
[C:\WINDOWS\system32\backgroundTaskHost.exe](backgroundTaskHost.exe-E22E7BD6B146BDE93DC48643B772D8BB.md) | 35
[C:\Windows\system32\browser_broker.exe](browser_broker.exe-C7C56DB13D5F1A2BB6DE92B8BBD22CA0.md) | 35
[C:\WINDOWS\system32\dllhost.exe](dllhost.exe-680045579134D8AD9D0400A9DBE30786.md) | 33
[C:\Windows\system32\dllhost.exe](dllhost.exe-D2AB39EA2C0FCD172751F84BDA723A97.md) | 36
[C:\Windows\system32\oobe\FirstLogonAnim.exe](FirstLogonAnim.exe-6DD5ECC82E9118B2DE1CAE3B35550E14.md) | 32
[C:\WINDOWS\system32\oobe\FirstLogonAnim.exe](FirstLogonAnim.exe-94C10EAE7738DA6F112A6407E8C952F8.md) | 30
[C:\Windows\system32\prproc.exe](prproc.exe-7ABD17EE7B6B0F79CD4D2F3D4B4B11C2.md) | 33
[C:\WINDOWS\system32\prproc.exe](prproc.exe-BFD6335E4F61D44CA74B627A45686106.md) | 29
[C:\Windows\system32\ScriptRunner.exe](ScriptRunner.exe-71B9062F02950BAA4441E2FB79677E99.md) | 35
[C:\Windows\system32\SlideToShutDown.exe](SlideToShutDown.exe-2CE65A4F9A63402F38537BE59FA1689D.md) | 33
[C:\WINDOWS\system32\SlideToShutDown.exe](SlideToShutDown.exe-C428A6CE6F4424BF148AF087C0BF4B75.md) | 32
[C:\WINDOWS\SysWOW64\backgroundTaskHost.exe](backgroundTaskHost.exe-DD15DCECF4B1EF67B89FA0B603C7D413.md) | 40
[C:\Windows\SysWOW64\backgroundTaskHost.exe](backgroundTaskHost.exe-F8D636BD68156F0C653DBC3D69FC0F08.md) | 46
[C:\Windows\SysWOW64\CameraSettingsUIHost.exe](CameraSettingsUIHost.exe-443AFE0E4385A46CFE2AD14890DC1FD4.md) | 27
[C:\WINDOWS\SysWOW64\CameraSettingsUIHost.exe](CameraSettingsUIHost.exe-8E0D0D53CA176DDA94850F7A3B406408.md) | 33
[C:\WINDOWS\SysWOW64\dllhost.exe](dllhost.exe-60D0B50CFF3A0722ADC274F49FB16F14.md) | 33
[C:\Windows\SysWOW64\dllhost.exe](dllhost.exe-B5A6D2FB3F4521C37D613DE52AB3467D.md) | 35

## Possible Misuse

*The following table contains possible examples of `backgroundTaskHost.exe` being misused. While `backgroundTaskHost.exe` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[sigma](https://github.com/Neo23x0/sigma) | [sysmon_abusing_azure_browser_sso.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/sysmon/sysmon_abusing_azure_browser_sso.yml) | `         - BackgroundTaskHost.exe` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)



MIT License. Copyright (c) 2020 Strontic.

