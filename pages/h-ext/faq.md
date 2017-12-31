---
title: H-Ext FAQ
permalink: /h-ext/faq.html
sidebar: h-ext_sidebar
keywords: frequently asked questions, FAQ, question and answer
toc: false
folder: h-ext
---

{% include note.html content="This page may will subject to change at any time to add/update/delete the FAQs." %}

<div class="panel-group" id="accordion">
{% capture answer_md %}
DZS OS SAPP is the first that provide open source base on our decision, plus it is only stable enough to maintenance for limit time. S-Ext is to provide a extension support for other developers, in order to expand third-parties flexibility without cause of conflict between the two.
{% endcapture %}
{% include faq_item.html index="1" answer=answer_md question="Why there's two re-branding change?" %}

{% capture answer_md %}
The founder & developer, DZS\|All-In-One, has ton of ideas which could not be done all in one day. We only take one at a time to ensure there are no issues with new feature. Basically, we cannot remove "Beta" until we are satisfied with all the features that is added to our Halo Extension along with Add-on interfaces needed to achieve the maximum possibilities for other developers to create their own Add-on easier.
{% endcapture %}
{% include faq_item.html index="2" answer=answer_md question="Why does H-Ext have \"Beta\" at the end?" %}

{% capture answer_md %}
We currently do not have a timeline for this, however when it has hit to 0.7.x or somewhere near before couple major update to its final version. We will inform the final release date, also after the final release we will be working on Add-ons that may have not been done or our hosts have higher demand request to have in their H-Ext product.
{% endcapture %}
{% include faq_item.html index="3" answer=answer_md question="When will it be out of of \"Beta\" version?" %}

{% capture answer_md %}
We have considered this and has done this in 0.1.4's open source. Then we later decided to establish it as limited source code which only be accessible through Add-on API. Although, after the 2 years of final version (starting from 1.0, not the version releases afterward) we will have it open source except for some closed source Add-on(s) relative to our server and it will be shut down as well for security purposes.
{% endcapture %}
{% include faq_item.html index="4" answer=answer_md question="Will it be open source?" %}

{% capture answer_md %}
You can easily find them on [Add-on API FAQ](/add-on%20api/faq.html) page.
{% endcapture %}
{% include faq_item.html index="5" answer=answer_md question="I have questions about the Add-on API and/or my future product, where can I find the answer(s)?" %}

{% capture answer_md %}
No, as result... the answer is always no. Why? All will have identical hooks and may or may not work correctly for any of them. This also includes how the developer's expectation to how it should work as well. Plus they all share same goal. H-Ext is an interface that avoid conflict between two product (Add-on) that need to listen on and allow the compatibility to work correctly.
{% endcapture %}
{% include faq_item.html index="6" answer=answer_md question="Will H-Ext or its formal names work with Gandanur, Phasor, Rec0, and/or SAPP?" %}

{% capture answer_md %}
Answer is always yes. We have dozens asking about this and inform them it can. However, some Add-on(s) may or may not work correctly if the halo servers are in the same directory. Please contact them to verify about their product.
{% endcapture %}
{% include faq_item.html index="7" answer=answer_md question="Will H-Ext able to work with 2 or more halo servers on same computer/server?" %}

{% capture answer_md %}
As usual, our formal expect to work with Halo PC and CE dedicated server. However we have opened our eyes to see Halo Trial does have its identical to PC and CE version due to the blam! engine only has minor changes. So we proceed with support both dedicated server and client. (NOTICE: We are entirely unsure about Halo OS, Open Sauce due to their developer may or may not add a hook cause some conflict with our hooks. Although, we will verify it before we release the first H-Ext.)
{% endcapture %}
{% include faq_item.html index="8" answer=answer_md question="What does H-Ext's expectation have?" %}

