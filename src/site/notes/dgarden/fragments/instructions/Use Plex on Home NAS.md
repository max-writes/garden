---
{"dg-publish":true,"permalink":"/dgarden/fragments/instructions/use-plex-on-home-nas/","created":"2025-08-18T14:04:11.613-04:00","updated":"2025-08-18T14:19:57.874-04:00"}
---

#type/how-to #notes/technology #notes/content-management 
# Use Plex on Home NAS

> [!INFO] Audience note
> I am a beginner! I'm writing steps based on what I've done as my knowledge grows. 
> 
> If you're also a beginner this page may help guide you, but my instructions are specific to my tools. If your setup is different from mine, you might find more assistance via help articles from your NAS's website. However, from what I understand, much of the functionality is similar across different devices.
> 
> If you're coding or dealing with terminals, you know more than I do and these guides likely won't help you. (However, please feel free to review and correct me so I can give better information to my peers!)

## About
In a nutshell: Plex is an on-demand streaming service and media server comprised of your personal library of files, files shared by other Plex users you know, and Plex service options (free, rent, buy).

It's similar to Netflix and Hulu and the others in that Plex does offer options that you don't have to own, but it's different in that the majority of your library can be made up of your media. If you have the appropriate account level and setup, you can share your library with other Plex users to stream from their homes, or for yourself to stream from afar (when you're away from your home network). 

This is the primary reason I set up my [[dgarden/fragments/instructions/NAS\|NAS]] - so I could listen to my music library wherever I wanted without keeping it on my phone. (I also needed a good way to backup decades of photos and videos.)

I very specifically miss the YouTube recommendation engine, whatever they used from the mid 2010s to around 2023. It knew me very well and recommended a lot of good music to me during that time! RIP. Otherwise, I don't miss music streaming services and with my Plex lifetime membership, I'm glad not to pay a monthly service or rely on free versions of crappy music apps that privilege ad revenue over playing songs on a list in order. Being able to listen to an album beginning to end, in order, without other music from different artists played in between, is one of those bare minimum expectations I have for music apps and devices.

## Instructions
You must complete drive installation and NAS setup prior to following these steps. You can't use Plex on your NAS before your NAS is set up...
### Gather details
You will need these items for the remaining instructions in this guide. 

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
4. Follow the prompts to name your library (this shows up for everyone you share with), add media, and begin the library scan. 
	- When you select media locations, it should already be on your NAS. In other words, if it opens a folder on your computer and makes you browse to NAS, then you're not in the right place.
	- Review the URL to **ensure you are visiting via the NAS IP address** (*NAS.IP:32400/web*), **and not Plex's website** (*app.plex.tv/desktop).
	- If you connect via Plex's website, your *computer* will be the server instead of the NAS, and it must be on for you to stream your media.
5. Depending on the size of your library, the scan may take a few hours, but once it's done your library is ready to use!

#### Plex Updates
After a new Plex release, it may take time for your NAS control center to reflect the change and make the update available. (One reason you might need it is if your server suddenly becomes unreliable and gives you an update message.) If you want or need it right away, you can download and manually install an update file from here:

https://www.plex.tv/media-server-downloads/?cat=nas&plat=asustor

<small>Source: <a href="https://www.reddit.com/r/synology/comments/1baub57/why_cant_i_update_plex_on_my_synology_nas_anymore">reddit</a></small>

After choosing your platform, there may be more information or a link to a manual available that will help with your installation.

In my case, here were the steps:
1. Download the .apk file from the link above for **ASUSTOR**
2. Login to the **ASUSTOR Control Center**
3. Select **My Apps**
4. In the **App Central** box, select **Management > Manual Install**, then **Browse** for the .apk file downloaded in Step 1. Select **Upload** to initiate the update.

![[NAS-1746382125376.png\|(1) Management > (2) Manual Install > (3) Browse to find .apk file > (4) Upload]]

![[NAS-1746382261719.png\|Uploading File shows while you wait.]]

5. You may get a message about the risks associated with installing unverified apps (similar to the message you get when you try to install .apk files on your phone). Review the details and verify you're comfortable with continuing.
6. After accepting and installing, progress will begin.

![[NAS-1746382391786.png\|Plex Media Server shows a green progress bar while installing the update.]]

5. After installation completes: In Plex, go to **Settings > General** and ensure it confirms that you're up to date.

![[NAS-1746382995106.png\|(1) Settings > (2) General settings > (3) Check for updates]]

6. Make sure your Plex apps are up to date everywhere else (TV, phone, etc.) too!


Things to add: sharing your Plex library 