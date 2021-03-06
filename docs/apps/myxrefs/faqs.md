---
title: FAQs
sidebarDepth: 2
approot: C:\Users\Username\AppData\Roaming\Autodesk\ApplicationPlugins\AVVAMyXrefs.bundle
---
# Frequently Asked Questions
[[toc]]

## App Installed Location :file_folder:
- The app files are installed to below location.
::: tip App Location 
{{$frontmatter.approot}}
:::

## 2022 Loading issue
There is an issue in Autodesk 2022 products which is not loading the arx files automatically.

[Custom ObjectARX not loaded on startup of Acad 2022.](https://forums.autodesk.com/t5/objectarx/custom-objectarx-not-loaded-on-startup-of-acad-2022/m-p/10687519#M41082)

Untill this issue is solved, please try below workaround to use this app.

- Download this [xml file](/PackageContents.xml)
- In windows explorer, goto the app installed folder
<code>{{$frontmatter.approot}}</code>
- Replace the <code>PackageContents.xml</code> file with the new file you downloaded.
- Now in AutoCAD, type <code>APPLOAD</code>
- In that window, click <code>Contents</code> button to open Startup suite
- In the startup suite click <code>Add</code> button and select <code>SQLiteLsp24x64.arx</code> from folder <code>{{$frontmatter.approot}}</code>\Contents\Windows\2021'
- close all the windows and Restart AutoCAD.
