﻿---
title: nslookup.exe | nslookup
---

# nslookup.exe 

* File Path: `C:\Windows\system32\nslookup.exe`
* Description: nslookup

## Hashes

Type | Hash
-- | --
MD5 | `F2E3950C1023ACF80765C918791999C0`
SHA1 | `953726ECD156848921609201C97C51A50C0CF36C`
SHA256 | `55AB032D256ADBE3FDE40CF90FE83BA5EAB591E04AD720161ED8E6EF059CA747`
SHA384 | `4C9045F57205E36144FE02170E342186F7C66AF313F755179A138950248F8F9870A63D01EF561EAF26CFB01B95855FF3`
SHA512 | `BAA7FB2385BD82D9A6A0A92FC41E2D26122154AA47199FE3AA9030FCAB1BF12D6B926AA27957B1F6E33A3FAF41B2B9F6B655104CB337928FF95BBF45D1A93E6E`
SSDEEP | `1536:Ono+AIqFL2Gl26Uk+n4vAyl4Ds6blmRbxOcxm:OnnAI3GJ+A5Kg6Re7m`

## Runtime Data

### Usage (stdout):
```Batchfile
Default Server:  default-pc.mshome.net
Address:  172.16.1.1

> 
```

### Usage (stderr):
```Batchfile
Usage:
   nslookup [-opt ...]             # interactive mode using default server
   nslookup [-opt ...] - server    # interactive mode using 'server'
   nslookup [-opt ...] host        # just look up 'host' using default server
   nslookup [-opt ...] host server # just look up 'host' using 'server'

```

### Child Processes:
conhost.exe

## Signature

* Status: Signature verified.
* Serial: `330000026551AE1BBD005CBFBD000000000265`
* Thumbprint: `E168609353F30FF2373157B4EB8CD519D07A2BFF`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: nslookup.exe.mui
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.19041.1 (WinBuild.160101.0800)
* Product Version: 10.0.19041.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.


## Possible Misuse

