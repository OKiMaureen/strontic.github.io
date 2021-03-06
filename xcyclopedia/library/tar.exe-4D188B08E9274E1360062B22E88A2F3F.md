﻿---
title: tar.exe | bsdtar archive tool
---

# tar.exe 

* File Path: `C:\Windows\system32\tar.exe`
* Description: bsdtar archive tool

## Hashes

Type | Hash
-- | --
MD5 | `4D188B08E9274E1360062B22E88A2F3F`
SHA1 | `F93374196F5F6E19B370CDDD9332AC248937E5EF`
SHA256 | `0F28C8D166C7A671B0048137232E9CA6973F1EC826104834AE310681C1866E62`
SHA384 | `FE40A7B2E90581E231295F445F6DB120EA30CB4FA05A42BC0EB120E28A3F269DB1F711EFC87AB89C6DA93348EE90872B`
SHA512 | `5B0D1D2F0E48FB3B250891163C2F1E935663B6865483180EDD1167B8F3269508977893E3FAF905D0676EF0A5CBFDD3486A66D3D521643D68DDA7E55528337207`
SSDEEP | `768:CciB9nbl48DFyNO63/JoH4jEjwlz18rOq5+fQgD77uPhyHijOuPhtflM7J5SpxdG:Fy9nbktRoH4jAOz7CPZpPBMLSp7Kr`

## Runtime Data

### Usage (stdout):
```Batchfile
tar.exe(bsdtar): manipulate archive files
First option must be a mode specifier:
  -c Create  -r Add/Replace  -t List  -u Update  -x Extract
Common Options:
  -b #  Use # 512-byte records per I/O block
  -f <filename>  Location of archive (default \\.\tape0)
  -v    Verbose
  -w    Interactive
Create: tar.exe -c [options] [<file> | <dir> | @<archive> | -C <dir> ]
  <file>, <dir>  add these items to archive
  -z, -j, -J, --lzma  Compress archive with gzip/bzip2/xz/lzma
  --format {ustar|pax|cpio|shar}  Select archive format
  --exclude <pattern>  Skip files that match pattern
  -C <dir>  Change to <dir> before processing remaining files
  @<archive>  Add entries from <archive> to output
List: tar.exe -t [options] [<patterns>]
  <patterns>  If specified, list only entries that match
Extract: tar.exe -x [options] [<patterns>]
  <patterns>  If specified, extract only entries that match
  -k    Keep (don't overwrite) existing files
  -m    Don't restore modification times
  -O    Write entries to stdout, don't restore to disk
  -p    Restore permissions (including ACLs, owner, file flags)
bsdtar 3.3.2 - libarchive 3.3.2 zlib/1.2.5.f-ipp

```

### Usage (stderr):
```Batchfile
Usage:
  List:    tar.exe -tf <archive-filename>
  Extract: tar.exe -xf <archive-filename>
  Create:  tar.exe -cf <archive-filename> [filenames...]
  Help:    tar.exe --help

```

## Signature

* Status: Signature verified.
* Serial: `3300000266BD1580EFA75CD6D3000000000266`
* Thumbprint: `A4341B9FD50FB9964283220A36A1EF6F6FAA7840`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: bsdtar
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 3.3.2 (WinBuild.160101.0800)
* Product Version: 10.0.19041.1
* Language: English (United States)
* Legal Copyright: Copyright (c) libarchive authors

## File Similarity (ssdeep match)

File | Score
-- | --
[C:\Windows\system32\tar.exe](tar.exe-0B8821B257EEE9C01CD29C62AE9D3EF9.md) | 27
[C:\WINDOWS\system32\tar.exe](tar.exe-5F6B04A0EC5FE46FEEEC887406F63E57.md) | 29




MIT License. Copyright (c) 2020 Strontic.


