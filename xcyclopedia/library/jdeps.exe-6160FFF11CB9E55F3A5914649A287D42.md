﻿---
title: jdeps.exe | OpenJDK Platform binary
---

# jdeps.exe 

* File Path: `C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jdeps.exe`
* Description: OpenJDK Platform binary

## Hashes

Type | Hash
-- | --
MD5 | `6160FFF11CB9E55F3A5914649A287D42`
SHA1 | `794B248C9E15588EDA71E99C2F70876EAA05DCA0`
SHA256 | `4363BFFFD768D3847811B0D86F0107D34730541632F560FDD60770B78BD9AE2E`
SHA384 | `63E7BEADE805ED567453E70DA283BA3F0E4C0C68A7BF45FCF66413C5B4744371783EBD3E3A9E90DBA1E5DA8A3D56BC50`
SHA512 | `71ABE1BCF8AD74D9CC0C18156AA0C06DF879418E8DD5ED22A98D9A4CABA4E93674425B1350B65ED85F3D76424BE1F1313F05144D086500E5CD67B84876C45532`
SSDEEP | `192:LY+TXeqvDT3I60IKEfoZHy/eExNJ4yK6CYlLWwsUyY8k4Ma9sgfxIZHdt:LYeeuo6TKNZHy/eEHK6jS/Y8iDgf2hdt`

## Runtime Data

### Usage (stdout):
```Batchfile
Usage: jdeps <options> <classes...>
where <classes> can be a pathname to a .class file, a directory, a JAR file,
or a fully-qualified class name.  Possible options include:
  -dotoutput <dir>                   Destination directory for DOT file output
  -s           -summary              Print dependency summary only
  -v           -verbose              Print all class level dependencies
                                     Equivalent to -verbose:class -filter:none.
  -verbose:package                   Print package-level dependencies excluding
                                     dependencies within the same package by default
  -verbose:class                     Print class-level dependencies excluding
                                     dependencies within the same package by default
  -cp <path>   -classpath <path>     Specify where to find class files
  -p <pkgname> -package <pkgname>    Finds dependences matching the given package name
                                     (may be given multiple times)
  -e <regex>   -regex <regex>        Finds dependences matching the given pattern
                                     (-p and -e are exclusive)
  -f <regex>   -filter <regex>       Filter dependences matching the given pattern
                                     If given multiple times, the last one will be used.
  -filter:package                    Filter dependences within the same package (default)
  -filter:archive                    Filter dependences within the same archive
  -filter:none                       No -filter:package and -filter:archive filtering
                                     Filtering specified via the -filter option still applies.
  -include <regex>                   Restrict analysis to classes matching pattern
                                     This option filters the list of classes to
                                     be analyzed.  It can be used together with
                                     -p and -e which apply pattern to the dependences
  -P           -profile              Show profile or the file containing a package
  -apionly                           Restrict analysis to APIs i.e. dependences
                                     from the signature of public and protected
                                     members of public classes including field
                                     type, method parameter types, returned type,
                                     checked exception types etc
  -R           -recursive            Recursively traverse all dependencies.
                                     The -R option implies -filter:none.  If -p, -e, -f
                                     option is specified, only the matching dependences
                                     are analyzed.
  -jdkinternals                      Finds class-level dependences on JDK internal APIs.
                                     By default, it analyzes all classes on -classpath
                                     and input files unless -include option is specified.
                                     This option cannot be used with -p, -e and -s options.
                                     WARNING: JDK internal APIs may not be accessible in
                                     the next release.
  -version                           Version information

```

## Signature

* Status: Signature verified.
* Serial: `2F83C35B5136353D68CE9EB669FD1B0B`
* Thumbprint: `4BAD227329ADEF18F215B6475FB7948E1629B505`
* Issuer: CN=Symantec Class 3 SHA256 Code Signing CA, OU=Symantec Trust Network, O=Symantec Corporation, C=US
* Subject: CN=Amazon.com Services LLC, OU=Software Services, O=Amazon.com Services LLC, L=Seattle, S=Washington, C=US

## File Metadata

* Original Filename: jdeps.exe
* Product Name: OpenJDK Platform 8
* Company Name: Amazon.com Inc.
* File Version: 8.0.2650.1
* Product Version: 8.0.2650.1
* Language: Language Neutral
* Legal Copyright: Copyright  2020

## File Similarity (ssdeep match)

