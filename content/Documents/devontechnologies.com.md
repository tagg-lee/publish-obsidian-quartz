---
title: Devonthink(데본씽크) DT3
permalink: 
tags:
  - 🏷️Document
  - 📦App
Keywords:
  - "[[Secondbrain]]"
aliases:
  - Devonthink
  - 데본씽크
description: 
updated: 
created: 2024-02-26
publish: true
---
free-tags:: 

## How To
#### Email to Devonthink
##### References

>You can somewhat replicate the Mail-to-Evernote experience on your Mac:
> 
> 1. In the Contacts app set up a new contact (click “Company” and give the “Company name” something like “2Devonthink” or “2DT”).
>     
> 2. In the email address field, let’s say your email address is “[johnny.appleseed@icloud.com](mailto:johnny.appleseed@icloud.com)”, just add “+DT” or “+Devonthink” after the name before the “@”. So in this example it would be “[johnny.appleseed+DT@icloud.com](mailto:johnny.appleseed+DT@icloud.com)”. This is a little known fact that the “+” and anything after it up to the “@” is ignored by mail servers.
>     
> 3. In Mail on your MacOS machine create a rule:  
>     A. If “To” is equal to “[johnny.appleseed+DT@icloud.com](mailto:johnny.appleseed+DT@icloud.com)”;  
>     B. “Run Applescript” “Mail Rule - Add messages to DEVONthink” (this script is part of the DT3 add-ons);  
>     C. “Move message” to trash.
>     
> 
> So when you are out and about on your iPhone, just forward the message to the contact you had set up like you would to your mail-to-Evernote address. The message will be processed by Mail if and when it is running and you should get your email imported into the DT3 Inbox.
> 
> From there you can create smart rules to file the imported mail automatically. Of course, you could vary the “+your-text-here” part in the name and perhaps use a different one for each subject or database (like an EN Notebook) or tag. Or combine it with text that you add before forwarding to aid filing.
> —[Forward emails to Devonthink - DEVONthink - DEVONtechnologies Community](https://arc.net/l/quote/bdeycsdj)


>The simple answer is: you can’t.
> 
> Apple deprecated Apple Mail plugins and broke things for all third-parties who develop _(and also sell)_ these plugins. There is nothing we can do about this.
> 
> Drag and drop, mail scripts, and mail rule scripts are the first alternatives you could explore. DEVONthink’s **View > Import** sidebar will still work, albeit more slowly without the plugin.
>—[Sending mail to DevonThink not working with macOS Sonoma and DVTP 3.9.3 - DEVONthink - DEVONtechnologies Community](https://arc.net/l/quote/parcxdkk)


>Using Apple Mail Rules
>
>1. Go to **Mail > Settings > Rules**
>2. Click `Add Rule`
>4. Set about `if any/all of the following conditions are met:` with your preferences.
>5. Set `Pertorm the tollowing actions:`
>	1. Left side: `Run AppleScript`
>	2. Right side: `Mail Rule- Add messages to DEVONthink`
>6. Select the Mail and apply the rule
>	1. Shortcut: `option + command + L`
>	2. Option:  **Massage > Apply Rules**