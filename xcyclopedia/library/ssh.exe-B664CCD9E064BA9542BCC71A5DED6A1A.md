﻿---
title: ssh.exe | 
---

# ssh.exe 

* File Path: `C:\Windows\system32\OpenSSH\ssh.exe`

## Hashes

Type | Hash
-- | --
MD5 | `B664CCD9E064BA9542BCC71A5DED6A1A`
SHA1 | `1B4ED1E4E6D3F8EFFB0F119056D5B06342D80524`
SHA256 | `0C0E91427A4B0E4CD0B59BDB73054252FB74C0977D13A73AB7423E15528B0485`
SHA384 | `42EEC84E4B8A61A116E58DF421559EC5E9B639F17B7202634E8501DCC6D1604764446A5F7655F6AB5046CD5CEDF48AE2`
SHA512 | `7EB6A9ACB61D964C82C46E897F8A5195C7F06BEDF7F1ECD2D64F2783BE996F7A6356E9C991DA4BBE541F4E8A214B7D58DC9AF17652E448CE582BBFA2946690AB`
SSDEEP | `24576:QTDSQPwMHspFKajxUAn0/2L50P6DlZC2u:eSMYFKaT70P6DlZC`

## Runtime Data

### Usage (stderr):
```Batchfile
unknown option -- h
usage: ssh [-46AaCfGgKkMNnqsTtVvXxYy] [-B bind_interface]
           [-b bind_address] [-c cipher_spec] [-D [bind_address:]port]
           [-E log_file] [-e escape_char] [-F configfile] [-I pkcs11]
           [-i identity_file] [-J [user@]host[:port]] [-L address]
           [-l login_name] [-m mac_spec] [-O ctl_cmd] [-o option] [-p port]
           [-Q query_option] [-R address] [-S ctl_path] [-W host:port]
           [-w local_tun[:remote_tun]] destination [command]

```

### Child Processes:
conhost.exe

## Signature

* Status: Signature verified.
* Serial: `330000023241FB59996DCC4DFF000000000232`
* Thumbprint: `FF82BC38E1DA5E596DF374C53E3617F7EDA36B06`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: 
* Product Name: OpenSSH for Windows
* Company Name: 
* File Version: 7.7.2.1
* Product Version: OpenSSH_7.7p1 for Windows
* Language: English (United States)
* Legal Copyright: 


## Possible Misuse

*The following table contains possible examples of `ssh.exe` being misused. While `ssh.exe` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[sigma](https://github.com/Neo23x0/sigma) | [win_multiple_suspicious_cli.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_multiple_suspicious_cli.yml) | `            - ssh.exe` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)



MIT License. Copyright (c) 2020 Strontic.


