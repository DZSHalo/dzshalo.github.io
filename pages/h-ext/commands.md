---
title: Commands | H-Ext
sidebar: h-ext_sidebar
permalink: /h-ext/commands.html
folder: h-ext
toc: false
datatable: true
---

## Commands

<div class="datatable-begin"></div>

| Released | Command | Description | Deprecated Reason |
| --- | --- | --- | --- |
| ? - (Current) | ext_about | To see information about the H-Ext. | (none) |
| ? - (Current) | ext_admin_add (player_express/CDHash) (username) (password) (level) [remote] [temp_pass_force] | Permit hoster and/or higher level administrator with access to add administrator to the list. | (none) |
| ? - (Current) | ext_admin_del (index ID / username) | Ability to remove an administrator from the list permanently. | (none) |
| ? - (Current) | ext_admin_list [page_number] | List of all admins stored in the database. (Finally supportive!) | (none) |
| ? - (Current) | ext_admin_online | List of all admins online. (ingame only, remote will be support later) | (none) |
| ? - (Current) | ext_admin_update (index ID / username) (user / pass / level / ip / port / remote / temp_pass / hash) (your_input_here) | Ability to modify the administrator from the list. | (none) |
| ? - (Current) | ext_admin_sync | Allow the administrator to sync their IP Address and IP Port into the administrator list (similar to update) | (none) |
| ? - (Current) | ext_admin_requirement (login:boolean) (IP_Address:boolean) (IP_Port:boolean) | To enforce match requirement against the administrator list to determine is authorized or not. | (none) |
| ? - (Current) | ext_admin_requirement_login (IP_Address:boolean) (IP_Port:boolean) | Given administrator login enforcement to included the verify check security (the higher it is, the more chance administrator unable to login). | (none) |
| ? - (Current) | ext_admin_login (username:string) (password:string) | This allows the administrators to login just in case if the system does not recognize or not match the required qualification to recognize an administrator in-game. | (none) |
| ? - (Current) | ext_admin_password_change (current_password:string) (new_password:string) | Gives the opportunity for any level administrator to change their own password, even temporary password. | (none) |
| ? - (Current) | ext_admin_unlimit_level [0-9999] | To permit specific level and above to access every commands. (Default: 9999) | (none) |
| ? - (Current) | ext_rcon_admin_level [-1 - 9999] | Permit admins to use the rcon execute restriction. (Default: -1) | (none) |
| ? - (Current) | ext_rcon_admin_pass_enable [boolean] | To permit the admins to use their own password to execute the rcon command. (Default: true) | (none) |
| ? - (Current) | ext_rcon_pass_bad_disable [boolean] | If the password is wrong, it will return "bad password". As for extra protection, can enforce to "password is disabled" message return. (Default: false) | (none) |
| ? - (Current) | ext_addon_load (file_name) | Load a plugin file into Halo's memory. | (none) |
| ? - (Current) | ext_addon_unload (file_name) | Unload a plugin file from Halo's memory. | (none) |
| ? - (Current) | ext_addon_unload_all | Unload all of the active plugins from Halo's memory. | (none) |
| ? - (Current) | ext_addon_list [page_number] | To list of all active plugins. | (none) |
| ? - (Current) | ext_func_alias (func_name / alias_name ) | To see shorter name(s) for the function. | (none) |
| ? - (Current) | ext_func_alias_add (func_name) (alias_name) | Add a shorter name for the function. | (none) |
| ? - (Current) | ext_func_alias_del (func_name) (alias_name) | Delete a shorter name from the function. | (none) |
| 0.5.2.2 - (Current) | ext_halo_crash [boolean] | To allow Halo crash with notification show up. (Default: false) | (none) |

<div class="datatable-end"></div>

{% include links.html %}
