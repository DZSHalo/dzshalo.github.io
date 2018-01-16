---
title: Halo Extension
sidebar: h-ext_sidebar
permalink: /h-ext/index.html
folder: h-ext
---

For more information about developing a plugin, please visit [Add-on API section](/add-on%20api/index.html).

Welcome to our project tracking site, this site will be likely update before every release to keep everything up-to-date from bug fixes to new features. Starting with 0.4.0 release celebration this wiki project tracking will be used as main wiki site instead of our old wiki site. Please do enjoy viewing what you are looking or learn more about Halo Extension and what it can do.

We have determined to separate the each category into its own page with quicker update individually.  Please notice this will **NOT** include the plugin(s) update including the [Add-on API](/add-on api/index.html) which is on separate project yet is embedded with S-Ext versions from 0.3.0 - 0.4.2.2, and H-Ext version froms 0.5.0 and above.

To view the current up-to-date change log for all releases, please use this [change log link](changelog.html) instead of our old wiki site.

Curiously what Halo's commands are being overriden by H-Ext? Click [here](commands.html) to find out!

Got questions? Please visit our [FAQ page](faq.html) first before contacting us.

We have included the [Halo Netcode](halo_netcode.html) page of what does and does not sync base on Halo's netcode.

## System Requirement

| Requirement | Minimum | Recommended | Confirmed? |
| --- | --- | --- | --- |
| Operating System | Windows XP SP1 / Windows Server 2003 SP1 | Windows XP SP1 or higher / Windows Server 2003 SP1 or higher | YES |
| Processor | 733MHz | 1.4GHz or higher | Unknown, not tested yet. |
| Memory (RAM) | 128 MB + 10 MB or more | 128 MB + 50 MB or more (for plugin spaces to use) | YES |
| Screen Resolution | 800x640 | 800x640 or higher | YES |
| Graphic Card | 32MB | 32MB or more | Unknown, not tested yet. |
| DirectX | None (dedicated server) | 9.0c (client requirement) | YES |

## Compatibility for Halo

{% capture note_os_render %}We do not "support" Open Sauce's third-party integrations as we will be appending the hooks to allow other developers to create their own instead of third-party integrations if they preferred so. Or other Halo users do not want this included with their Halo.{% endcapture %}
{% capture note_os %}{% include note.html content=note_os_render %}{% endcapture %}
{% capture note_untested_render %}Halo versions below 1.10 are not fully tested.{% endcapture %}
{% capture note_untested %}{% include warning.html content=note_untested_render %}{% endcapture %}


| H-Ext Version | Halo Trial | Halo PC | Halo CE | Halo OS
| --- | --- | --- | --- | --- |
| (DZS OS SAPP)<br/>0.1.0 - 0.1.4 | --- | --- | 1.09 Dedi | Unknown |
| (S-Ext)<br/>0.2.0 - 0.4.2.2 | --- | --- | 1.00, 1.07-1.09 Dedi | 3.x & 4.x **(Please note the map commands will not work correctly for yelo maps, use the native halo command as a workaround)** |
| (H-Ext)<br/>0.5.0 - 0.5.1.2 | ALL | 1.00 - 1.09 | 1.00-1.09 |3.x & 4.x {::nomarkdown}{{ note_os | markdownify | strip_newlines }}{:/} |
| (H-Ext)<br/>0.5.2.2 - 0.5.2.4 | Partial | 1.03 - 1.10 | ALL | 3.x & 4.x {::nomarkdown}{{ note_os | markdownify | strip_newlines }}{:/} |
| (H-Ext)<br/>0.5.3.4 - ? | Partial | Untested | Untested | 3.x & 4.x {::nomarkdown}{{ note_os | markdownify | strip_newlines }}{:/} {::nomarkdown}{{ note_untested | markdownify | strip_newlines }}{:/} |



More coming soon...

{% include links.html %}
