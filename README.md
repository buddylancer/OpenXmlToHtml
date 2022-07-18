# OpenXmlToHtml

Converts docx to html

[![Nuget](https://img.shields.io/nuget/v/Codeuctivity.HtmlRenderer.svg)](https://www.nuget.org/packages/Codeuctivity.HtmlRenderer) [![Build](https://github.com/Codeuctivity/OpenXmlToHtml/actions/workflows/dotnet.yml/badge.svg)](https://github.com/Codeuctivity/OpenXmlToHtml/actions/workflows/dotnet.yml)

- .net implementation
- No external infrastructure needed (No Microsoft Office or Libre Office needed)
- Focused on Windows and Linux support
- Demo CLI Api [OpenXmlToHtmlCli.zip](https://github.com/Codeuctivity/OpenXmlToHtml/releases)
- Azure [Demo Open Api](http://openxmlconverter.azurewebsites.net/index.html) (running on limited budget... may be offline after usage quota exceeds)

```c#
await OpenXmlToHtml.ConvertToHtmlAsync(inputPathDocx, outputPathHtml);
```

## Fonts and Linux - WIP Section

Some windows specific fonts used in many docx can be installed on linux using

```bash
sudo apt install ttf-mscorefonts-installer -y && sudo fc-cache -vr
```
