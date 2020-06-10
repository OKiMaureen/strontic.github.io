﻿
# Register-CimProvider.exe 
* File Path: `C:\Windows\system32\Register-CimProvider.exe`
* Description: WMI
* Comments: 

## Hashes
Type | Hash
-- | --
MD5 | `2EAEAF637C621487553BDFB6116BA432`
SHA1 | `E6F488805635B2F9F86A009D6B43A276870AA1A7`
SHA256 | `9CB89F4D7557E1659848E7561EC35A7955E7ABF259103BD1BB48BEE16CD1C9B5`
SHA384 | `EB51D8399EDDF8D445E53C40A334F82B0AD6F0364AD8B553B6226C9DACAF2E679465A2009C3E7F9B2CEC76328230069D`
SHA415 | `32CF49751615440D8DA8674B26185C758426CC8E5810BA8A1A746795D28D0ACC2C548850E89B10CB3CEBC0186F304C0890C319C3446B972EAC52C11296D96C96`
SSDEEP | `384:YYej3FYu/Y7uEEZLsG5lrtVpVhuUSfSCioLiTjPk8Qp9XHUol0l3ExvWx1W:YFeu6I/1t3rSaCL+I8+VHUol63Ex2`

## Runtime Data
### Usage (stdout):
```Batchfile

Registers CIM Provider into system

Usage:  Register-CimProvider.exe
		-Namespace <NamespaceName>
		-ProviderName <ProviderName>
		-Path <ProviderDllPath>
		[-ClassList <Space delimited list of white-listed classes>]
		[-Impersonation <True or False>]
		[-Decoupled <SDDL>]
		[-HostingModel <HostingModel>]
		[-Localize <locale>]
		[-NoAutorecover]
		[-SupportWQL]
		[-GenerateUnregistration]
		[-ForceUpdate]
		[-Verbose]

-Namespace <NamespaceName>
	Specifies the target namespace of the provider.

-ProviderName <ProviderName>
	Specifies the provider name.

-Path <ProviderDllPath>
	Specifies the provider binary path.

-Impersonation <True or False>
	Specifies foldidentity of decoupled provider, by default is True.

-Decoupled <SDDL>
	Registers provider as decoupled and specifies the security descriptor
	that determines the set of users that can successfully register
	the provider.

-HostingModel <HostingModel>
	Specifies the HostingModel of coupled provider.

-Localize <locale>
	Localizes the provider with resource of specified locale.

-NoAutorecover
	Doesn't autorecover the provider.

-SupportWQL
	Passes the query expression to the filter.

-GenerateUnregistration
	Generate the uninstall mof for the registration,
	which is disabled by default.

-ForceUpdate
	Force update the class if it exists in the system.

-ClassList <ProviderDllPath>
	Specifies space delimited list of white-listed classes that
	will be generated in the mof.

-Verbose
	Outputs registration log.


```

### Usage (stderr):
```Batchfile

```

### Child Processes:


## Signature

* Status: Signature verified.
* Serial: 33000000BCE120FDD27CC8EE930000000000BC
* Thumbprint: E85459B23C232DB3CB94C7A56D47678F58E8E51E
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: Register-CimProvider2.exe.mui
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.14393.0 (rs1_release.160715-1616)
* Product Version: 10.0.14393.0
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.

