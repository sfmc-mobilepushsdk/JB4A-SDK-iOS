---
layout: page
title: "Custom Sound"
subtitle: "Specify Custom Notification Sound"
category: features
date: 2015-05-14 12:00:00
order: 7
---

This feature uses a sound included in your mobile app as a custom audio signal when a push message arrives on the mobile device. To enable the use of custom audio for your <i>remote notifications<i/>, implement the following steps:

1. Add a **custom.caf** file (label it exactly as written) to your project. The cloud push payload will look for a file named **custom.caf**.
<br/>
 <img class="img-responsive" src="{{ site.baseurl }}/assets/audio_step1.png" /><br/>
<br/>
1. Add the "custom.caf" audio file to the **Copy Bundle Resources** for your app. 
<br/>
 <img class="img-responsive" src="{{ site.baseurl }}/assets/audio_step2.png" /><br/>
<br/>
1. [Specify the **Custom** option for sound](http://help.exacttarget.com/en/documentation/mobilepush/administering_your_mobilepush_account/apps_and_optional_settings_in_your_mobilepush_account/#customSound) when you send a push message from the Marketing Cloud user interface. 

> When troublehooting and moving audio assets around, make sure you perform a clean build folder in Xcode anytime you make changes to your audio file assets. Otherwise, Xcode may used cached files. Navigate to the Product menu, then hold option key down and select **Clean Builder Folder**.