﻿---
title: TRACERT.EXE | TCP/IP Traceroute Command
---

# TRACERT.EXE 

* File Path: `C:\windows\system32\TRACERT.EXE`
* Description: TCP/IP Traceroute Command

## Hashes

Type | Hash
-- | --
MD5 | `FE01242CC5414473B0BF3A09D4216D3D`
SHA1 | `6D8D0CE1EB068D30D88376DA5D5E1B133F5D8390`
SHA256 | `A7A0CB3A7867D8CE594DAEBFC7571EB5CD59BE321D4D45296BE378EFE66109A2`
SHA384 | `A858F6A9E9B1428FEF4642673BADB6A86474AED39CA75CA47486BC226F0EBD61296E42094269FA71D8EA2F208B9BEC3B`
SHA512 | `70C253534FD51F0281CE9A58C6EA90B7FF5ADA6A0A22DCF95488E397B9F9C335EF632ECF037A5805C1BEADE529975CDD74D23EEADDF956D70494C451DF9175B9`
SSDEEP | `384:NYdbSRXUC+tQnnmoTRw3lYs9Q7aQMlmZL1ysWWlaW:NXj+mnu3Y6QZL1f`

## Runtime Data

### Usage (stdout):
```Batchfile

Usage: tracert [-d] [-h maximum_hops] [-j host-list] [-w timeout] 
               [-R] [-S srcaddr] [-4] [-6] target_name

Options:
    -d                 Do not resolve addresses to hostnames.
    -h maximum_hops    Maximum number of hops to search for target.
    -j host-list       Loose source route along host-list (IPv4-only).
    -w timeout         Wait timeout milliseconds for each reply.
    -R                 Trace round-trip path (IPv6-only).
    -S srcaddr         Source address to use (IPv6-only).
    -4                 Force using IPv4.
    -6                 Force using IPv6.

```

### Child Processes:
conhost.exe

## Signature

* Status: Signature verified.
* Serial: `33000001C422B2F79B793DACB20000000001C4`
* Thumbprint: `AE9C1AE54763822EEC42474983D8B635116C8452`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: tracert.exe.mui
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.17763.1 (WinBuild.160101.0800)
* Product Version: 10.0.17763.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.


## Possible Misuse

*The following table contains possible examples of `TRACERT.EXE` being misused. While `TRACERT.EXE` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[sigma](https://github.com/Neo23x0/sigma) | [win_apt_turla_comrat_may20.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_apt_turla_comrat_may20.yml) | `            - 'tracert -h 10 yahoo.com'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_multiple_suspicious_cli.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_multiple_suspicious_cli.yml) | `            - tracert.exe` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)

## Additional Info*

**The information below is copied from [MicrosoftDocs](https://github.com/MicrosoftDocs/windowsserverdocs), which is maintained by [Microsoft](https://opensource.microsoft.com/codeofconduct/). Available under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.*

---

## tracert

> Applies to: Windows Server (Semi-Annual Channel), Windows Server 2019, Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

Determines the path taken to a destination by sending Internet Control Message Protocol (ICMP) echo Request or ICMPv6 messages to the destination with incrementally increasing time to Live (TTL) field values. The path displayed is the list of near/side router interfaces of the routers in the path between a source host and a destination. The near/side interface is the interface of the router that is closest to the sending host in the path. Used without parameters, tracert displays help.


### Syntax

```
tracert [/d] [/h <MaximumHops>] [/j <Hostlist>] [/w <timeout>] [/R] [/S <Srcaddr>] [/4][/6] <TargetName>
```

##### Parameters

|Parameter|Description|
|-------|--------|
|/d|Prevents **tracert** from attempting to resolve the IP addresses of intermediate routers to their names. This can speed up the display of **tracert** results.|
|/h \<MaximumHops>|Specifies the maximum number of hops in the path to search for the target (destination). The default is 30 hops.|
|/j \<Hostlist>|Specifies that echo Request messages use the Loose Source Route option in the IP header with the set of intermediate destinations specified in *Hostlist*. With loose source routing, successive intermediate destinations can be separated by one or multiple routers. The maximum number of addresses or names in the host list is 9. The *Hostlist* is a series of IP addresses (in dotted decimal notation) separated by spaces. Use this parameter only when tracing IPv4 addresses.|
|/w \<timeout>|Specifies the amount of time in milliseconds to wait for the ICMP time Exceeded or echo Reply message corresponding to a given echo Request message to be received. If not received within the time-out, an asterisk (*) is displayed. The default time-out is 4000 (4 seconds).|
|/R|Specifies that the IPv6 Routing extension header be used to send an echo Request message to the local host, using the destination as an intermediate destination and testing the reverse route.|
|/S \<Srcaddr>|Specifies the source address to use in the echo Request messages. Use this parameter only when tracing IPv6 addresses.|
|/4|Specifies that tracert.exe can use only IPv4 for this trace.|
|/6|Specifies that tracert.exe can use only IPv6 for this trace.|
|\<TargetName>|Specifies the destination, identified either by IP address or host name.|
|/?|Displays help at the command prompt.|

### Remarks

- This diagnostic tool determines the path taken to a destination by sending ICMP echo Request messages with varying time to Live (TTL) values to the destination. Each router along the path is required to decrement the TTL in an IP packet by at least 1 before forwarding it. Effectively, the TTL is a maximum link counter. When the TTL on a packet reaches 0, the router is expected to return an ICMP time Exceeded message to the source computer. tracert determines the path by sending the first echo Request message with a TTL of 1 and incrementing the TTL by 1 on each subsequent transmission until the target responds or the maximum number of hops is reached. The maximum number of hops is 30 by default and can be specified using the **/h** parameter. The path is determined by examining the ICMP time Exceeded messages returned by intermediate routers and the echo Reply message returned by the destination. However, some routers do not return time Exceeded messages for packets with expired TTL values and are invisible to the tracert command. In this case, a row of asterisks (*) is displayed for that hop.
- To trace a path and provide network latency and packet loss for each router and link in the path, use the [**pathping**](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/pathping.md) command.
- This command is available only if the Internet Protocol (TCP/IP) protocol is installed as a component in the properties of a network adapter in Network Connections.

### Examples

To trace the path to the host named corp7.microsoft.com, type:
```
tracert corp7.microsoft.com
```
To trace the path to the host named corp7.microsoft.com and prevent the resolution of each IP address to its name, type:
```
tracert /d corp7.microsoft.com
```
To trace the path to the host named corp7.microsoft.com and use the loose source route 10.12.0.1/10.29.3.1/10.1.44.1, type:
```
tracert /j 10.12.0.1 10.29.3.1 10.1.44.1 corp7.microsoft.com
```

### Additional References

- [Command-Line Syntax Key](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/command-line-syntax-key.md)

---



MIT License. Copyright (c) 2020 Strontic.


