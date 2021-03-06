﻿---
title: upgrade.exe | Glary Utilities Upgrade
---

# upgrade.exe 

* File Path: `C:\Program Files (x86)\Glary Utilities 5\upgrade.exe`
* Description: Glary Utilities Upgrade

## Hashes

Type | Hash
-- | --
MD5 | `9810F0E323B516DE7A1565BFF34CC95F`
SHA1 | `5C5EFF04893A0CC2A54A1BD961B216843CA714CB`
SHA256 | `0E00D23DDD6FC1B70B9C0F75DC564FA6FC32C5390FA1BCE8837F341D2501AAA9`
SHA384 | `8EA9C654E490841A9ED6E138E889E885465F7A0ECA38429201B7B493388DB7E683C639898CBA4EF21D7EE9AF8A3FC10C`
SHA512 | `513E0EBDA484E6370A7A3B8754D8ABC1D75EE42685F5021EC5E548026F10E4961BA2A8B04C5AA6CB858ECA16499D7BC7F59F9AA41E26597FDFDF16FF7407E959`
SSDEEP | `1536:VJMyihOOXd78vyBxF1pnOS8zORuCpeyK5jREdxOSOxiekVHqUfI:VJMyihOOXd7SyBxF1pnOSQORu4ezUxOr`

## Signature

* Status: Signature verified.
* Serial: `0F05AE21CDC17B9F3CF09D7BFC659BA3`
* Thumbprint: `362EBB303E088105BDCC07D94E6B7875D30C0D06`
* Issuer: CN=DigiCert Assured ID Code Signing CA-1, OU=www.digicert.com, O=DigiCert Inc, C=US
* Subject: CN=Glarysoft LTD, O=Glarysoft LTD, S=Beijing, C=CN

## File Metadata

* Original Filename: upgrade.exe
* Product Name: Glary Utilities
* Company Name: Glarysoft Ltd
* File Version: 5.0.0.12
* Product Version: 5.0.0.12
* Language: English
* Legal Copyright: Copyright (c) 2003-2020 Glarysoft Ltd


## Possible Misuse

*The following table contains possible examples of `upgrade.exe` being misused. While `upgrade.exe` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[sigma](https://github.com/Neo23x0/sigma) | [pypi-publish.yml](https://github.com/Neo23x0/sigma/blob/master/.github/workflows/pypi-publish.yml) | `        python -m pip install --upgrade pip` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [sigma-test.yml](https://github.com/Neo23x0/sigma/blob/master/.github/workflows/sigma-test.yml) | `        python -m pip install --upgrade pip` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_service_stop.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_service_stop.yml) | `    - Administrator shutting down the service due to upgrade or removal purposes` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[malware-ioc](https://github.com/eset/malware-ioc) | [rakos.yar](https://github.com/eset/malware-ioc/blob/master/rakos/rakos.yar) | `        $ = "upgrade/vars.yaml"` | [© ESET 2014-2018](https://github.com/eset/malware-ioc/blob/master/LICENSE)
[malware-ioc](https://github.com/eset/malware-ioc) | [vf_ioc_linux_rakos.py](https://github.com/eset/malware-ioc/blob/master/rakos/vf_ioc_linux_rakos.py) | `                          $ = "upgrade/vars.yaml"` | [© ESET 2014-2018](https://github.com/eset/malware-ioc/blob/master/LICENSE)
[atomic-red-team](https://github.com/redcanaryco/atomic-red-team) | [python](https://github.com/redcanaryco/atomic-red-team/blob/master/execution-frameworks/contrib/python/README.md) | - Upgrade pip to the latest version: "pip install --upgrade pip" | [MIT License. © 2018 Red Canary](https://github.com/redcanaryco/atomic-red-team/blob/master/LICENSE.txt)
[signature-base](https://github.com/Neo23x0/signature-base) | [apt_vpnfilter.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/apt_vpnfilter.yar) |       $x3 = "Please upgrade! This version of Tor (%s) is %s, according to the directory authorities. Recommended versions are: %s" fullword ascii | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)
[signature-base](https://github.com/Neo23x0/signature-base) | [crime_mirai.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/crime_mirai.yar) |       $s2 = "loadURL>$(echo HUAWEIUPNP)</NewDownloadURL></u:Upgrade></s:Body></s:Envelope>" fullword ascii | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)
[signature-base](https://github.com/Neo23x0/signature-base) | [yara_mixed_ext_vars.yar](https://github.com/Neo23x0/signature-base/blob/master/yara/yara_mixed_ext_vars.yar) | 		$s2 = "Virtual hardware upgrade helper service" fullword wide | [CC BY-NC 4.0](https://github.com/Neo23x0/signature-base/blob/master/LICENSE)



MIT License. Copyright (c) 2020 Strontic.


