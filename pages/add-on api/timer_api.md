---
title: Timer | Add-on API
keywords: api
sidebar: add-on_api_sidebar
permalink: /add-on api/timer_api.html
folder: add-on api
tags: [api]
---

*First support is: H-Ext 0.5.2.2 (Add-on API 3.1.1 to 3.1.2)*

*Supported: H-Ext 0.5.3.4 (Add-on API 4.0) or newer*

To register the Timer support, the following below is required to be exported with `#define EXT_ITIMER` and `#define EXT_HKTIMER` before including the header of Add-on API. Also require you to manage your own stacks with the idTimer. This provide you more independent of what kind of parameters/structure to use. It is recommended to keep the idTimer included.

```c
CNATIVE dllAPI bool WINAPIC EXTOnTimerExecute(unsigned int idTimer, unsigned int counter) {
   //...
   return 0; //Tell H-Ext not to repeat timer. Or use 1, true, for repeat request.
}
CNATIVE dllAPI void WINAPIC EXTOnTimerCancel(unsigned int idTimer) {
   //...
}
```

{% include links.html %}