*The following table contains possible examples of `nslookup.exe` being misused. While `nslookup.exe` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[sigma](https://github.com/Neo23x0/sigma) | [apt_silence_eda.yml](https://github.com/Neo23x0/sigma/blob/master/rules/apt/apt_silence_eda.yml) | `            - '$Command \| nslookup 2>&1 \| Out-String'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_apt_chafer_mar18.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_apt_chafer_mar18.yml) | `        CommandLine: '*\nslookup.exe -q=TXT*'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_multiple_suspicious_cli.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_multiple_suspicious_cli.yml) | `            - nslookup.exe` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_shell_spawn_susp_program.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_shell_spawn_susp_program.yml) | `            - '*\nslookup.exe'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_susp_commands_recon_activity.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_susp_commands_recon_activity.yml) | `            - nslookup` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_susp_execution_path_webserver.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_susp_execution_path_webserver.yml) | `    - Tools that include ping or nslookup command invocations` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[atomic-red-team](https://github.com/redcanaryco/atomic-red-team) | [index.md](https://github.com/redcanaryco/atomic-red-team/blob/master/atomics/Indexes/Indexes-Markdown/index.md) |   - Atomic Test #8: Remote System Discovery - nslookup [windows] | [MIT License. © 2018 Red Canary](https://github.com/redcanaryco/atomic-red-team/blob/master/LICENSE.txt)
[atomic-red-team](https://github.com/redcanaryco/atomic-red-team) | [windows-index.md](https://github.com/redcanaryco/atomic-red-team/blob/master/atomics/Indexes/Indexes-Markdown/windows-index.md) |   - Atomic Test #8: Remote System Discovery - nslookup [windows] | [MIT License. © 2018 Red Canary](https://github.com/redcanaryco/atomic-red-team/blob/master/LICENSE.txt)
[atomic-red-team](https://github.com/redcanaryco/atomic-red-team) | [T1018.md](https://github.com/redcanaryco/atomic-red-team/blob/master/atomics/T1018/T1018.md) | - [Atomic Test #8 - Remote System Discovery - nslookup](#atomic-test-8---remote-system-discovery---nslookup) | [MIT License. © 2018 Red Canary](https://github.com/redcanaryco/atomic-red-team/blob/master/LICENSE.txt)
[atomic-red-team](https://github.com/redcanaryco/atomic-red-team) | [T1018.md](https://github.com/redcanaryco/atomic-red-team/blob/master/atomics/T1018/T1018.md) | ## Atomic Test #8 - Remote System Discovery - nslookup | [MIT License. © 2018 Red Canary](https://github.com/redcanaryco/atomic-red-team/blob/master/LICENSE.txt)
[atomic-red-team](https://github.com/redcanaryco/atomic-red-team) | [T1018.md](https://github.com/redcanaryco/atomic-red-team/blob/master/atomics/T1018/T1018.md) | Powershell script that runs nslookup on cmd.exe against the local /24 network of the first network adaptor listed in ipconfig. | [MIT License. © 2018 Red Canary](https://github.com/redcanaryco/atomic-red-team/blob/master/LICENSE.txt)
[atomic-red-team](https://github.com/redcanaryco/atomic-red-team) | [T1018.md](https://github.com/redcanaryco/atomic-red-team/blob/master/atomics/T1018/T1018.md) | Upon successful execution, powershell will identify the ip range (via ipconfig) and perform a for loop and execute nslookup against that IP range. Output will be via stdout. | [MIT License. © 2018 Red Canary](https://github.com/redcanaryco/atomic-red-team/blob/master/LICENSE.txt)
[atomic-red-team](https://github.com/redcanaryco/atomic-red-team) | [T1018.md](https://github.com/redcanaryco/atomic-red-team/blob/master/atomics/T1018/T1018.md) | foreach ($ip in 1..255 \| % { "$firstOctet.$secondOctet.$thirdOctet.$_" } ) {cmd.exe /c nslookup $ip} | [MIT License. © 2018 Red Canary](https://github.com/redcanaryco/atomic-red-team/blob/master/LICENSE.txt)
[signature-base](https://github.com/Neo23x0/signature-base) | [apt_laudanum_webshells.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/apt_laudanum_webshells.yar) | 		$s1 = "command = \"nslookup -type=\" & qtype & \" \" & query " fullword ascii /* PEStudio Blacklist: strings */ | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)
[signature-base](https://github.com/Neo23x0/signature-base) | [gen_suspicious_strings.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/gen_suspicious_strings.yar) |       $ = "nslookup" | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)

## Additional Info*

**The information below is copied from [MicrosoftDocs](https://github.com/MicrosoftDocs/windowsserverdocs), which is maintained by [Microsoft](https://opensource.microsoft.com/codeofconduct/). Available under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.*

---

## nslookup

> Applies to: Windows Server (Semi-Annual Channel), Windows Server 2019, Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

Displays information that you can use to diagnose Domain Name System (DNS) infrastructure. Before using this tool, you should be familiar with how DNS works. The nslookup command-line tool is available only if you have installed the TCP/IP protocol.

The nslookup command-line tool has two modes: interactive and noninteractive.

If you need to look up only a single piece of data, we recommend using the non-interactive mode. For the first parameter, type the name or IP address of the computer that you want to look up. For the second parameter, type the name or IP address of a DNS name server. If you omit the second argument, **nslookup** uses the default DNS name server.

If you need to look up more than one piece of data, you can use interactive mode. Type a hyphen (-) for the first parameter and the name or IP address of a DNS name server for the second parameter. If you omit both parameters, the tool uses the default DNS name server. While using the interactive mode, you can:

- Interrupt interactive commands at any time, by pressing CTRL+B.

- Exit, by typing **exit**.

- Treat a built-in command as a computer name, by preceding it with the escape character (\). An unrecognized command is interpreted as a computer name.

### Syntax

```
nslookup [exit | finger | help | ls | lserver | root | server | set | view] [options]
```

#### Parameters

| Parameter | Description |
| --------- | ----------- |
| [nslookup exit](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-exit-command.md) | Exits the nslookup command-line tool. |
| [nslookup finger](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-finger-command.md) | Connects with the finger server on the current computer. |
| [nslookup help](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-help.md) | Displays a short summary of subcommands. |
| [nslookup ls](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-ls.md) | Lists information for a DNS domain. |
| [nslookup lserver](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-lserver.md) | Changes the default server to the specified DNS domain. |
| [nslookup root](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-root.md) | Changes the default server to the server for the root of the DNS domain name space. |
| [nslookup server](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-server.md) | Changes the default server to the specified DNS domain. |
| [nslookup set](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set.md) | Changes configuration settings that affect how lookups function. |
| [nslookup set all](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-all.md) | Prints the current values of the configuration settings. |
| [nslookup set class](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-class.md) | Changes the query class. The class specifies the protocol group of the information. |
| [nslookup set d2](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-d2.md) | Turns exhaustive Debugging mode on or off. All fields of every packet are printed. |
| [nslookup set debug](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-debug.md) | Turns Debugging mode on or off. |
| [nslookup set domain](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-domain.md) | Changes the default DNS domain name to the name specified. |
| [nslookup set port](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-port.md) | Changes the default TCP/UDP DNS name server port to the value specified. |
| [nslookup set querytype](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-querytype.md) | Changes the resource record type for the query. |
| [nslookup set recurse](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-recurse.md) | Tells the DNS name server to query other servers if it doesn't have the information. |
| [nslookup set retry](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-retry.md) | Sets the number of retries. |
| [nslookup set root](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-root.md) | Changes the name of the root server used for queries. |
| [nslookup set search](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-search.md) | Appends the DNS domain names in the DNS domain search list to the request until an answer is received. This applies when the set and the lookup request contain at least one period, but do not end with a trailing period. |
| [nslookup set srchlist](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-srchlist.md) | Changes the default DNS domain name and search list. |
| [nslookup set timeout](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-timeout.md) | Changes the initial number of seconds to wait for a reply to a request. |
| [nslookup set type](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-type.md) | Changes the resource record type for the query. |
| [nslookup set vc](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-vc.md) | Specifies to use or not use a virtual circuit when sending requests to the server. |
| [nslookup view](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-view.md) | Sorts and lists the output of the previous **ls** subcommand or commands. |

#### Remarks

- If *computerTofind* is an IP address and the query is for an **A** or **PTR** resource record type, the name of the computer is returned.

- If *computerTofind* is a name and doesn't have a trailing period, the default DNS domain name is appended to the name. This behavior depends on the state of the following **set** subcommands: **domain**, **srchlist**, **defname**, and **search**.

- If you type a hyphen (-) instead of *computerTofind*, the command prompt changes to **nslookup** interactive mode.

- If the lookup request fails, the command-line tool provides an error message, including:

  | Error message | Description |
  | ------------- | ----------- |
  | timed out |The server didn't respond to a request after a certain amount of time and a certain number of retries. You can set the time-out period with the [nslookup set timeout](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-timeout.md) command. You can set the number of retries with the [nslookup set retry](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-retry.md) command. |
  | No response from server | No DNS name server is running on the server computer. |
  | No records | The DNS name server doesn't have resource records of the current query type for the computer, although the computer name is valid. The query type is specified with the [nslookup set querytype](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/nslookup-set-querytype.md) command. |
  | Nonexistent domain | The computer or DNS domain name doesn't exist. |
  | Connection refused or Network is unreachable | The connection to the DNS name server or finger server could not be made. This error commonly occurs with the **ls** and **finger** requests. |
  | Server failure | The DNS name server found an internal inconsistency in its database and could not return a valid answer. |
  | Refused | The DNS name server refused to service the request. |
  | format error | The DNS name server found that the request packet was not in the proper format. It may indicate an error in **nslookup**. |

### Additional References

- [Command-Line Syntax Key](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/command-line-syntax-key.md)

---



MIT License. Copyright (c) 2020 Strontic.