{% capture answer_md %}
It is expected to work with Halo Open Sauce and its newer releases, however they both will not be integrated since there are no interference with each other. ***NOTICE: This may subject to change if there are such interference.*** Also, there are some concerned with the additional feature which Halo Open Sauce should not be included as of 3.1 and possible later release. And suggestive to be separated instead of integrating into Halo Open Sauce. (Basically this is ideal to have H-Ext's Add-ons to manage it more better than break the support between two non-communication third-party software as usual.)
{% endcapture %}
{% include faq_item.html index="9" answer=answer_md question="Will it work with Halo Open Sauce (Modified Halo Custom Edition)?" %}

{% capture answer_md %}
Yes, we have worked with 2 developers (their name are concealed, yet is mentioned on some areas on the site) and gladly to assist them in any way we can. However, there is another developer that is actually marked as enemy which we will not work with him at all.
{% endcapture %}
{% include faq_item.html index="10" answer=answer_md question="Are you working with other known developers on Halo?" %}

{% capture answer_md %}
No, we will never abandon these projects. If we have done this, then it would not be very good for halo community's reputation. As for new features, if they have reached to its final stage, then it's a high chance will be a no. However, we may will consider add a plugin to a project that supports it.
{% endcapture %}
{% include faq_item.html index="11" answer=answer_md question="Will you abandon any of the projects that may contain some or major issues/bugs? What about new features?" %}

{% capture answer_md %}
Base on hearing from one of the hosting company complaint of its size, we are moving those features/commands into the Add-on which can be download separately. The H-Ext will be drop down to almost bare-bone while keep its flexibility, durable, and under controllable.
{% endcapture %}
{% include faq_item.html index="12" answer=answer_md question="I'm noticing most features/commands in H-Ext is gone, why?" %}

{% capture answer_md %}
Due to H-Ext have transform into PC game versions for both dedicated server and client, we decide not to include this in the main feature. Do not worry about this as we will bring back the GUI support in H-Ext 0.6 or later as seperate dll and will be load automatically if detect the halo is running as dedicated server AND the sgui.dll is in the dll folder. The client may will be using cgui.dll format. However we are still unsure how we should proceed with this yet. We will inform later when we get to 0.6 development plan.
{% endcapture %}
{% include faq_item.html index="13" answer=answer_md question="I noticed the GUI in S-Ext 0.4.x is not in H-Ext 0.5, why?" %}

{% capture answer_md %}
Absolutely **NOT**! We don't care what team did to modified the original Halo and redistribute it on the Internet. If we ever found out you are using it with our product, we will no longer helping you to have it working with your modified Halo at any time in the future. Use the ilegal way, find the official download site, such as microsoft, cnet, or halomaps.org website. Then use the cd key you have with it, we know it does work 100% with the original Halo distribute.
{% endcapture %}
{% include faq_item.html index="14" answer=answer_md question="Do you support crack Halo software?" %}

{% capture answer_md %}
Yes and no. Due to the price of Halo has NEVER been lowered, which is not an economically standard and being greedy for years now. Yes, Halo is a famous game ever happened to all of us. And we should not be punished for no price drop just like every other games does reduce their price. That would be the reasonabilty of yes. As for no reason, due to pirate copies around the Internet availability to download illegally. However, there are still hackers alternating their hash key which are likely known been used and still stated as legit keys. With the bypass of legit cd keys verified from GameSpy, it helps the server being more secure. Plus there are some players which is known around us that are using the same and/or pirated keys which does break the safety for the servers.
{% endcapture %}
{% include faq_item.html index="15" answer=answer_md question="Do you support crack Halo cd key?" %}

{% capture answer_md %}
Yes, since this can be done with EXTOnPlayerValidateConnect (May subject to change the name) from the Add-on API to determine if the player and/or admin is validated or not. Although, by default as of H-Ext (including S-Ext) it will still enforce the check with gamespy. (As for offline mode, we are still looking for method to have this supported with gamespy validate.)
{% endcapture %}
{% include faq_item.html index="16" answer=answer_md question="Since you are not fully support pirated Halo, is there still a way to allow pirate and/or same cd key in the server?" %}

{% capture answer_md %}
The list below are either likely or known incompatible with our H-Ext.
* Any of server modications such as Phasor, Gandanur, SAPP, etc.
* Version Changer by Omega (Goemitar)
* Halo Dev Control by jesus7freak (may will be official add-on for his' app to be included since we are very friendly.)
* Halo Anti-Cheat 2 (HAC2) NOTICED: Claimed it worked before and doesn't work so far at the moment.
* To be listed... (Will post more here and need reports what is not compatible from H-Ext users as well. Thank you)
{% endcapture %}
{% include faq_item.html index="17" answer=answer_md question="What are the third-party software incompatible with H-Ext?" %}

{% capture answer_md %}
Yes, you can use the "Contact Us" form on our halo's site and we will be gladly answer to any of your questions.
{% endcapture %}
{% include faq_item.html index="18" answer=answer_md question="Can I ask you any questions relative to H-Ext and its Add-ons?" %}

</div>
<!-- /.panel-group -->

{% include links.html %}
