﻿---
title: ntoskrnl.exe | NT Kernel & System
---

# ntoskrnl.exe 

* File Path: `C:\WINDOWS\system32\ntoskrnl.exe`
* Description: NT Kernel & System

## Hashes

Type | Hash
-- | --
MD5 | `E876B427E3F116CC37EA3BA758FCB00D`
SHA1 | `AEB320E8897708BC7A808C1A369038DC463DDC2D`
SHA256 | `CCCFDA078A89D2ADB3BD6E93F30A031B24FD37FBF2CAF3D2A6BB39F2E790D13B`
SHA384 | `55E261C9BFAD147957B90FEBB2F854DD390FCCF30694AEFB5652C4C3F55FBDE51C8EBD4BA9B44D0A3631D684E5D189ED`
SHA512 | `1D240FD30158A7E919345FD214266DC212CFA84200941061B33C291691AD1DCC0A9F450D9BA00A168A5A3163F0F7FBFA1AC08BAB1DFE3B10E88D3022537841F9`
SSDEEP | `98304:DO8HiadPoQXojOqRg+iaoyYEA0oa8xNOu7nNI8JijYkPcZ:7xBiBRgyfYw8fOu7nvUjYkPcZ`

## Signature

* Status: Signature verified.
* Serial: `3300000266BD1580EFA75CD6D3000000000266`
* Thumbprint: `A4341B9FD50FB9964283220A36A1EF6F6FAA7840`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: ntkrnlmp.exe
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.18362.836 (WinBuild.160101.0800)
* Product Version: 10.0.18362.836
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.


## Possible Misuse

*The following table contains possible examples of `ntoskrnl.exe` being misused. While `ntoskrnl.exe` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[signature-base](https://github.com/Neo23x0/signature-base) | [apt_hackingteam_rules.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/apt_hackingteam_rules.yar) | 		$x4 = "C:\\\\Windows\\\\Sysnative\\\\ntoskrnl.exe" fullword ascii /* PEStudio Blacklist: strings */ | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)
[signature-base](https://github.com/Neo23x0/signature-base) | [apt_winnti.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/apt_winnti.yar) | 		$s17 = "NTOSKRNL.EXE" fullword wide /* Goodware String - occured 4 times */ | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)
[signature-base](https://github.com/Neo23x0/signature-base) | [apt_winnti.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/apt_winnti.yar) |       $a5 = "ntoskrnl.exe" ascii fullword | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)
[signature-base](https://github.com/Neo23x0/signature-base) | [apt_winnti.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/apt_winnti.yar) |       $a3 = "%SystemRoot%\\System32\\ntoskrnl.exe" ascii | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)
[signature-base](https://github.com/Neo23x0/signature-base) | [apt_winnti_hdroot.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/apt_winnti_hdroot.yar) |       $s1 = "\\system32\\ntoskrnl.exe" fullword ascii | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)
[signature-base](https://github.com/Neo23x0/signature-base) | [spy_querty_fiveeyes.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/spy_querty_fiveeyes.yar) | 		$s3 = "ntoskrnl.exe" fullword ascii | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)
[signature-base](https://github.com/Neo23x0/signature-base) | [spy_regin_fiveeyes.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/spy_regin_fiveeyes.yar) | 		$s4 = "ntoskrnl.exe" fullword ascii | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)



MIT License. Copyright (c) 2020 Strontic.


