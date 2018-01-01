---
title: How to use the Add-on API? | Add-on API
keywords: api
sidebar: add-on_api_sidebar
permalink: /add-on api/how-to_setup.html
folder: add-on api
tags: [how-to,getting_started]
---

We made it very simple to use. Just follow this chart of directory to make things easier for you!


| Root or subdirectory | directory | files |
|---|---|---|
| C:\ or C:\H-Ext Apps\ or any directory you preferred | Add-on API | all folders and files of Add-on API goes here |
| (same as above) | Plugin 1 | all files of plugin 1 goes here |
| (same as above) | Plugin 2 | all files of plugin 2 goes here |
| (same as above) | Plugin 3 | all files of plugin 3 goes here |
| (same as above) | etc | etc |

Then the next thing you need to do is insert the include these method
```
#pragma comment(lib, "../Add-on API/Add-on API.lib")
#include "..\Add-on API\Add-on API.h"
```
into your main source file or a main header.

Then you will need to determine which interfaces you will be using by declaring as an example:
```c
#define EXT_IHALOENGINE
```
which means you are using the pIHaloEngine class in your plugin and will be reveal to you. Do the same for other defined EXT_ if needed to.

Anything else to do next? Nope, just start programming! If you cannot find a name in a class or structure, then look in the origin of the file contain this or use a helper built-in Visual Studio.

We recently added another header file called expChecker.h which allows you to put at end of a main source file.
```c
#include "..\Add-on API\expChecker.h"
```
This way, it will help the plugin developers to determine they have correct exported functions and/or need a fix before they could release unstable build.

{% include links.html %}
