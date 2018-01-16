---
title: Program Language Support | Add-on API
keywords: api
sidebar: add-on_api_sidebar
permalink: /add-on api/program_language_support.html
folder: add-on api
tags: [api]
---

The following coding language support are:
* C
* C++
* C# **
* D
* Visual Basic **

Currently not supported are:
* F# ***
* (Know a coding language support to compile as Windows' dll module and support C standard language? Let us know!)

Be aware coding languages using .NET Framework or in other term of managed code method do require a wrapper which takes more time to complete than unmanaged code. Plus is still under experimental stage for the wrapper itself. Add-on API hooks and interfaces are currently under full C language support.

{% include note.html content="** Language is a managed code which uses .NET Framework. Therefore do require to use UnmanagedExports extension in order to work properly. Otherwise H-Ext will not be able to communicate with managed Add-on software." %}
{% include note.html content="Add-ons with .NET Framework does not support unload process internally for time being. Please restart halo in order to take effect." %}
{% include note.html content="*** There is no Add-on API language support for it. However do has ability to include support." %}

{% include links.html %}
