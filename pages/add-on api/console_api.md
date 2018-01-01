---
title: Console | Add-on API
keywords: api
sidebar: add-on_api_sidebar
permalink: /add-on api/console_api.html
folder: add-on api
tags: [api]
---

{% include warning.html content="Currently on hold. Console feature will return later on." %}

{% comment %}
Very simple integration for ability to retrieved the output from console and send to another location plus possibility of more features for expansion if needed.

{% include warning.html content="This is currently in draft for development of H-Ext 0.4.0." %}

{% include warning.html content="This is subject to change at ANY time until it is fully feature." %}

```c
extern "C" __declspec(dllexport) bool EXTHookConsole() {
	return true;
}
extern "C" __declspec(dllexport) void EXTOnConsoleOutput(wchar_t outputData[]) {
}
```
{% endcomment %}

{% include links.html %}
