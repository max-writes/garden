---
{"dg-publish":true,"dg-path":"fragments/instructions/NAS.md","permalink":"/fragments/instructions/nas/","created":"2025-02-15T11:26:20.906-05:00","updated":"2025-08-18T15:47:15.995-04:00"}
---

#type/how-to #notes/technology #notes/content-management 
# NAS (Network Attached Server)

> [!INFO] Audience note
> I am a beginner! I'm writing steps based on what I've done as my knowledge grows. 
> 
> If you're also a beginner this page may help guide you, but my instructions are specific to my tools. If your setup is different from mine, you might find more assistance via help articles from your NAS's website. However, from what I understand, much of the functionality is similar across different devices.
> 
> If you're coding or dealing with terminals, you know more than I do and these guides likely won't help you. (However, please feel free to review and correct me so I can give better information to my peers!)

## About
In a nutshell: A home NAS (Network Attached Server) is a personal storage device (hard drive) that connects to your home network, so that any device in your network can access it. This is similar to how office printers are set up - they connect to the network, not a specific computer, so that all computers connected to that network can print stuff.

NAS devices often have built-in software to allow for streaming and remote access. When I sought out my NAS I specifically looked for one compatible with 
[[garden/fragments/instructions/Use Plex on Home NAS\|Plex media server]] so I could stream music to myself while I was on road trips.

Notes
- Make sure you set up a backup system sooner rather than later
- Even if you're not touching it for a while, login to all the apps in case they need updates! Sometimes your NAS will get updates for safety and security.

### My setup
[Asus AS5402T](https://www.asustor.com/en/product?p_id=81)

## Instructions

### 1. Install drive
Before initializing your NAS, you must install a drive. Your NAS will have specific instructions provided with the product. Use the product's website to find compatible hard disks. **Ensure compatibility before purchasing.**

Asustor AS5402T compatibility and instructions: https://www.asustor.com/getting_start/steps?series=21

*To be continued...* I didn't take pictures while I set up the hardware but I'll need a second drive soon, so I'll add them then.
### 2. Set up NAS
If you're using an NAS with simplified instructions, it probably recommends a mobile app to manage your NAS. There may also be a control center you can install to your computer for device management.
	My NAS uses [AiMaster](https://www.asustor.com/admv2?type=4&subject=19&sub=69) mobile app and the [Asustor Control Center](https://www.asustor.com/service/download_acc) on the computer.

### Access storage via computer
The first time you ever access via a new device, you'll need to login to the server. Subsequent visits will connect automatically unless you sign off.

1. Navigate to the file explorer on your computer (or open your Documents, Pictures, or other default folders).
2. On the left sidebar, select **Network**.
3. You might see your router, printer, or other computers/devices. The NAS should appear here as well given the name you provided during setup.
4. Double-click on the NAS. If you get an error, it may still be starting up. Wait a bit then try again. 
5. This will prompt you to login. Add your NAS user/password (your username is not an email).
6. After you login, you'll be able to browse, add, update, delete, or reorganize files in the NAS.

### Gather details
You will need these items for the remaining instructions in this guide. You must complete drive installation and NAS setup prior to following these steps.

* **NAS IP**: You can find this in the NAS app.
	In AiMaster, find this information by selecting the **System information** icon then choosing **Network**. You'll find the IPv4 under LAN1 or LAN2.
### Set up a website
1. Use your NAS app to download the appropriate apps, depending on your needs. For a simple site, you can start with an HTTP Server. If you plan to use WordPress, make sure you also download one of the PHP options (most up to date).
     - I am not sure what I'll use this for yet, so for the time being I downloaded Apache HTTP Server and PHP 8.3.
2. Use your NAS app to enable web server ports. 
	- In AiMaster, navigate to **Web Center** and select both options to **Enable Web server port** and **Enable secured Web server port**. 
	- Toggle **Minimum security protocol** and **Enable personal website**. 
3. On your computer, navigate to your home folder on the NAS, create a folder called **www**, and add an index.html test file with text on it.
4. In the browser, navigate to NAS.IP/~USERFOLDER. Your index.html file should come up.
    - Congratulations! You can now visit your website, and you're your own host! 
    - In the next steps, I'll figure out how to make it so people outside your network can visit your website.
*To be continued...*


### Backup your NAS
- Find a cloud service that meets your needs (I use iDrive)
- Install the app on your NAS
- Backup now (it will take several hours)
- Schedule a backup (frequency depends on how often you change it - I do this once a month because I only change my server files that often)
- If there's enough space for all your things, you can take this opportunity to backup your computer too (this will also take several hours)

Links
- https://www.idrive.com/asustor-backup
- https://www.asustor.com/online/College_topic?topic=152

Things to add: EZ-connect