File | Score
-- | --
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\appletviewer.exe](appletviewer.exe-430C820B9C25F84873606F9577ED885C.md) | 57
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\clhsdb.exe](clhsdb.exe-E1BCE5AE504EC02D6CE72820D5C65104.md) | 57
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\extcheck.exe](extcheck.exe-1558E9C8EB7C811CE72AF08BBDE7BC1C.md) | 57
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\hsdb.exe](hsdb.exe-814D8D11A58015EF79936248A91FF87A.md) | 55
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\idlj.exe](idlj.exe-B8FF03F3747D2220B78EF20F5BDFB1A6.md) | 60
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jar.exe](jar.exe-FDE3CD0231E7F936B7914D4BC1DEE713.md) | 58
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jarsigner.exe](jarsigner.exe-916A8B80152B0A5F09F755A6B0F0CEEE.md) | 58
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\javac.exe](javac.exe-E1A9361E0F13035D3450B2E5BF9F565A.md) | 79
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\javadoc.exe](javadoc.exe-D58A3821C950F9A8810571758D454BF3.md) | 71
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\javah.exe](javah.exe-738EEF3648337D35FE7FDDAEDB7A7AE6.md) | 77
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\javap.exe](javap.exe-263625513CED1A2F3CC530A873DA78D8.md) | 75
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jcmd.exe](jcmd.exe-2F08542DE06EE7A5312A3DA2EE2B24BC.md) | 60
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jconsole.exe](jconsole.exe-F6A2528FAF7F94C21B6171C7714CF312.md) | 57
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jdb.exe](jdb.exe-0D18C300EDB8083FE7DF9EBCB73272B7.md) | 57
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jfr.exe](jfr.exe-963613DC729D1F04DBFC1AE070C62FBC.md) | 61
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jhat.exe](jhat.exe-6775B43B078A43741B7A88D7C83E3250.md) | 58
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jinfo.exe](jinfo.exe-698B44C29D5E55EA17046DB44381EAF7.md) | 60
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jjs.exe](jjs.exe-59BBE7560FAA914F246C4E3F29662273.md) | 58
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jmap.exe](jmap.exe-196C8715740CAA592B223567FC81892F.md) | 57
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jps.exe](jps.exe-3E2339751905B0F23F2B60479567B4C5.md) | 61
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jrunscript.exe](jrunscript.exe-26D55A136CF4A9375EBC15B1CC1E3A87.md) | 61
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jsadebugd.exe](jsadebugd.exe-EDD35409A96C24BAA80F32D8A153DBD5.md) | 58
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jstack.exe](jstack.exe-679B7EBA04F034DBEBF7CF23CE7D96FF.md) | 58
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jstat.exe](jstat.exe-4D42D198AEA1B89EA69C6C1EB589A5CF.md) | 61
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\jstatd.exe](jstatd.exe-DCB5BED30B4C0C0DBB8909533ECB53FA.md) | 57
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\keytool.exe](keytool.exe-8E9FA6337C05EA19B49857407FE76324.md) | 54
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\klist.exe](klist.exe-46C3EFEFBB84EF261A21CE50DD82538B.md) | 63
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\native2ascii.exe](native2ascii.exe-4E0D48DBD27C912BAA95BB16392B98DA.md) | 58
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\orbd.exe](orbd.exe-88A71D46CF9DAD0A1A922B7A81FF3F94.md) | 58
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\pack200.exe](pack200.exe-194F7DAC4BF0CE689B11E658EE4BE4EC.md) | 55
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\policytool.exe](policytool.exe-84733E93F92F1C702AD8D51085A0C141.md) | 57
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\rmid.exe](rmid.exe-B2EC7C7A298A74A6A7FE6994EEA30AEB.md) | 58
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\rmiregistry.exe](rmiregistry.exe-A1B6A0957EDC2CE30464D592058BDCFF.md) | 58
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\schemagen.exe](schemagen.exe-2E0814457A3FA699E49A19A5951071A9.md) | 60
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\serialver.exe](serialver.exe-7E2682A55024756C0D6988648EC46F80.md) | 61
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\servertool.exe](servertool.exe-DA2C531652A2C306B02D9A7598ABFA86.md) | 60
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\tnameserv.exe](tnameserv.exe-B95BD13779CB322743ABB3C3AC406B1D.md) | 57
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\wsgen.exe](wsgen.exe-FE1C1F8495990F2BCB301E53BCAB2B79.md) | 60
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\wsimport.exe](wsimport.exe-1789534F6D671FA68ACD4FB49179C70B.md) | 58
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\bin\xjc.exe](xjc.exe-D7067F41EA6E860CC7EFCEF110406D16.md) | 58
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\jre\bin\java-rmi.exe](java-rmi.exe-2C8BE8549F5A30706D882BF98BA1F593.md) | 58
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\jre\bin\jjs.exe](jjs.exe-83B89AADBE362DAAF3AEFDE9B90A7E70.md) | 60
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\jre\bin\keytool.exe](keytool.exe-E64A133341297033FB908CF0412A32EC.md) | 55
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\jre\bin\kinit.exe](kinit.exe-8279A6B305002709B2FA0E42D508F5B7.md) | 57
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\jre\bin\klist.exe](klist.exe-CB6F44DE9B3831B042E93254E6C90991.md) | 57
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\jre\bin\ktab.exe](ktab.exe-4E10E111BC97C675CFE3BF5A40E0D29F.md) | 60
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\jre\bin\orbd.exe](orbd.exe-B7D6DFE20B64D0E89E2CAAC0918C7ABF.md) | 55
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\jre\bin\pack200.exe](pack200.exe-3BA7B22C46AB4E39C166185B6C5644EB.md) | 60
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\jre\bin\policytool.exe](policytool.exe-9000C71F8C10BE60FDC45CDCBF93D25B.md) | 57
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\jre\bin\rmid.exe](rmid.exe-49EA4C57E276B964B770F36A4ACDD764.md) | 58
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\jre\bin\rmiregistry.exe](rmiregistry.exe-AC45D66B78E93F793F684492A0A3BCF8.md) | 54
[C:\Program Files\Amazon Corretto\jdk1.8.0_265\jre\bin\servertool.exe](servertool.exe-7CC71DC253D94C84121954F54EB18BCA.md) | 57
[C:\Program Files\Amazon Corretto\jdk11.0.8_10\bin\javadoc.exe](javadoc.exe-0F018693795EEBE8E09C80212FA8F046.md) | 29
[C:\Program Files\Amazon Corretto\jdk11.0.8_10\bin\jconsole.exe](jconsole.exe-D8C95F3A553D05CB200221FFFB6BA28A.md) | 35
[C:\Program Files\Amazon Corretto\jdk11.0.8_10\bin\jinfo.exe](jinfo.exe-714D372EF77EB0C6C5F3DA8F7BAFED2F.md) | 33
[C:\Program Files\Amazon Corretto\jre8\bin\java-rmi.exe](java-rmi.exe-ABB442793EFD5B49BCBD985457471CBA.md) | 58
[C:\Program Files\Amazon Corretto\jre8\bin\jjs.exe](jjs.exe-88F2557464000E73373C35FC2F541DBD.md) | 58
[C:\Program Files\Amazon Corretto\jre8\bin\keytool.exe](keytool.exe-5B2EED8BF1F4AD2266D1AB4DACD5EFB5.md) | 55
[C:\Program Files\Amazon Corretto\jre8\bin\kinit.exe](kinit.exe-279AB5BC8B1580FBD051A17B03A105FC.md) | 57
[C:\Program Files\Amazon Corretto\jre8\bin\klist.exe](klist.exe-485D7DCE45873697DD951A75B3358C7A.md) | 60
[C:\Program Files\Amazon Corretto\jre8\bin\ktab.exe](ktab.exe-7273553C79E43A7A0FC111E39B2D7462.md) | 61
[C:\Program Files\Amazon Corretto\jre8\bin\orbd.exe](orbd.exe-D0E99C227083E332225BC7C56D66CC32.md) | 57
[C:\Program Files\Amazon Corretto\jre8\bin\pack200.exe](pack200.exe-A7A5CFDD68743FCA89B2006B483F778F.md) | 55
[C:\Program Files\Amazon Corretto\jre8\bin\policytool.exe](policytool.exe-1F96ACF1BC80FE1A0CAD540611C6EBC2.md) | 57
[C:\Program Files\Amazon Corretto\jre8\bin\rmid.exe](rmid.exe-216048544A1924DDFFD12C96094A23F1.md) | 60
[C:\Program Files\Amazon Corretto\jre8\bin\rmiregistry.exe](rmiregistry.exe-11A6CEF71C782AF4B29951C8EA0C4541.md) | 58
[C:\Program Files\Amazon Corretto\jre8\bin\tnameserv.exe](tnameserv.exe-0D875404AEA73CD0FCD92880DA829E70.md) | 57




MIT License. Copyright (c) 2020 Strontic.


