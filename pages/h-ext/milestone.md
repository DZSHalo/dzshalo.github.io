---
title: Milestone | H-Ext
sidebar: h-ext_sidebar
permalink: /h-ext/milestone.html
folder: h-ext
---

## Versions Planned

{% capture v0_0 %}
* The very first development initiative and very primate base progress.
* Learning how to trace and very little asm language coding. Also first time using C++ language as well.
* Fixing the SuperAbyll  mistakes into better stability.
* Using dirty files due to not enough knowledge with how to use Microsoft database file handler.
{% endcapture %}
{% capture v0_1 %}
* Internal Database support (native mdb file similar to rec0 usage except for administrator system)
* First time added AdminBot feature (please visit the wiki site to review the commands with description provided).
* Mainly redirected most functions to extension.exe instead inside Halo Dedicated Server for safety reasons.
{% endcapture %}
{% capture v0_2 %}
* Internal Database support (native mdb file similar to rec0 usage except for administrator system)
* First time added AdminBot feature (please visit the wiki site to review the commands with description provided).
* Mainly redirected most functions to extension.exe instead inside Halo Dedicated Server for safety reasons.
{% endcapture %}
{% capture v0_3 %}
* Mainly focus on Add-on API in order to freely distribution by other developers to create plugins to be used in S-Ext.
* Player records featured to track names, ips, and ports per CD Key hash.
{% endcapture %}
{% capture v0_4 %}
* No longer using two separate windows and replaced to one better GUI console (see next line below). 
* Redesign the console into more simpler GUI console to permit local hosts to be able control the server easier. (Will be constant redesign until meet suitable needs.)
* Planned for Official Updater ~~and Remote Control~~ Add-on feature.
* Some has been transferred into Halo console for stability and some are redirected for more controls.
{% endcapture %}
{% capture v0_5 %}
* For such example, killall command would say "It's quite bit too quiet in here tbh" which you can change to "It's deserted in here...where did everyone go?" or something similar.
* Officially will be integrated into Halo's process instead of separate process.
* ~~Will be toggle-ability to switch from halo console to basic/advance GUI console which will be using halo console by default.~~ (Will not be supportive and will be transfer to as extended add-on api support.)
* More hooks for more control of every possible activities relate to player and such. (Will be listed more later or use the task list on 0.5.0 ticket made.)
* Will be using code scanning to support all Halo Trial, PC, and CE versions (this includes the missing 1.02, 1.03, 1.06, and such except for Trial never has been updated).
* WILL be made from scratch, aka version 3 coding, which will generally using native C language without any std classes as possible. This also includes removing all unnecessary functions, reducing memory usage for other purposes, more custom classes support, native installation. (This will means all role-play commands will be separated and no longer built-in.)
* Dynamic Stack Vector class. (We had a very new idea how to replace a massive std::vector into much smaller class!) 
* NOTICE: Due to new introduction of install the H-Ext product, it will no longer need a patcher at all which then reduce the steps into simple 1 step. More information can be found in [install page](/h-ext/install.html).
* NOTICE: This will be strip down to barebone only. Most commands you are looking for will be in separate Add-on which will be release later.
* At least add support send to and receive from client/server's communication in order permit H-Ext's clients and hosts to communicate each other more friendly. (This will hook into the Halo's communication and will be using the standard UDP protocol and the host/clients port is/are using.)
{% endcapture %}
{% capture v0_5_3 %}
* Include 0.5 task-list above.
* Major re-work on Add-on API to fix ton of issues that are not following C-99 standard and several other issues of managed code refuse to work correctly.
* Compatible issue with Trial, Combat Evolved, and Custom Edition will be re-verify. **(After Add-on API and hooks are fully done.)**
* At least get more static message into message.ini file from H-Ext product.
* Re-define possibility to use custom message relative to player and some other things. **(If possible before moving to 0.6 task-list.)**
* More bug fixing from time to time. (If reported...)
{% endcapture %}
{% capture v0_6 %}
* Everything from 0.4's GUI will be back for dedicated server and continue make compatible.**
* DirectX GUI for client of extended menu support.**
* Fix and improved chat system with few options support. (Will be in client's API integration, unload the H-Ext will restore the chat system originally. Keep this in mind before start complaint about the same original chat bug as it has been for years.)
* Client & Server GUI will be access directly from H-Ext as H-Ext will load the correct Client/Server API dll to generate a GUI for the addon to use more friendly.
* If possible, convert the client's rcon and console into unicode instead of ASCII format. (Server's standard console will be re-written to unicode and at least format it automatically to view the unicode correctly. And if append a '-gui' for the server, will be using the H-Ext's GUI console.)
* (Not sure what else to put in here)

  * (Notice: All Add-ons are required to use this interface! Only if the add-on is using the GUI and keyboard listener.)
{% endcapture %}
{% capture v1_0 %}
* Fully and featured support that is 100% working condition, no other details needed.
{% endcapture %}

| 0.x Versions | Basic Concept |
| --- | --- |
| (0.0, Unknown) | First started from SuperAbyll open source draft from Internet. {::nomarkdown}{{ v0_0 | markdownify | strip_newlines }}{:/} |
| (0.1, Grunt) | Recognize as showing supportive stable release. {::nomarkdown}{{ v0_1 | markdownify | strip_newlines }}{:/} |
| (0.2, Jackal) | Mainly separate all exceptions into separate executable for allowing the native Halo Dedicated Server to continue running with auto restart (which eventually did not capture all exceptions by itself). {::nomarkdown}{{ v0_2 | markdownify | strip_newlines }}{:/} |
| (0.3, Elite) | Add-on API development + others {::nomarkdown}{{ v0_3 | markdownify | strip_newlines }}{:/} |
| (0.4, Brute) | GUI features {::nomarkdown}{{ v0_4 | markdownify | strip_newlines }}{:/} |
| (0.5, Drone) | Fully customizable message list instead of using standard usage and integrated to Halo Dedicated Server ***and Client with all game versions support and expected to work all updated versions*** with better improvement performance. {::nomarkdown}{{ v0_5 | markdownify | strip_newlines }}{:/} |
| (0.5.3+, Drone Engineer) | Major re-work of Add-on API to work with major code languages support. {::nomarkdown}{{ v0_5_3 | markdownify | strip_newlines }}{:/} |
| (0.6, Hunter) | GUI features (returned) {::nomarkdown}{{ v0_6 | markdownify | strip_newlines }}{:/} |
| (0.7, Engineer) | Reserved if needed. |
| (0.8, Prophet) | Reserved if needed. |
| ... | |
| (1.0, Forerunner) | Final and completed Version {::nomarkdown}{{ v1_0 | markdownify | strip_newlines }}{:/} |

{% include links.html %}
