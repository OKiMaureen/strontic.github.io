﻿---
title: fc.exe | DOS 5 File Compare Utility
---

# fc.exe 

* File Path: `C:\windows\system32\fc.exe`
* Description: DOS 5 File Compare Utility

## Hashes

Type | Hash
-- | --
MD5 | `041DD62718BF388E6671F00BF2FE68A4`
SHA1 | `D808ED9E5FEAA8DC9227CE05DE4F352B52B35ECC`
SHA256 | `953BCC35710ED410212BD56CDEA2E25FD9BC013707DF17CB203E102A4F9C05DA`
SHA384 | `ACC6FCCCCBC0F20340A46D27F814711D36DAD5CB046C135226561696C8712E41F8CBEA81B6D92C032E5211BDA229DE44`
SHA512 | `A6FC31D6479A50994733757ECD8628120424EEEE87D31DA697807746C885EF637F6E033C2781873E96DAFFA337BBC8F0F040323675FFE56CAC4C6059FDAF5E56`
SSDEEP | `384:gZC8g8G2Za8TMqgJBsByUWRcAzjLhgXWC5XGKK74KC81WWaYW:QC8UUAqgUM3t6XWWXGXfC`

## Runtime Data

### Usage (stdout):
```Batchfile
Compares two files or sets of files and displays the differences between
them


FC [/A] [/C] [/L] [/LBn] [/N] [/OFF[LINE]] [/T] [/U] [/W] [/nnnn]
   [drive1:][path1]filename1 [drive2:][path2]filename2
FC /B [drive1:][path1]filename1 [drive2:][path2]filename2

  /A         Displays only first and last lines for each set of differences.
  /B         Performs a binary comparison.
  /C         Disregards the case of letters.
  /L         Compares files as ASCII text.
  /LBn       Sets the maximum consecutive mismatches to the specified
             number of lines.
  /N         Displays the line numbers on an ASCII comparison.
  /OFF[LINE] Do not skip files with offline attribute set.
  /T         Does not expand tabs to spaces.
  /U         Compare files as UNICODE text files.
  /W         Compresses white space (tabs and spaces) for comparison.
  /nnnn      Specifies the number of consecutive lines that must match
             after a mismatch.
  [drive1:][path1]filename1
             Specifies the first file or set of files to compare.
  [drive2:][path2]filename2
             Specifies the second file or set of files to compare.


```

### Usage (stderr):
```Batchfile
FC: Insufficient number of file specifications


```

## Signature

* Status: Signature verified.
* Serial: `33000001C422B2F79B793DACB20000000001C4`
* Thumbprint: `AE9C1AE54763822EEC42474983D8B635116C8452`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: FC.EXE.MUI
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.17763.1 (WinBuild.160101.0800)
* Product Version: 10.0.17763.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.



## Additional Info*

