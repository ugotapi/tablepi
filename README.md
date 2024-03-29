# tablepi
These are shell scripts to turn a Raspberry pi 4+ device into a dashboard for your data on a large screen TV. 
- Using Raspberry Pi OS Bookworm based 64-bit OS on the pi4 8GB device.
- Use Python, Powershell, Chromium, WordPress, WPDatatables a Wordpress plugin and Wordpress plugin fullwidth-templates
- We dowload an Excel file from SharePoint online site or Teams SharePoint online. Then convert to csv and display it in Wordpress on the locally attached TV. 

Youtube walkthrough: [link
](https://youtu.be/YeW6VvDHDKQ)

This involves using Raspberry Pi OS on a Raspberry Pi. The device is then modified to behave as digital signage. Nothing but the content is displayed on the screen. Also there is no Digital Signage service to pay for. It’s Raspbian so it’s secure and doesn’t drop out of being maintained quickly like the other Pi based digital signage setups might. 

Hardware Items you will need:
- Raspberry Pi4 device with 8GB of RAM. 
- MicroSD card for the Pi operating system recommend at least 16GB
- Pi power supply
- HDMI cable
- Pi4 case 
- USB keyboard and mouse. This will only be used for initial setup.
- 4K TV with HDMI port - This is your TV mounted on the wall. 
- Raspberry Pi OS with desktop 64-bit image downloaded
- An Office 365 account with read access to a sharepoint site. Notes: This user does not have need licenses assigned to it. This will not work with an MFA enabled account. Just create an unlicensed user with no group memeberships and lengthen the password.  Then go to the Sharepoint Site and add the user to view only part of the site.
- This assumes your Excel file is in the Root folder of your SharePoint Online site. The scripts or input could be edited to use a subfolder. 

Passwords: I would recommend a long password on the Office365 Limited user account. That user account cannot have MFA set on it. I would also recommend to use a separate long password for the regular sudo user account. Then for all the MariaDB and WordPress accounts I'd make it the same as the regular account just to keep it simple. You won't have multiple users in this setup. 

What you get: Pi4 device that shows a web page of an Excel file on the TV. When the excel file is changed in Office365, it will show on the TV after 15 minutes.  

STEPS:
![Screenshot 2023-10-04 081245](https://github.com/ugotapi/tablepi/assets/14945441/340e5350-cdb0-488d-a4d7-961ee9eaa2b1)


Photo of 4k screen:
![IMG_0336](https://github.com/ugotapi/tablepi/assets/14945441/4afd854f-4e01-4f9c-ba29-6a49110b38cd)




