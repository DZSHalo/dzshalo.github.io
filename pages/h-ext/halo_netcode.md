---
title: Halo Netcode
sidebar: h-ext_sidebar
permalink: /h-ext/halo_netcode.html
folder: h-ext
---

{% include note.html content="We have ''NOT'' implement the custom netcode ''yet''." %}

Keep in reminder, the listed below are ''just'' for halo management only. We will perform some syncs for listed below to work with either halo's netcode or custom netcode.

## Vehicle Section

| function | Player sync? | AI sync? | Comment |
|---|---|---|---|
| enter | YES | NO | Might will have a workaround for this. |
| exit | YES | NO? | Has not verified for AI. |

## Biped Section

| function | Player sync? | AI sync? | Comment |
|---|---|---|---|
| flashlight | PARTIAL | Unconfirmed | Noticed player claimed flash light is off but most players can see flashlight is still on. (Flashlight toggle may be incorrect or loss of packet data.) |

## Object Section

| function | Sync? | Comment |
|---|---|---|
| created | Player: YES<br/>AI: PARTIAL<br/>Scenery: PARTIAL<br/>Vehicle: YES<br/>Weapon: YES<br/>Gametype Object: YES | Has not verified for AI and Scenery. |
| deleted | Player: PARTIAL<br/>AI: NO<br/>Scenery: NO<br/>Vehicle: YES<br/>Weapon: YES<br/>Gametype Object: YES | Has not verified for AI and Scenery. |
| update | Player: YES<br/>AI: NO<br/>Scenery: NO<br/>Vehicle: YES<br/>Weapon: YES<br/>Gametype Object: YES | Some claim players are able to warp around the map. |
| camouflage | Player: YES<br/>AI: NO<br/>Scenery: NO<br/>Vehicle: NO<br/>Weapon: NO<br/>Gametype Object: NO | Camouflage is only setup for players base on halo's code. Will need to perform separate netcode packet in order to sync. |

## AI Section

Including above sections

| function | Sync? | Comment |
|---|---|---|
| position | NO | Confirmed with other players. |
| action | NO | Does not sync AI shooting at specific player or other AI along with other things. |
| death | PARTIAL | Never has revealed death even when it occurred. |

{% include note.html content="This page may subject to change at ''ANY'' time." %}

{% include links.html %}
