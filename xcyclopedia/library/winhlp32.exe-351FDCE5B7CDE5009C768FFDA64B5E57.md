﻿---
title: winhlp32.exe | Windows Winhlp32 Stub
---

# winhlp32.exe 

* File Path: `C:\windows\winhlp32.exe`
* Description: Windows Winhlp32 Stub

## Hashes

Type | Hash
-- | --
MD5 | `351FDCE5B7CDE5009C768FFDA64B5E57`
SHA1 | `1FAB1E89A86956A2281EE8364774BE307D81F689`
SHA256 | `0AE37C1D7FC84E5E956874458508205F4DAD68D933BE6B801CFF2E42475664B5`
SHA384 | `11F3469FF4D36905BAE955F9E0E7E713198950F9F8A9E101DFC6750DC99689D607FA27E9AFFF95FEC7538BD658CD2821`
SHA512 | `71311CD7E0AD65C0B39AE1B8EA14E536E005090815527E2FA91811D238CFE33BB14DCBA34545F68D5A6BF7E8D7FD6255AE11425F7F318C014A360E2580029BF6`
SSDEEP | `192:PvR0uTw4mh2sKYHqWZxeqQ4t5tmXdkLWMeHWthh4jBrA:PiuTorHq8ZnCqLWMeHWthh49s`

## Signature

* Status: Signature verified.
* Serial: `33000001C422B2F79B793DACB20000000001C4`
* Thumbprint: `AE9C1AE54763822EEC42474983D8B635116C8452`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: WINHLP32.EXE.MUI
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.17763.1 (WinBuild.160101.0800)
* Product Version: 10.0.17763.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.

## File Similarity (ssdeep match)

File | Score
-- | --
[C:\WINDOWS\winhlp32.exe](winhlp32.exe-CAA192BFDFB5F2A131EBD649B7062DE3.md) | 63

## Possible Misuse

*The following table contains possible examples of `winhlp32.exe` being misused. While `winhlp32.exe` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[signature-base](https://github.com/Neo23x0/signature-base) | [apt_korplug_fast.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/apt_korplug_fast.yar) |         $s4 = "\\winhlp32.exe" fullword ascii | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)



MIT License. Copyright (c) 2020 Strontic.


