﻿---
title: wecutil.exe | Event Collector Command Line Utility
---

# wecutil.exe 

* File Path: `C:\windows\system32\wecutil.exe`
* Description: Event Collector Command Line Utility

## Hashes

Type | Hash
-- | --
MD5 | `21F57C1E019094BC410FDFFFE542C62E`
SHA1 | `E198E04C7BCC584779CAB9A42E5D6AA13D668395`
SHA256 | `96F7CA1B02C1A0D63747F0BD1448A723A4F49CBEF45A0DBB168E69B2F5FB98F5`
SHA384 | `3140A0357CE042D7C4604D4DB3ADEE995B2E7FC25138048626CA29BE8741DA5B004EFC320946E27CAADB287C8A3FC0DD`
SHA512 | `2F843C9034B8E274E4A9C4F101E95B3917AF2D29215B41D1FC4B17B47C2EE0F64D15953AAF5D06FAF73D223662D631593445981C0854959E7D4814F10820672A`
SSDEEP | `3072:9m7rsTmitRNqIc9rijGByFvW6nuFe7jjf:9m7Amd7iaUZuFAj`

## Runtime Data

### Usage (stdout):
```Batchfile
Windows Event Collector Utility

Enables you to create and manage subscriptions to events forwarded from remote
event sources that support WS-Management protocol.

Usage:

You can use either the short (i.e. es, /f) or long (i.e. enum-subscription, /format)
version of the command and option names. Commands, options and option values are
case-insensitive.

(ALL UPPER-CASE = VARIABLE)

wecutil COMMAND [ARGUMENT [ARGUMENT] ...] [/OPTION:VALUE [/OPTION:VALUE] ...]

Commands:

es (enum-subscription)               List existent subscriptions.
gs (get-subscription)                Get subscription configuration.
gr (get-subscriptionruntimestatus)   Get subscription runtime status.
ss (set-subscription)                Set subscription configuration.
cs (create-subscription)             Create new subscription.
ds (delete-subscription)             Delete subscription.
rs (retry-subscription)              Retry subscription.
qc (quick-config)                    Configure Windows Event Collector service.

Common options:

/h|? (help)
Get general help for the wecutil program.

wecutil { -help | -h | -? }

For arguments and options, see usage of specific commands:

wecutil COMMAND -?

```

### Usage (stderr):
```Batchfile
Command help is not supported. Error = 0x57.
The parameter is incorrect.

```

## Signature

* Status: Signature verified.
* Serial: `33000001C422B2F79B793DACB20000000001C4`
* Thumbprint: `AE9C1AE54763822EEC42474983D8B635116C8452`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: WECUTIL.EXE.MUI
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.17763.1 (WinBuild.160101.0800)
* Product Version: 10.0.17763.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.



## Additional Info*

