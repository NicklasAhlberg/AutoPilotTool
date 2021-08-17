# AutoPilot Tool – Upload HW hash with a user interface

<!-- wp:paragraph -->
<p><strong>.Version 1.0.2.3</strong><br>It is now possible to set a default domain name. Get the latest version (1.0.2.3) from GitHub and you will find "<strong>config.txt</strong>" - edit as per your need. Thanks <strong>Dylan Brown</strong> for the idea!</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example: <br></strong><img class="wp-image-552" style="width: 244px;" src="https://www.nicklasahlberg.se/wp-content/uploads/2020/11/config_example.png" alt=""><br><img class="wp-image-551" style="width: 630px;" src="https://www.nicklasahlberg.se/wp-content/uploads/2020/11/config_example2.png" alt=""></p>
<!-- /wp:paragraph -->

.Version 1.0.2.2<br>
It is now possible to use a custom logo. Place "logo.png" in the same directory as the .exe<br>
Recommended logo size: 210x110 px

If you have been working with Windows Autopilot you know that manual upload of the hardware hash is a repetitive and time consuming task.

**This tool will make your life easier by…**<br>
*- Install the necessary PowerShell modules*<br>
*- Connect to the tenant (MFA is supported)*<br>
*- Import the hardware hash.csv-file to the tenant*<br>
*- Initiate a sync*

…. directly from the autopilot device! 

No more need to struggle to manually get, move and import the csv-file from another device. All you need to do is run the tool (Shift+F10 when you get to pick your keyboard layout), start Autopilot Tool and sign in to Azure (when you get prompted) with an administrative user. This works well with MFA!

**Instructions**<br>
1. Put "Autopilot Tool.exe", "Logo.Png" and "Upload-WindowsAutopilotDeviceInfo.ps1" in same directory on either a USB-stick or on a network location<br>
2. Press Shift+F10 when you are at the "pick your keyboard layout" screen<br>
3. Navigate to "Autopilot Tool.exe", press Enter to start the tool<br>
4. Change yourDomain.onmicrosoft.com to your specific need<br>
5. Press the OK-button<br>
6. Sign-on with an Intune Administrator account (or similar) when prompted<br>
7. The HW hash has now been uploaded and will be visible in the Windows Autopilot service

![alt text](https://www.nicklasahlberg.se/wp-content/uploads/2021/08/Autopilot_GIF_new.gif)

| Windows 10 version | Supported |
| ------- | ------------------ |
| 21H1  | :white_check_mark: |
| 20H2  | :white_check_mark: |
| 2004  | :white_check_mark: |
| 1909  | :white_check_mark: |
| 1903  | :white_check_mark: |

This is a UI to Nickolaj Andersens script found at<br>
https://github.com/MSEndpointMgr/Intune/blob/master/Autopilot/Upload-WindowsAutopilotDeviceInfo.ps1
