---
{"dg-publish":true,"dg-path":"trees/instructions/NAS.md","permalink":"/trees/instructions/nas/","created":"2025-02-15T11:26:20.906-05:00","updated":"2025-03-18T20:14:02.635-04:00"}
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
* What is an NAS?
* My goals
* My setup - https://www.asustor.com/en/product?p_id=81
## Instructions

### 1. Install drive
Before initializing your NAS, you must install a drive. Your NAS will have specific instructions provided with the product. Use the product's website to find compatible hard disks. **Ensure compatibility before purchasing.**

Asustor AS5402T compatibility and instructions: https://www.asustor.com/getting_start/steps?series=21
### 2. Set up NAS
If you're using an NAS with simplified instructions, it probably recommends a mobile app to manage your NAS. There may also be a control center you can install to your computer for device management.
	My NAS uses [AiMaster](https://www.asustor.com/admv2?type=4&subject=19&sub=69) mobile app and the [Asustor Control Center](https://www.asustor.com/service/download_acc) on the computer.
*To be continued...*
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
### Set up Plex Media Library
1. Move all your media to separate folders depending on type. (Note: This is my recommendation, but you can store your files however you'd prefer.)
	- Plex supports multiple media types and shows the media to users differently, depending on each. 
	- For example, if you put TV shows in the Movies bucket, then each episode will show as a separate movie. If you put TV shows in the TV bucket, then all episodes will be combined into a bucket for that show.
	- Read [Plex's guidance](https://support.plex.tv/articles/) for more details on how to divide your media or find information on your specific use cases.
2. Use your NAS app to download the Plex Media Server app.
3. Follow the [Plex Quick-start instructions](https://support.plex.tv/articles/200264746-quick-start-step-by-step-guides/) to set up your server. The steps you follow depend on your setup, but here's what I did.
	- I've used Plex before so I skipped Step 1 and went immediately to the "Accessing Plex Media Server via the Plex Web App" header.
	- From here, I followed the instructions to launch from NAS.
		- Open a browser window and type the following: *NAS.IP:32400/web*
		- This opens Plex. If you're not a member yet, you can sign up here. If you are, sign in.
		- If you have the Control Center installed to your computer, you can navigate to the Plex Media Server app and it'll open on the NAS IP for you.
4. Follow the prompts to name your library (this shows up for everyone you share with), add media, and begin the library scan. Depending on the size of your library, the scan may take a few hours.
	- When you select media locations, it should already be on your NAS. In other words, if it opens a folder on your computer and makes you browse to NAS, then you're not in the right place.
	- Review the URL to **ensure you are visiting via the NAS IP address** (*NAS.IP:32400/web*), **and not Plex's website** (*app.plex.tv/desktop).
	- If you connect via Plex's website, your computer will be the server and it must be on for you to stream your media.
*To be continued...*
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

Things to add: EZ-connect, sharing your Plex library