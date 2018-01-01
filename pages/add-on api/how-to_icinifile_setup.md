---
title: ICIniFile Setup | Add-on API
keywords: api
sidebar: add-on_api_sidebar
permalink: /add-on api/how-to_icinifile_setup.html
folder: add-on api
tags: [how-to,getting_started]
---

I strongly advise you to use UnitTest___ repository to see an example of how to use ICIniFile setup.

Usually Add-on code should follow these steps.

1. Open file
 * If return false, go to step 2.
 * If return true, go to step 3. 
2. Create file
 * If return false, then user does not have permission for directory/file.
 * If return true, go to step 1. 
3. Load data
 * If return false, then there's a problem with file's data.
 * If return true, go to step 4.
4. Check section or key exist
 * If return false, go to step 5.
 * If return true, go to step 6. (only for key exist)
5. Add section or key
 * If return false, then there's a problem with your code or user's side.
 * If return true, go to step 6.
6. Get key
 * If return false, go to step 5.
 * If return true, go to step 7.
7. Save data
 * If return false, then there's a problem with either your code or internally.
 * If return true, go to step 8.
8. Close file
9. Release (Required, can be put in EAOUnload function)

{% include links.html %}
