# Overview     <img src="./Assets/Analogy128x128.jpg" align="right" width="155px" height="155px">
 Overview of projects and their repositories
 
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-reddit-red?logo=reddit)](https://reddit.com/submit?url=https://github.com/Analogy-LogViewer/Analogy.LogViewer&title=Analogy.LogViewer)
[![GitHub Repo stars](https://img.shields.io/badge/share%20on-hacker%20news-orange?logo=ycombinator)](https://news.ycombinator.com/submitlink?u=https://github.com/Analogy-LogViewer/Analogy.LogViewer)
[![GitHub Repo stars](https://img.shields.io/badge/share%20on-twitter-03A9F4?logo=twitter)](https://twitter.com/share?url=https://github.com/Analogy-LogViewer/Analogy.LogViewer&t=Analogy.LogViewer)
[![GitHub Repo stars](https://img.shields.io/badge/share%20on-facebook-1976D2?logo=facebook)](https://www.facebook.com/sharer/sharer.php?u=https://github.com/Analogy-LogViewer/Analogy.LogViewer)
[![GitHub Repo stars](https://img.shields.io/badge/share%20on-linkedin-3949AB?logo=linkedin)](https://www.linkedin.com/shareArticle?url=https://github.com/Analogy-LogViewer/Analogy.LogViewer&title=Analogy.LogViewer)

# Analogy Log Viewer

Analogy Log Viewer is multi purpose Log Viewer for Windows Operating systems (with built-in Parser for most commonly used log frameworks and file types).

The application has many standard operations for analysis logs (like filtering, excluding) but its strength is in the ability to add additional custom data sources by implementing few interfaces.
This allows adding any logs formats and/or custom modification of logs before presenting the data in the UI Layer.
Some features of this tool are:
1.	Windows event log support (evtx files)
2.	Logs aggregation into single view.
3.	Search in multiple files
4.	Combine multiple files
5.	Compare logs 
6.	Themes support
7.	64 bit support
8.	Personalization (users settings per user) 
9.	Columns extension to add more columns specific to the data source implementation
10.	Exporting to Excel/CSV files

# Log Viewer Application
The main Analogy Log Viewer app resides at the following repositories:
- [Analogy Log Viewer (DevExpress Version)](https://github.com/Analogy-LogViewer/Analogy.LogViewer)

You can create your own provider by basing it On the Example project: [Analogy.LogViewer.Example](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Example)

# Real Time Data Providers

Analogy Log Viewer has a Real time gRPC Data provider:

| Data Provider   |      CI Status      |  Nuget Version |
|----------|:---------------:|------|
| [gRPC Real Time Data Provider](https://github.com/Analogy-LogViewer/Analogy.LogViewer.gRPC) |![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.gRPC/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.gRPC)](https://www.nuget.org/packages/Analogy.LogViewer.gRPC/) 
| [Real Time AspNetCore Provider](https://github.com/Analogy-LogViewer/Analogy.AspNetCore.LogProvider/) | ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.AspNetCore.LogProvider/workflows/.NET%20Core%20Desktop/badge.svg)  | [![Nuget](https://img.shields.io/nuget/v/Analogy.AspNetCore.LogProvider)](https://www.nuget.org/packages/Analogy.AspNetCore.LogProvider) 
| [Real Time NLog Target](https://github.com/Analogy-LogViewer/Analogy.LogViewer.NLog.Targets) | ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.NLog.Targets/workflows/.NET%20Core%20Desktop/badge.svg)   | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.NLog.Targets)](https://www.nuget.org/packages/Analogy.LogViewer.NLog.Targets/) |
| [Real Time Serilog Sinks](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Serilog) |   ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Serilog/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.Serilog.Sinks)](https://www.nuget.org/packages/Analogy.LogViewer.Serilog.Sinks) |

## Real Time Client/Server

| Nuget/Repo   |      Version      |  Description |
|----------|:-------------:|------|
| [Analogy.LogServer](https://github.com/Analogy-LogViewer/Real-Time-Log-Server) |    | A windows Service for receiving logs 
| [Analogy.LogServer.Clients](https://www.nuget.org/packages/Analogy.LogServer.Clients/) |   [![Nuget](https://img.shields.io/nuget/v/Analogy.LogServer.Clients)](https://www.nuget.org/packages/Analogy.LogServer.Clients) | gRPC client to pull back messages from Analogy Service |

# Data Providers
The following custom data providers exists:
### Common Data providers:
| Data Provider   |      CI Status      |  Nuget Version |
|----------|:---------------:|------|
| [Serilog Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Serilog) |  ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Serilog/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.Serilog)](https://www.nuget.org/packages/Analogy.LogViewer.Serilog/)
| [NLog Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.NLogProvider)|  ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.NLog/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.NLogProvider)](https://www.nuget.org/packages/Analogy.LogViewer.NLogProvider/) 
| [Log4Net Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Log4Net) |  ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Log4Net/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.Log4Net)](https://www.nuget.org/packages/Analogy.LogViewer.Log4Net/)
| [Log4jXml Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Log4jXml) |  [![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Log4jXml/actions/workflows/dotnet-core-desktop.yml/badge.svg)](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Log4jXml/actions/workflows/dotnet-core-desktop.yml) |  [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.Log4jxml)](https://www.nuget.org/packages/Analogy.LogViewer.Log4jxml/)
| [Regular Expression Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.RegexParser)| ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.RegexParser/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.RegexParser)](https://www.nuget.org/packages/Analogy.LogViewer.RegexParser/)
| [Plain Text Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.PlainTextParser) | ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.PlainTextParser/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.PlainTextParser)](https://www.nuget.org/packages/Analogy.LogViewer.PlainTextParser/)
| [Json Log Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.JsonParser)| ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.JsonParser/workflows/.NET%20Core%20Desktop/badge.svg) |[![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.JsonParser)](https://www.nuget.org/packages/Analogy.LogViewer.JsonParser/)
| [XML Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.XMLFileProvider)| ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.XMLParser/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.XMLParser)](https://www.nuget.org/packages/Analogy.LogViewer.XMLParser/)
| [IIS log Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.IISLogParser)| ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.IISLogsProvider/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.IISLogsProvider)](https://www.nuget.org/packages/Analogy.LogViewer.IISLogsProvider/)
| [Windows event logs](https://github.com/Analogy-LogViewer/Analogy.LogViewer.WindowsEventLogs)| ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.WindowsEventLogs/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.WindowsEventLogs)](https://www.nuget.org/packages/Analogy.LogViewer.WindowsEventLogs/)


### Special Purpose Data providers:
| Data Provider   |      CI Status      |  Nuget Version |
|----------|:---------------:|------|
| [Real Time Log Server](https://github.com/Analogy-LogViewer/Real-Time-Log-Server) | ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Real-Time-Log-Server/workflows/.NET%20Core%20Desktop/badge.svg)   | 
| [Git History](https://github.com/Analogy-LogViewer/Analogy.LogViewer.GitHistory) | ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.GitHistory/workflows/.NET%20Core%20Desktop/badge.svg)  | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.GitHistory)](https://www.nuget.org/packages/Analogy.LogViewer.GitHistory/)
| [GitHub repositories info](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Github) |![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Github/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.Github)](https://www.nuget.org/packages/Analogy.LogViewer.Github/)
| [Microsoft PowerToys Log Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.PowerToys) |  ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.PowerToys/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.PowerToys)](https://www.nuget.org/packages/Analogy.LogViewer.PowerToys/)
| [Words Search](https://github.com/Analogy-LogViewer/Analogy.LogViewer.WordsSearch)| ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.WordsSearch/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.WordsSearch)](https://www.nuget.org/packages/Analogy.LogViewer.WordsSearch/)
| [Kafka Producer/ consumer](https://github.com/Analogy-LogViewer/Analogy.LogViewer.KafkaProvider)| ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.KafkaProvider/workflows/.NET%20Core%20Desktop/badge.svg) |[![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.KafkaProvider)](https://www.nuget.org/packages/Analogy.LogViewer.KafkaProvider/)
| [Sqlite SB Browser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Sqlite)| ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Sqlite/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.Sqlite)](https://www.nuget.org/packages/Analogy.LogViewer.Sqlite/)
| [Example project](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Example) | ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Example/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.Example)](https://www.nuget.org/packages/Analogy.LogViewer.Example/) 

### Organizations/Companies Data providers:
| Data Provider   |      CI Status      |
|----------|:---------------:|
| [Kama Research and Development](https://github.com/Analogy-LogViewer/Analogy.LogViewer.KamaResearch) |  ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.KamaResearch/workflows/.NET%20Core%20Desktop/badge.svg) 
| [Philips I4 BU](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Philips.I4) 
| [Philips ICAP BU](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Philips.ICAP)  | 
| [MIrada XD logs Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.MiradaXD) | 

### Obsolete Data providers:
| Data Provider   |      CI Status      |
|----------|:---------------:|
| [Kama Research and Development](https://github.com/Analogy-LogViewer/Analogy.LogViewer.KamaResearch) |  ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.KamaResearch/workflows/.NET%20Core%20Desktop/badge.svg) 
| [Philips I4 BU](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Philips.I4) 
| [Philips ICAP BU](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Philips.ICAP)  | 
| [MIrada XD logs Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.MiradaXD) | 
| [RabbitMq Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.RabbitMq) |  ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.RabbitMq/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.RabbitMq)](https://www.nuget.org/packages/Analogy.LogViewer.RabbitMq/)
| [Catel log Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.CatelProject) 
| [RSS Reader](https://github.com/Analogy-LogViewer/Analogy.LogViewer.RSSReader) | ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.RSSReader/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.RSSReader)](https://www.nuget.org/packages/Analogy.LogViewer.RSSReader/)
| [WCF Sender/Receiver](https://github.com/Analogy-LogViewer/Analogy.LogViewer.WCF) | ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.WCF/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.WCF)](https://www.nuget.org/packages/Analogy.LogViewer.WCF/)
| [WhatsApp Chat Log Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.WhatsApp) | ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.WhatsApp/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.WhatsApp)](https://www.nuget.org/packages/Analogy.LogViewer.WhatsApp/)
| [Visual Studio Activity Log Parser](https://github.com/Analogy-LogViewer/Analogy.LogViewer.VisualStudioLogParser) | ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.VisualStudioLogParser/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.VisualStudioLogParser)](https://www.nuget.org/packages/Analogy.LogViewer.VisualStudioLogParser/)

# Core Repositories

| Data Provider   |      CI Status      |  Nuget Version |
|----------|:---------------:|------|
| [Analogy Interface Project](https://github.com/Analogy-LogViewer/Analogy.Interfaces) | ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.Interfaces/workflows/.NET%20Core%20Desktop/badge.svg) | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.Interfaces)](https://www.nuget.org/packages/Analogy.LogViewer.Interfaces/) 
| [Analogy Template/Base Project](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Template) | ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.LogViewer.Template/workflows/.NET%20Core%20Desktop/badge.svg)  | [![Nuget](https://img.shields.io/nuget/v/Analogy.LogViewer.Template)](https://www.nuget.org/packages/Analogy.LogViewer.Template/) 
| [Analogy Common Utilities](https://github.com/Analogy-LogViewer/Analogy.CommonUtilities) | ![.NET Core Desktop](https://github.com/Analogy-LogViewer/Analogy.CommonUtilities/workflows/.NET%20Core%20Desktop/badge.svg)  | [![Nuget](https://img.shields.io/nuget/v/Analogy.CommonUtilities)](https://www.nuget.org/packages/Analogy.CommonUtilities/) 

# Dependencies & Build
- Main Application UI is complied to .Net Framework 4.7.2 and to .Net Core 3.1. The supported version of Visual studio for this framework is Visual studio 2017 (or above).
After successfull build any custom data source assemblies should be placed at the same folder as the executable (Analogy.exe) with the folowing pattern naming: Analogy.LogViewer.*.dll
- Analogy Interfaces assembly is complied to .Net Standard 2.0.

- DevExpress User Controls:
in order to compile the DevExpress version  [DevExpress](https://www.devexpress.com/) assemblies are required (winforms package only).




<a name="contact"></a>
## Contact

### Owner
- [Lior Banai](mailto:liorbanai@gmail.com)
