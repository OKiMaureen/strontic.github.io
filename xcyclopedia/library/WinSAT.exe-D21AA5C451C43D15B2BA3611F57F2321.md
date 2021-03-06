﻿---
title: WinSAT.exe | Windows System Assessment Tool
---

# WinSAT.exe 

* File Path: `C:\windows\system32\WinSAT.exe`
* Description: Windows System Assessment Tool

## Hashes

Type | Hash
-- | --
MD5 | `D21AA5C451C43D15B2BA3611F57F2321`
SHA1 | `BD152D8C2467B974DCA7B2B11982D3EA06B2B4F9`
SHA256 | `2380049E6E56B969990C598A3731E8322E8DEF86B08DFE44E452392CF529498D`
SHA384 | `534D32F50C97A3BAC33C98C9F586877A66C1B8DE393C53ED50C435D0F4B0D242B770869F6EFBDBAC4138DE7C7EECB2DA`
SHA512 | `08BE8EB24D22C41623BA482CB89B8995C52BB06555A3F4A24E8075C5C913D760456DFE95C95E347252F2975DB254F32349C55C21E0BD69F4268B48D891915CB7`
SSDEEP | `49152:/XpiCMrI7ninpTyjY7Q9i9GYmq1dKwdfU2bECbe:PUCUzT1DFE/`

## Runtime Data

### Usage (stdout):
```Batchfile

Windows System Assessment Tool

    
COMMAND LINE USAGE :   
    WINSAT <assessment_name> [switches]

It's necessary to supply an assessment name.  In contrast, switches are optional. 
Valid assessment names already seen in Vista include: 

    formal		run the full set of assessments 

    dwm		Run the Desktop Windows Manager assessment
            - Re-assess the systems graphics capabilities and 
              restart the Desktop Window Manager.

    cpu		Run the CPU assessment.  
    mem		Run the system memory assessment.  
    d3d		Run the d3d assessment 
                (Note that the d3d assessment no longer runs the workload. 
                For backward compatibility, pre-determined scores and metrics are reported.)
    disk		Run the storage assessment
    media		Run the media assessment 			
    mfmedia		Run the Media Foundation based assessment	
    features	Run just the features assessment      		
            - Enumerates the system's features. 
            - It's best used with the -xml <filename> switch 
            to save the data.  
            - The 'eef'switch can be used to enumerate extra 
            features such as optical disks,	memory modules, 
            and other items.
    
PRE-POPULATION: 
The new command-line  options for pre-populating WinSAT assessment results are :  
    
    Winsat prepop [-datastore <directory>] [ -graphics | -cpu | -mem | -disk | -dwm ]


This generates WinSAT xml files whose filenames contain "prepop".  For example :
    0008-09-26 14.48.28.542 Cpu.Assessment (Prepop).WinSAT.xml

The filename pattern is :	
    %IdentifierDerivedFromDate% %Component%.Assessment(Prepop).WinSAT.xml

The datastore directory option specifies an alternative target location for generated xml files. 
If no location is specified, everything is pre-populated to 
    %WINDIR%\performance\winsat\datastore.  

To generate a full set of result xml files, use "winsat prepop".  

It is also possible to pre-populate results for a subsystem, such as CPU, 
subject to the following dependencies:

    The CPU assessment has a secondary dependency on the Memory assessment
    The Memory assessment has a secondary dependency on the CPU assessment
    The Graphics assessment has a secondary dependency on both CPU and Memory assessments
    The DWM assessment can run standalone
    The Disk assessment can run standalone 

If the assessment for a secondary dependency is not present, WinSAT will run the 
secondary assessment along with the requested primary assessment.  

For example,  "winsat prepop -cpu"  will run both the CPU and the Memory test, 
if the xml file for the Memory test is not present.	



OTHER NEW Win7 ASSESSMENT OPTIONS :

    dwmformal	Run Desktop Windows Manager assessment to generate the WinSAT Graphics score
    cpuformal	Run CPU assessment to generate the WinSAT Processor score
    memformal	Run Memory assessment to generate the WinSAT Memory (RAM) score
    graphicsformal	Run Graphics assessment to generate the WinSAT Gaming Graphics score
    diskformal	Run Disk assessment to generate the WinSAT Primary Hard Disk score
            
All formal assessments will save the data (xml files) in 
        %WINDIR%\performance\winsat\datastore.  

If a system has been prepopulated (using files generated by the "winsat prepop" option), 
it is not necessary to run formal assessments.


SUB-ASSESSMENTS:
While investigating results, it may be convenient to look at individual assessments.  
Options for running Gaming Graphics sub-assessments include:

    Winsat graphicsformal3d
    Winsat graphicsformalmedia

    DX9 Variations:  
        Winsat d3d -dx9
        winsat d3d -batch
        winsat d3d -alpha
        winsat d3d -tex
        winsat d3d -alu

    DWM/DX10 variations:  
        Winsat d3d -dx10
        winsat d3d -dx10 -alpha
        winsat d3d -dx10 -tex
        winsat d3d -dx10 -alu
        winsat d3d -dx10 -batch
        winsat d3d -dx10 -geomf4
        winsat d3d -dx10 -geomf27
        winsat d3d -dx10 -geomv8
        winsat d3d -dx10 -gemov32
        winsat d3d -dx10 -cbuffer



OPTIONS FOR FORMAL ASSESSMENTS FOR SUBSEQUENT RUNS ON THE SAME MACHINE:

The default behavior for "WinSAT formal" when a complete set of winsat formal files is present 
and a second "winsat formal" run is requested is to 
    1) Run incrementally if component change implies that an assessment needs to be re-run, 
        e.g. if a video card were updated  
    2) If no component updates were detected, re-run all assessments.

    The restart option enables behavior other than the default.  The syntax is :   	
        Winsat formal -restart [clean|never]
    
        Winsat formal -restart	 	Reruns all assessments. 
        Winsat formal -restart never 	Attempts to run incrementally.
        Winsat formal -restart clean 	Reruns all assessments and provides the same functionality as "forgethistory". 
        Winsat forgethistory		Choosing to forgethistory will rate a machine as if for the first time.


OTHER COMMAND LINE OPTIONS :
    -v			Enables verbose output
    -xml			Saves the XML output to 'filename'

    <command> -log <fn>	Generates a log file associated with the specified command, such as disk
                The -log switch can be used with any WinSAT command.

    viewlog -i <filename> 	Dumps the results of a log file .  
    viewevents 		Used to view relevant winsat events in the event log. 
                (This launches the event log)
    query 			Can be used to query the current datastore.

```

### Usage (stderr):
```Batchfile
Error: Unable to run inside of a Virtual Machine.  Please try again running directly on the native hardware.

```

## Signature

* Status: Signature verified.
* Serial: `3300000266BD1580EFA75CD6D3000000000266`
* Thumbprint: `A4341B9FD50FB9964283220A36A1EF6F6FAA7840`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: WinSAT.exe.mui
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.17763.1 (WinBuild.160101.0800)
* Product Version: 10.0.17763.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.

## File Similarity (ssdeep match)

File | Score
-- | --
[C:\Windows\system32\WinSAT.exe](WinSAT.exe-6654FC269DF21AA165842E479678A94B.md) | 47
[C:\Windows\system32\WinSAT.exe](WinSAT.exe-715DB53A8064C6DECCF68B7501DF3386.md) | 54
[C:\WINDOWS\system32\WinSAT.exe](WinSAT.exe-ED2505CC79AB0C0008E1A23A731D9107.md) | 50




MIT License. Copyright (c) 2020 Strontic.


