---
title: Add-on API
tags: [getting_started]
sidebar: add-on_api_sidebar
permalink: /add-on api/index.html
folder: add-on api
---

Ever since the beginning of the Add-on API, the following 4 standard requirement, see below, for initializing a plugin.

*NOTICE: This is updated for Add-on API 4.0.*

The following definition to this date are supported:
```c
EXT_ICINIFILE
EXT_IDATABASE
EXT_IDATABASESTATEMENT
EXT_HKDATABASE (Required EXT_IDATABASE and EXT_IDATABASESTATEMENT)
EXT_IOBJECT
EXT_IEXTERNAL
EXT_IHALOENGINE
EXT_IOBJECT
EXT_IPLAYER
EXT_ICOMMAND
EXT_ITIMER (Required EXT_HKTIMER)
EXT_HKTIMER (Required EXT_ITIMER)
EXT_IADMIN
```
To create an Add-on, you need to provide information in addon_info structure:
```c
addon_info EXTPluginInfo = { L"Your Plugin Name", //Plugin Name
			L"1.0.0.0", //Version
			L"Author", //Your name
			L"Simple description of what it does.", //Description
			L"Config folder", //Preferred configuration folder to be used for this plugin. (For ICIniFile interface usage)
			NULL, //Sector1 (Sector 1-5 is used for import the commands level from commands.ini
			NULL, //Sector2
			NULL, //Sector3
			NULL, //Sector4
			NULL};//Sector5
```
Then you need to provide the load and unload functions. Since it is variety in different language, I will provide standard parameter and return expectation. You can also look at UnitTest's source codes too.
```
EAO_RETURN EXTOnEAOLoad(unsigned int hash) {
	// do whatever you need to initialize your plugin such as load settings, start functions need to check up, etc.
	// Including the commands to be append with our command listener system.
	return EAOCONTINUE; //Look in Add-on API.h's EAO_RETURN enum for all supported values.
}

void EXTOnEAOUnload(void) {
	// do whatever you need to stop your plugin such as save settings, end functions need to check up, etc.
	// Including to remove all of command from our command listener system. (May subject to change for self remove commands.)
}
```
Once you have compile your Add-on, you need to use Add-on Converter application in order for Halo Extension to load your Add-on. Add-on Converter will validate your definition, hooks, etc, then convert it. You will find converted file in the same directory where you compiled it.

Have questions? Please use the [Add-on API FAQ](faq.html) page before contacting us.

For complete list of events from native Halo, please go to [events section](events.html).

For complete list of Database API functions needed, please go to [Database API section](database_api.html).

For complete list of Console API functions needed, please go to [Console API section](console_api.html).

For complete list of Timer API functions needed, please go to [Timer API section](timer_api.html).

{% include links.html %}
