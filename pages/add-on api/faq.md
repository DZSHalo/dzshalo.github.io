---
title: Add-on API FAQ
permalink: /add-on api/faq.html
sidebar: add-on_api_sidebar
keywords: frequently asked questions, FAQ, question and answer
toc: false
folder: add-on api
---

{% include note.html content="This page may will subject to change at any time to add/update/delete the FAQs." %}

<div class="panel-group" id="accordion">

{% capture answer_md %}
You can determine this check through the load process with the haloEngine class and return of value which can't be load at all.
{% endcapture %}
{% include faq_item.html index="1" answer=answer_md question="What if I do not want my Add-on support Halo Trial, PC, and/or CE?" %}

{% capture answer_md %}
Also included with the haloEngine class.
{% endcapture %}
{% include faq_item.html index="2" answer=answer_md question="What about the detect if it is a dedicated server or a client version?" %}

{% capture answer_md %}
At this time, no.  If request to have your own admin API management, then please inform us and we will create one for it.
{% endcapture %}
{% include faq_item.html index="3" answer=answer_md question="Can I use my own admin API management?" %}

{% capture answer_md %}
Yes, H-Ext will allow only one override the default database management.
{% include tip.html content="Hint, if determined to use MySQL or shared database, then two or more H-Ext can be use synchronizing information." %}
{% endcapture %}
{% include faq_item.html index="4" answer=answer_md question="Can I create or use another Add-on for a database management?" %}

{% capture answer_md %}
Please use the ticket system to make the request feature. And do be aware of one manned programmer with mid-skilled of reverse engineering will take time. Along with other Add-ons, he has to develop support mainly for the role-playing. Although, he is now focusing on 0.x's version plan task.
{% endcapture %}
{% include faq_item.html index="5" answer=answer_md question="There are missing features in Add-on API, where can I report at?" %}

{% capture answer_md %}
Please do provide the information so we can make the missing event/feature more quicker instead of much longer delays or likely unable to provide the feature to you and others. We can use that information to verified it is at the correct location and gather the correct information for all PC game versions supportive.
{% endcapture %}
{% include faq_item.html index="6" answer=answer_md question="What if I found the location for the missing feature to be hook at?" %}

{% capture answer_md %}
Use the ticket system to make the bug report, we will keep this in check if this have occurs base on the Trial, PC, and/or CE versions. And please do report in every details as possible or otherwise we can't fix what you are stating the issue is.
{% include important.html content="Other modified Halo will not be checked as it is not recommended to alternate." %}
{% endcapture %}
{% include faq_item.html index="7" answer=answer_md question="Something odd going on with the events from the Add-on API, where can I report this bug/glitch?" %}

{% capture answer_md %}
No, we supplies the all of available hooks at the moment of which the Add-on can use. Meaning you can create almost anything you want with it.
{% endcapture %}
{% include faq_item.html index="8" answer=answer_md question="Am I required to have knowledge with reverse engineering?" %}

{% capture answer_md %}
Absolutely! This is one part of our goal to resolve the conflict of multiple third party required to listen for user's command.
{% endcapture %}
{% include faq_item.html index="9" answer=answer_md question="Can I register a command for players to use?" %}

{% capture answer_md %}
Depending on the command that has registered with the command system. Some would allow to be overriden, some wouldn't permit. However, only one overriden command is permitted per command.
{% endcapture %}
{% include faq_item.html index="10" answer=answer_md question="I want to override a command, is this possible?" %}

{% capture answer_md %}
As of Add-on API v4.0 and newer, it is now supported for C, C++, D, C#, and Visual Basic languages. If any of supported languages is not one of your language you want to use. Please verify your language has ability to compile into Windows dll module. Otherwise it is not compatible.
{% include note.html content="If it, then please create a ticket. Or recreate Add-on API in your code language then make a pull request to include support." %}
{% include warning.html content="You must verify each APIs are fully functional before we can merge your pull request." %}
{% endcapture %}
{% include faq_item.html index="11" answer=answer_md question="I want to make an Add-on other than C/C++ language, is this possible?" %}


</div>
<!-- /.panel-group -->

{% include links.html %}