**The information below is copied from [MicrosoftDocs](https://github.com/MicrosoftDocs/windowsserverdocs), which is maintained by [Microsoft](https://opensource.microsoft.com/codeofconduct/). Available under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.*

---

## wecutil



Enables you to create and manage subscriptions to events that are forwarded from remote computers. The remote computer must support the WS-Management protocol.


### Syntax

```
wecutil  [{es | enum-subscription}]
[{gs | get-subscription} <Subid> [/f:<Format>] [/uni:<Unicode>]]
[{gr | get-subscriptionruntimestatus} <Subid> [<Eventsource> â€¦]]
[{ss | set-subscription} [<Subid> [/e:[<Subenabled>]] [/esa:<Address>] [/ese:[<Srcenabled>]] [/aes] [/res] [/un:<Username>] [/up:<Password>] [/d:<Desc>] [/uri:<Uri>] [/cm:<Configmode>] [/ex:<Expires>] [/q:<Query>] [/dia:<Dialect>] [/tn:<Transportname>] [/tp:<Transportport>] [/dm:<Deliverymode>] [/dmi:<Deliverymax>] [/dmlt:<Deliverytime>] [/hi:<Heartbeat>] [/cf:<Content>] [/l:<Locale>] [/ree:[<Readexist>]] [/lf:<Logfile>] [/pn:<Publishername>] [/essp:<Enableport>] [/hn:<Hostname>] [/ct:<Type>]] [/c:<Configfile> [/cun:<Username> /cup:<Password>]]]
[{cs | create-subscription} <Configfile> [/cun:<Username> /cup:<Password>]]
[{ds | delete-subscription} <Subid>]
[{rs | retry-subscription} <Subid> [<Eventsource>â€¦]]
[{qc | quick-config} [/q:[<Quiet>]]].
```

#### Parameters

|Parameter|Description|
|---------|-----------|
|{es \| enum-subscription}|Displays the names of all remote event subscriptions that exist.|
|{gs \| get-subscription} \<Subid> [/f:\<Format>] [/uni:\<Unicode>]|Displays remote subscription configuration information. \<Subid> is a string that uniquely identifies a subscription. \<Subid> is the same as the string that was specified in the \<SubscriptionId> tag of the XML configuration file, which was used to create the subscription.|
|{gr \| get-subscriptionruntimestatus} \<Subid> [\<Eventsource> â€¦]|Displays the runtime status of a subscription. \<Subid> is a string that uniquely identifies a subscription. \<Subid> is the same as the string that was specified in the \<SubscriptionId> tag of the XML configuration file, which was used to create the subscription. \<Eventsource> is a string that identifies a computer that serves as a source of events. \<Eventsource> should be a fully qualified domain name, a NetBIOS name, or an IP address.|
|{ss \| set-subscription} \<Subid> [/e:[\<Subenabled>]] [/esa:\<Address>] [/ese:[\<Srcenabled>]] [/aes] [/res] [/un:\<Username>] [/up:\<Password>] [/d:\<Desc>] [/uri:\<Uri>] [/cm:\<Configmode>] [/ex:\<Expires>] [/q:\<Query>] [/dia:\<Dialect>] [/tn:\<Transportname>] [/tp:\<Transportport>]  [/dm:\<Deliverymode>] [/dmi:\<Deliverymax>] [/dmlt:\<Deliverytime>] [/hi:\<Heartbeat>] [/cf:\<Content>] [/l:\<Locale>] [/ree:[\<Readexist>]] [/lf:\<Logfile>] [/pn:\<Publishername>] [/essp:\<Enableport>] [/hn:\<Hostname>] [/ct:\<Type>]</br>or</br>{ss \| set-subscription /c:\<Configfile> [/cun:\<Comusername> /cup:\<Compassword>]|Changes the subscription configuration. You can specify the subscription ID and the appropriate options to change subscription parameters, or you can specify an XML configuration file to change subscription parameters.|
|{cs \| create-subscription} \<Configfile> [/cun:\<Username> /cup:\<Password>]|Creates a remote subscription. \<Configfile> specifies the path to the XML file that contains the subscription configuration. The path can be absolute or relative to the current directory.|
|{ds \| delete-subscription} \<Subid>|Deletes a subscription and unsubscribes from all event sources that deliver events into the event log for the subscription. Any events already received and logged are not deleted. \<Subid> is a string that uniquely identifies a subscription. \<Subid> is the same as the string that was specified in the \<SubscriptionId> tag of the XML configuration file, which was used to create the subscription.|
|{rs \| retry-subscription} \<Subid> [\<Eventsource>â€¦]|Retries to establish a connection and send a remote subscription request to an inactive subscription. Attempts to reactivate all event sources or specified event sources. Disabled sources are not retried. \<Subid> is a string that uniquely identifies a subscription. \<Subid> is the same as the string that was specified in the \<SubscriptionId> tag of the XML configuration file, which was used to create the subscription. \<Eventsource> is a string that identifies a computer that serves as a source of events. \<Eventsource> should be a fully qualified domain name, a NetBIOS name, or an IP address.|
|{qc \| quick-config} [/q:[\<Quiet>]]|Configures the Windows Event Collector service to ensure a subscription can be created and sustained through reboots. This includes the following steps:</br>1.  Enable the ForwardedEvents channel if it is disabled.</br>2.  Set the Windows Event Collector service to delay start.</br>3.  Start the Windows Event Collector service if it is not running.|

### Options

|Option|Description|
|------|-----------|
|/f:\<Format>|Specifies the format of the information that is displayed. \<Format> can be XML or Terse. If <Format> is XML, the output is displayed in XML format. If \<Format> is Terse, the output is displayed in name-value pairs. The default is Terse.|
|/c:\<Configfile>|Specifies the path to the XML file that contains a subscription configuration. The path can be absolute or relative to the current directory. This option can only be used with the **/cun** and **/cup** options and is mutually exclusive with all other options.|
|/e:[\<Subenabled>]|Enables or disables a subscription. \<Subenabled> can be true or false. The default value of this option is true.|
|/esa:\<Address>|Specifies the address of an event source. \<Address> is a string that contains a fully qualified domain name, a NetBIOS name, or an IP address, which identifies a computer that serves as a source of events. This option should be used with the **/ese**, **/aes**, **/res**, or **/un** and **/up** options.|
|/ese:[\<Srcenabled>]|Enables or disables an event source. \<Srcenabled> can be true or false. This option is allowed only if the **/esa** option is specified. The default value of this option is true.|
|/aes|Adds the event source that is specified by the **/esa** option if it is not already a part of the subscription. If the address specified by the **/esa** option is already a part of the subscription, an error is reported. This option is only allowed if the **/esa** option is specified.|
|/res|Removes the event source that is specified by the **/esa** option if it is already a part of the subscription. If the address specified by the **/esa** option is not a part of the subscription, an error is reported. This option is only allowed if **/esa** option is specified.|
|/un:\<Username>|Specifies the user credential to use with the event source specified by the **/esa** option. This option is only allowed if the **/esa** option is specified.|
|/up:\<Password>|Specifies the password that corresponds to the user credential. This option is only allowed if the **/un** option is specified.|
|/d:\<Desc>|Provides a description for the subscription.|
|/uri:\<Uri>|Specifies the type of the events that are consumed by the subscription. \<Uri> contains a URI string that is combined with the address of the event source computer to uniquely identify the source of the events. The URI string is used for all event source addresses in the subscription.|
|/cm:\<Configmode>|Sets the configuration mode. \<Configmode> can be one of the following strings: Normal, Custom, MinLatency or MinBandwidth. The Normal, MinLatency, and MinBandwidth modes set delivery mode, delivery max items, heartbeat interval, and delivery max latency time. The **/dm**, **/dmi**, **/hi** or **/dmlt** options may only be specified if the configuration mode is set to Custom.|
|/ex:\<Expires>|Sets the time when the subscription expires. \<Expires> should be defined in standard XML or ISO8601 date-time format: yyyy-MM-ddThh:mm:ss[.sss][Z], where T is the time separator and Z indicates UTC time.|
|/q:\<Query>|Specifies the query string for the subscription. The format of \<Query> may be different for different URI values and applies to all sources in the subscription.|
|/dia:\<Dialect>|Defines the dialect that the query string uses.|
|/tn:\<Transportname>|Specifies the name of the transport that is used to connect to a remote event source.|
|/tp:\<Transportport>|Sets the port number that is used by the transport when connecting to a remote event source.|
|/dm:\<Deliverymode>|Specifies the delivery mode. \<Deliverymode> can be either pull or push. This option is only valid if the **/cm** option is set to Custom.|
|/dmi:\<Deliverymax>|Sets the maximum number of items for batched delivery. This option is only valid if **/cm** is set to Custom.|
|/dmlt:\<Deliverytime>|Sets the maximum latency in delivering a batch of events. \<Deliverytime> is the number of milliseconds. This option is only valid if **/cm** is set to Custom.|
|/hi:\<Heartbeat>|Defines the heartbeat interval. \<Heartbeat> is the number of milliseconds. This option is only valid if **/cm** is set to Custom.|
|/cf:\<Content>|Specifies the format of the events that are returned. \<Content> can be Events or RenderedText. When the value is RenderedText, the events are returned with the localized strings (such as event description) attached to the event. The default value is RenderedText.|
|/l:\<Locale>|Specifies the locale for delivery of the localized strings in RenderedText format. \<Locale> is a language and country/region identifier, for example, EN-us. This option is only valid if the **/cf** option is set to RenderedText.|
|/ree:[\<Readexist>]|Identifies the events that are delivered for the subscription. \<Readexist> can true or false. When the <Readexist> is true, all existing events are read from the subscription event sources. When the <Readexist> is false, only future (arriving) events are delivered. The default value is true for a **/ree** option without a value. If no **/ree** option is specified, the default value is false.|
|/lf:\<Logfile>|Specifies the local event log that is used to store events received from the event sources.|
|/pn:\<Publishername>|Specifies the publisher name. It must be a publisher that owns or imports the log specified by the **/lf** option.|
|/essp:\<Enableport>|Specifies that the port number must be appended to the service principal name of the remote service. \<Enableport> can be true or false. The port number is appended when <Enableport> is true. When the port number is appended, some configuration may be required to prevent the access to event sources from being denied.|
|/hn:\<Hostname>|Specifies the DNS name of the local computer. This name is used by remote event source to push back events and must be used only for a push subscription.|
|/ct:\<Type>|Sets the credential type for the remote source access. \<Type> should be one of the following values: default, negotiate, digest, basic or localmachine. The default value is default.|
|/cun:\<Comusername>|Sets the shared user credential to be used for event sources that do not have their own user credentials. If this option is specified with the **/c** option, UserName and UserPassword settings for individual event sources from the configuration file are ignored. If you want to use a different credential for a specific event source, you should override this value by specifying the **/un** and **/up** options for a specific event source on the command line of another **ss** command.|
|/cup:\<Compassword>|Sets the user password for the shared user credential. When \<Compassword> is set to * (asterisk), the password is read from the console. This option is only valid when the **/cun** option is specified.|
|/q:[\<Quiet>]|Specifies whether the configuration procedure prompts for confirmation. \<Quiet> can be true or false. If <Quiet> is true, the configuration procedure does not prompt for confirmation. The default value of this option is false.|

### Remarks

> [!IMPORTANT]
> If you receive the message, â€œThe RPC server is unavailable? when you try to run wecutil, you need to start the Windows Event Collector service (wecsvc). To start wecsvc, at an elevated command prompt type net start wecsvc.

- To shows the contents of a configuration file:
  ```
  <Subscription xmlns=https://schemas.microsoft.com/2006/03/windows/events/subscription>
  <Uri>https://schemas.microsoft.com/wbem/wsman/1/windows/EventLog</Uri>
  <!-- Use Normal (default), Custom, MinLatency, MinBandwidth -->
  <ConfigurationMode>Normal</ConfigurationMode>
  <Description>Forward Sample Subscription</Description>
  <SubscriptionId>SampleSubscription</SubscriptionId>
  <Query><![CDATA[
  <QueryList>
  <Query Path=Application>
  <Select>*</Select>
  </Query>
  </QueryList>
  ]]></Query>
  <EventSources>
  <EventSource Enabled=true>
  <Address>mySource.myDomain.com</Address>
  <UserName>myUserName</UserName>
  <Password>*</Password>
  </EventSource>
  </EventSources>
  <CredentialsType>Default</CredentialsType>
  <Locale Language=EN-US></Locale>
  </Subscription>
  ```

### Examples

Output configuration information for a subscription named sub1:
```
wecutil gs sub1
```
Example output:
```
EventSource[0]:
Address: localhost
Enabled: true
Description: Subscription 1
Uri: wsman:microsoft/logrecord/sel
DeliveryMode: pull
DeliveryMaxSize: 16000
DeliveryMaxItems: 15
DeliveryMaxLatencyTime: 1000
HeartbeatInterval: 10000
Locale:
ContentFormat: renderedtext
LogFile: HardwareEvents
```
Display the runtime status of a subscription named sub1:
```
wecutil gr sub1
```
Update the subscription configuration named sub1 from a new XML file called WsSelRg2.xml:
```
wecutil ss sub1 /c:%Windir%\system32\WsSelRg2.xml
```
Update the subscription configuration named sub2 with multiple parameters:
```
wecutil ss sub2 /esa:myComputer /ese /un:uname /up:* /cm:Normal
```
Create a subscription to forward events from a Windows Vista Application event log of a remote computer at mySource.myDomain.com to the ForwardedEvents log (see Remarks for an example of a configuration file):
```
wecutil cs subscription.xml
```
Delete a subscription named sub1:
```
wecutil ds sub1
```

### Additional References

- [Command-Line Syntax Key](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/command-line-syntax-key.md)

---



MIT License. Copyright (c) 2020 Strontic.