**The information below is copied from [MicrosoftDocs](https://github.com/MicrosoftDocs/windowsserverdocs), which is maintained by [Microsoft](https://opensource.microsoft.com/codeofconduct/). Available under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.*

---

## fc

Compares two files or sets of files and displays the differences between them.

### Syntax

```
fc /a [/c] [/l] [/lb<n>] [/n] [/off[line]] [/t] [/u] [/w] [/<nnnn>] [<drive1>:][<path1>]<filename1> [<drive2>:][<path2>]<filename2>
fc /b [<drive1:>][<path1>]<filename1> [<drive2:>][<path2>]<filename2>
```

#### Parameters

| Parameter | Description |
| --------- | ----------- |
| /a | Abbreviates the output of an ASCII comparison. Instead of displaying all of the lines that are different, **fc** displays only the first and last line for each set of differences. |
| /b | Compares the two files in binary mode, byte by byte, and does not attempt to resynchronize the files after finding a mismatch. This is the default mode for comparing files that have the following file extensions: .exe, .com, .sys, .obj, .lib, or .bin. |
| /c | Ignores the letter case. |
| /l | Compares the files in ASCII mode, line-by-line, and attempts to resynchronize the files after finding a mismatch. This is the default mode for comparing files, except files with the following file extensions: .exe, .com, .sys, .obj, .lib, or .bin. |
| /lb`<n>` | Sets the number of lines for the internal line buffer to *N*. The default length of the line buffer is 100 lines. If the files that you are comparing have more than 100 consecutive differing lines, **fc** cancels the comparison. |
| /n | Displays the line numbers during an ASCII comparison. |
| /off[line] | Doesn't skip files that have the offline attribute set. |
| /t | Prevents **fc** from converting tabs to spaces. The default behavior is to treat tabs as spaces, with stops at each eighth character position. |
| /u | Compares files as Unicode text files. |
| /w | Compresses white space (that is, tabs and spaces) during the comparison. If a line contains many consecutive spaces or tabs, **/w** treats these characters as a single space. When used with **/w**, **fc** ignores white space at the beginning and end of a line. |
| /`<nnnn>` | Specifies the number of consecutive lines that must match following a mismatch, before **fc** considers the files to be resynchronized. If the number of matching lines in the files is less than *nnnn*, **fc** displays the matching lines as differences. The default value is 2. |
| `[<drive1>:][<path1>]<filename1>` | Specifies the location and name of the first file or set of files to compare. *filename1* is required. |
| `[<drive2>:][<path2>]<filename2>` | Specifies the location and name of the second file or set of files to compare. *filename2* is required. |
| /? | Displays help at the command prompt. |

##### Remarks

- This command is implemeted by c:\WINDOWS\fc.exe. You can use this command within PowerShell, but be sure to spell out the full executable (fc.exe) since 'fc' is also an alias for Format-Custom.

- When you use **fc** for an ASCII comparison, **fc** displays the differences between two files in the following order:

  - Name of the first file

  - Lines from *filename1* that differ between the files

  - First line to match in both files

  - Name of the second file

  - Lines from *filename2* that differ

  - First line to match

- **/b** displays mismatches that are found during a binary comparison in the following syntax:

    `\<XXXXXXXX: YY ZZ>`

    The value of *XXXXXXXX* specifies the relative hexadecimal address for the pair of bytes, measured from the beginning of the file. Addresses start at 00000000. The hexadecimal values for *YY* and *ZZ* represent the mismatched bytes from *filename1* and *filename2*, respectively.

- You can use wildcard characters (**&#42;** and **?**) in *filename1* and *filename2*. If you use a wildcard in *filename1*, **fc** compares all the specified files to the file or set of files specified by *filename2*. If you use a wildcard in *filename2*, **fc** uses the corresponding value from *filename1*.

- When comparing ASCII files, **fc** uses an internal buffer (large enough to hold 100 lines) as storage. If the files are larger than the buffer, **fc** compares what it can load into the buffer. If **fc** doesn't find a match in the loaded portions of the files, it stops and displays the following message:

    `Resynch failed. Files are too different.`

    When comparing binary files that are larger than the available memory, **fc** compares both files completely, overlaying the portions in memory with the next portions from the disk. The output is the same as that for files that fit completely in memory.

#### Examples

To make an ASCII comparison of two text files, *monthly.rpt* and *sales.rpt*, and display the results in abbreviated format, type:

```
fc /a monthly.rpt sales.rpt
```

To make a binary comparison of two batch files, *profits.bat* and *earnings.bat*, type:

```
fc /b profits.bat earnings.bat
```

Results similar to the following appear:

```
00000002: 72 43
00000004: 65 3A
0000000E: 56 92
000005E8: 00 6E
FC: earnings.bat longer than profits.bat
```

If the profits.bat and earnings.bat files are identical, **fc** displays the following message:

```
Comparing files profits.bat and earnings.bat
FC: no differences encountered
```

To compare every .bat file in the current directory with the file *new.bat*, type:

```
fc *.bat new.bat
```

To compare the file *new.bat* on drive C with the file *new.bat* on drive D, type:

```
fc c:new.bat d:*.bat
```

To compare each batch file in the root directory on drive C to the file with the same name in the root directory on drive D, type:

```
fc c:*.bat d:*.bat
```

### Additional References

- [Command-Line Syntax Key](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/command-line-syntax-key.md)

---



MIT License. Copyright (c) 2020 Strontic.


