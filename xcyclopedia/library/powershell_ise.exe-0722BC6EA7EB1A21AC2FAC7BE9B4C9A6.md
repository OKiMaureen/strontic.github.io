﻿---
title: powershell_ise.exe | Windows PowerShell ISE
---

# powershell_ise.exe 

* File Path: `C:\Windows\SysWOW64\WindowsPowerShell\v1.0\powershell_ise.exe`
* Description: Windows PowerShell ISE
* Comments: 

## Hashes

Type | Hash
-- | --
MD5 | `0722BC6EA7EB1A21AC2FAC7BE9B4C9A6`
SHA1 | `433001D7173D18F5B294CC2B6F5F1FB411843764`
SHA256 | `92A89AE883ED67889C50FA7AF84B1A94768C7A257DAA263211616D745D8DBDC3`
SHA384 | `5D90625927DB70C74525971AC1AFC2EBAC2E2CF97D004397DFDCAB856758F5AB527627EDE455E2EABAD872EE08B3C842`
SHA512 | `684EEC347F39D9135E856A827D6410C545CFB6E0F10A34E93785E975C958192C700B991A23A78817FBFDA14B4CD8FA2488D4F304B110CD3F46A22D1680E2B7C5`
SSDEEP | `3072:o9kVjGPsw40xLkVjqP4w6U+ToIuWNXmmZTWl/jC7gDooMLdx:0kauZToIuUXmmZbgDooMb`

## Runtime Data

### Usage (stdout):
```Batchfile

```

### Usage (stderr):
```Batchfile

```

### Child Processes:


## Signature

* Status: Signature verified.
* Serial: `330000023241FB59996DCC4DFF000000000232`
* Thumbprint: `FF82BC38E1DA5E596DF374C53E3617F7EDA36B06`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: powershell_ise.EXE
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.19041.1 (WinBuild.160101.0800)
* Product Version: 10.0.19041.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.

## File Similarity (ssdeep match)

File | Score
-- | --
[C:\WINDOWS\system32\WindowsPowerShell\v1.0\powershell_ise.exe](powershell_ise.exe-30A2792A2428CD06CFEC23ECB074889A.md) | 93
[C:\Windows\system32\WindowsPowerShell\v1.0\powershell_ise.exe](powershell_ise.exe-3F06E220C3E591F458D549B01ECCCB95.md) | 88
[C:\Windows\system32\WindowsPowerShell\v1.0\powershell_ise.exe](powershell_ise.exe-E05920670516CC96822699E5688A79FA.md) | 94
[C:\Windows\SysWOW64\WindowsPowerShell\v1.0\powershell_ise.exe](powershell_ise.exe-8F1F1C4EDA2CFA2073E82A409BBE35D0.md) | 90
[C:\WINDOWS\SysWOW64\WindowsPowerShell\v1.0\powershell_ise.exe](powershell_ise.exe-9F47663A5E104CD1EF4079CC37F12674.md) | 91

## Possible Misuse

*The following table contains possible examples of `powershell_ise.exe` being misused. While `powershell_ise.exe` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[sigma](https://github.com/Neo23x0/sigma) | [win_renamed_binary.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_renamed_binary.yml) | `            - 'powershell_ise.exe'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_renamed_binary.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_renamed_binary.yml) | `            - '\powershell_ise.exe'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_renamed_binary_highly_relevant.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_renamed_binary_highly_relevant.yml) | `            - "powershell_ise.exe"` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_renamed_binary_highly_relevant.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_renamed_binary_highly_relevant.yml) | `            - '*\powershell_ise.exe'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_renamed_powershell.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_renamed_powershell.yml) | `            - '*\powershell_ise.exe'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [sysmon_alternate_powershell_hosts_pipe.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/sysmon/sysmon_alternate_powershell_hosts_pipe.yml) | `            - '\powershell_ise.exe'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [sysmon_in_memory_powershell.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/sysmon/sysmon_in_memory_powershell.yml) | `            - '\powershell_ise.exe'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[atomic-red-team](https://github.com/redcanaryco/atomic-red-team) | [T1059.001.md](https://github.com/redcanaryco/atomic-red-team/blob/master/atomics/T1059.001/T1059.001.md) | 1. Open Powershell_ise as a Privileged Account | [MIT License. © 2018 Red Canary](https://github.com/redcanaryco/atomic-red-team/blob/master/LICENSE.txt)

## Additional Info*

**The information below is copied from [MicrosoftDocs](https://github.com/MicrosoftDocs/windowsserverdocs), which is maintained by [Microsoft](https://opensource.microsoft.com/codeofconduct/). Available under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.*

---

## PowerShell_ise



Windows PowerShell Integrated Scripting Environment (ISE) is a graphical host application that enables you to read, write, run, debug, and test scripts and modules in a graphic-assisted environment. Key features such as IntelliSense, Show-Command, snippets, tab completion, syntax-coloring, visual debugging, and context-sensitive Help provide a rich scripting experience.

The **PowerShell_ISE.exe** tool starts a Windows PowerShell ISE session. When you use **PowerShell_ISE.exe**, you can use its optional parameters to open files in Windows PowerShell ISE or to start a Windows PowerShell ISE session with no profile or with a multithreaded apartment.

**PowerShell_ISE.exe** was introduced in Windows PowerShell 2.0 and expanded significantly in Windows PowerShell 3.0.

### Using PowerShell_ISE.exe

You can use **PowerShell_ISE.exe** to start and end a Windows PowerShell session as follows:
- To start a Windows PowerShell ISE session, in a Command Prompt window, in Windows PowerShell, or at the Start menu, type:
  ```
  PowerShell_Ise
  ```
- To open a script (.ps1), script module (.psm1), module manifest (.psd1), XML file, or any other supported file in Windows PowerShell ISE, use the following command format:
  ```
  PowerShell_Ise <FilePath>
  ```
  In Windows PowerShell 3.0, you can use the optional **File** parameter as follows:
  ```
  PowerShell_Ise -File <FilePath>
  ```
- To start a Windows PowerShell ISE session without your Windows PowerShell profiles, use the **NoProfile** parameter. (The **NoProfile** parameter is introduced in Windows PowerShell 3.0.)
  ```
  PowerShell_Ise -NoProfile
  ```
- To see the **PowerShell_ISE.exe** Help file in a Command Prompt window, use the following command format:
  ```
  PowerShell_Ise -help, -?, /?
  ```
  For a complete list of the **PowerShell_ISE.exe** command-line parameters, see [about_PowerShell_Ise.exe](https://go.microsoft.com/fwlink/?LinkId=256512).

### Start Windows PowerShell ISE in other ways

For information about other ways to start Windows PowerShell ISE, see [Starting Windows PowerShell](https://go.microsoft.com/fwlink/?LinkID=135259).

### Remarks

Windows PowerShell runs on the Server Core installation option of Windows Server operating systems. However, because Windows PowerShell ISE requires a graphic user interface, it does not run on Server Core installations.

### Additional References

[about_PowerShell_Ise.exe](https://go.microsoft.com/fwlink/?LinkId=256512)
[about_PowerShell.exe](https://go.microsoft.com/fwlink/?LinkID=113439)
[Windows PowerShell](https://go.microsoft.com/fwlink/?LinkID=107116)
[Scripting with Windows PowerShell](https://technet.microsoft.com/scriptcenter/dd742419)
See Also

---



MIT License. Copyright (c) 2020 Strontic.

