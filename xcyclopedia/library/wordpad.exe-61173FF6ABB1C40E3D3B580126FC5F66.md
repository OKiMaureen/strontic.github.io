﻿---
title: wordpad.exe | Windows Wordpad Application
---

# wordpad.exe 

* File Path: `C:\Program Files (x86)\Windows NT\Accessories\wordpad.exe`
* Description: Windows Wordpad Application

## Screenshot

![wordpad.exe](screenshots/wordpad.exe-34B557ACE63A6AF3EC4B02B4A9EC46AF-1.png)

## Hashes

Type | Hash
-- | --
MD5 | `61173FF6ABB1C40E3D3B580126FC5F66`
SHA1 | `C017E91A526DFBB37293CD79D86A1D7261ED0141`
SHA256 | `09F10E7344CA61B53A080E4D54C7CB6ECD4E3308254B350906437E29E7A7D9B2`
SHA384 | `0A8951333DEA88F9EF4CAD098E8B502420F7F074EBECC14A10878F43092F0A6C5AE77CBC3C17815EFC76B6CE5CB0A1AE`
SHA512 | `C5C8D5AD867987D18F88EF7D88E86E9A8DE13185F17F2E722409816D83147152ADB87EAB4A88E6327CBB1BD60D0223BBFE8689D54F747438BC66DD93C76CD9DA`
SSDEEP | `24576:pxHn7MgYE6WM73vT62FxvNEYr8oSUGeP9PDkjjqX+l:pxH7MgYE67BxvWCXSZeP9PDk37l`

## Runtime Data

### Child Processes:
splwow64.exe

## Signature

* Status: Signature verified.
* Serial: `330000023241FB59996DCC4DFF000000000232`
* Thumbprint: `FF82BC38E1DA5E596DF374C53E3617F7EDA36B06`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: WORDPAD.EXE.MUI
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.19041.1 (WinBuild.160101.0800)
* Product Version: 10.0.19041.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.

## File Similarity (ssdeep match)

File | Score
-- | --
[C:\Program Files\Windows NT\Accessories\wordpad.exe](wordpad.exe-34B557ACE63A6AF3EC4B02B4A9EC46AF.md) | 60

## Possible Misuse

*The following table contains possible examples of `wordpad.exe` being misused. While `wordpad.exe` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[signature-base](https://github.com/Neo23x0/signature-base) | [apt_winnti_burning_umbrella.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/apt_winnti_burning_umbrella.yar) |       $s1 = "Wordpad.Document.1\\shell\\open\\command\\" fullword wide | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)
[signature-base](https://github.com/Neo23x0/signature-base) | [thor-hacktools.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/thor-hacktools.yar) |       $s3 = "Accessories\\wordpad.exe" fullword ascii | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)



MIT License. Copyright (c) 2020 Strontic.


