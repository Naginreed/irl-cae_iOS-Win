# General Info
This Guide describes a **Cheap and Easy** Solution for
- better **IRL**-Streaming 
- **IPhone (iOS)** as Streaming Phone
- **Windows** as Home PC

> [!NOTE]  
> There are completely "free" methods, but they need more technical expertise and if wrongly configured could be a security risk for your Home PC.
> With this Method you don't open up purposely any holes in your Security. *(No fixed IP | No PF | No FW Changes)*

> [!IMPORTANT]  
> <details>
> <summary>You can use the 3 Lines at the top right to jump to any Section of the Guide</summary>
> <img src="https://github.com/Naginreed/irl-cae-setup-ioS/assets/71943093/ddcfa25e-e806-48a7-9882-60fdc8794947">
> </details>
---
## Ko-Fi
<a href="https://ko-fi.com/naginreed"><img src="https://github.com/Naginreed/irl-cae-setup-ioS/assets/71943093/29446800-fcff-4170-9ee0-7fec375ddfd8" alt="Naginreed Ko-Fi" height="60"></a><br> [Wanna help me out?](https://ko-fi.com/naginreed)

---
## Map

<img src="https://github.com/Naginreed/irl-cae_iOS-Win/assets/71943093/1b7cc70e-8250-405b-865c-3a9b3b837140">

> [!NOTE]  
> At first this looks pretty complicated, but we will go Step-by-Step with Pictures *(when available)* trough the whole Setup Process.

**Positives**  

- 👍 can be used with a single Internet connection from Phone
- 👍 when connection from Phone is failing, the Viewer will still see Videos/Clips (1x Stream Start and 1x VOD)
- 👍 a second internet can be added to make the Phone Connection more reliable
- 👍 when switching from WiFi to Mobile and back stream is not going offline

**Negatives**  

- 👎 Additional monthly cost for Relay Server ($10 USD)
- 👎 Additional monthly cost for 2nd Internet (Optional)
- 👎 Takes some time for first Setup
---

# 1 - Streaming Phone  

> [!NOTE]   
> If you have multiple phones, use the strongest/newest one as Streaming Phone

1.a - Follow this [Youtube Guide](https://www.youtube.com/watch?v=GbR0xfpJXJE) to install Moblin and set it up for direct Twitch Streaming _(as Backup)_

---
# 2 - SRT/SRTLA Relay

> [!NOTE]   
> This Server takes the Two SRTLA Streams and combines them into one SRT Stream as seen on [Map](#map)

> [!IMPORTANT]   
> This Service costs $10 USD.

2.a - Create an Account with [Github](https://github.com/signup) *(If you already have one skip to Login)*
 - You then need to Verify your E-Mail Address and [Login](https://github.com/login)

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/bafd6a15-7ec2-4f3e-8a1f-7737e41d9a8f" height="600">

2.b - Once logged in open the [Belabox Sponsorship](https://github.com/sponsors/rationalsa) Page  
 - Scroll down and select the **$10 a month** Tier which includes 1x SRT/SRTLA Relay Server
 - Fill out your Billing Info and setup your Payment Info *(Only Credit Card or Paypal supported)*
 - Alternatively you can also let your Viewers buy [Vouchers](https://shop.belabox.net/product/belabox-cloud-voucher) for multiple Months.

2.c - Once you either sponsored or have a voucher open the [Belabox Cloud](https://cloud.belabox.net) Page and
 - Login/Authorize with your Github Account  

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/5385a7b6-e1c4-42ac-a5a1-729cf53dc732" height="600">
<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/f8b19ac5-7862-4097-8701-78001048d003" height="600">

2.d - On the Top of the Page press the **3 Lines** then **SRT(LA) relays**

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/4c33128e-253c-493e-8d40-2c19e67a2389" height="600">

2.e - Click on **Add** and change the Name. Change the **Server** to your **closest Location**

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/8425c1a1-add3-40d1-8082-b03312429539" height="600">

2.f - Scroll down until you see **Moblin Settings** and tap the **Add automatically to Moblin** Button to automatically add the right Info in Moblin.  

---
# 3 - Streaming Phone
3.a - Open the **Moblin App** and go to **Gear** Symbol *(Settings)* on the top right  

<img src="https://github.com/Naginreed/irl-cae-setup-ioS/assets/71943093/f0723f0a-53a1-441d-990c-00a88d0349f3" width="600">

3.b - Go to **Streams** and then tap the **Belabox Cloud** one  
3.c - Go to **Video** and set the following settings  
 - **Resolution:** 1920x1080p  
 - **FPS:** fixed 30fps  
 - **Bitrate:** 4500 kbps  
 - **Codec:** HEVC(h2.65)

3.d - Go back then **active Twitch** and tap on it to enter. Set your Twitch Name and Twitch ID. *(You can get the ID from [here](https://www.streamweasels.com/tools/convert-twitch-username-to-user-id/))*  
3.e - Next we want to add our Alerts to Moblin. To do this we go to into our Alerts Dashboard via Browser  
 - [Streamlabs](https://streamlabs.com/dashboard#/alertbox) and copy the Widget URL

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/255e3ef7-cbd5-4cfa-84a8-17d68c78ccb6" height="600">
<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/82365cc6-ade2-458f-b583-ccad4b0b62f1" height="600">

3.f - Head back to Moblin and go to the **Settings** Screen. 
 - Tap on **Scenes** then on **Widgets** then **Create**. 
 - Name it **Alerts**  

3.g - Set type to **Browser**  
 - paste the Widget URL into **URL** Field.  
 - Set Width to 600 and Height to 400 *(you change size if the Alerts are wrong size)*  

3.h - Go back to the **Scenes** Menu and tap on **My scene**   
 - Then tap **Add Widget** and choose the **Alert**-Widget we just created.
 - Make sure its on the Top of the List.  

3.i - Go back to the **Main View** and **check** that **Chat** is loading and Test that **Alerts** are **working**  
 - Streamlabs *(Test-Alerts are available in the Dashboard)*  

---
# 4 - Windows-PC
Any normal PC or Laptop can be used, best cabled directly to your Home Internet Router.
 If you want to buy a new one just for this task, maybe look into Mini-Pc's.
> [!WARNING]  
> This PC needs to have a **STABLE** Internet Connection during the whole stream with at least 6Mbit Upload *[Speedtest](https://www.nperf.com)*

## 4.1 OBS
> [!NOTE]  
> This is the Programm that gets the Stream from the Relay Server and converts it back to old RTMP/h.264 Standards and streams it directly to Twitch. Here you have a lot of Options to set Videos, Text, Music to entertain your viewers while you reconnect*

4.1.a - **Download [OBS Studio](https://obsproject.com/download)** for your System  
4.1.b - **Install OBS** Studio and **Launch** it.  

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/3555ea78-d6bd-440b-9bdc-15a91799f1a2" width="400">

4.1.c - In the Auto-Wizard 
 - Optimize for Streaming
 - **Resolution:** 1920x1080
 - **FPS:** 30
 - **Service:** Twitch
 - Connect Account
 - Log in the newly popped up Window.
 - Uncheck the **Estimate bitrate** and enter manually **5900** *(7900 if you're Twitch Partner)*
 - **Finish** the Wizard

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/a6164a26-5ba9-4219-9c22-c2eb6abfa0e1" height="400">
<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/bafb9a3c-1d6e-4909-9c78-d0381c521b30" height="400">
<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/4bf17fc2-00ad-40b0-b262-0334f62d978a" height="400">
<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/c7e714a3-fd5a-4783-aaff-9c82ea227f59" height="400">

4.1.d - **In OBS** on the bottom left **add** now following **scenes**
 - Start
 - Live
 - Low
 - Brb
 - End

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/344aaedc-92df-41c1-9e65-1dd6223deb0d" width="600">

4.1.e - Click on the Live Scene, and add a **Media Source** and with name **Belabox Cloud**. 
 - A new Window with settings will open

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/dedc65b3-03c6-4ad0-a2f6-ef907ff541cc" width="600">

4.1.f - Open the **[Belabox Cloud](https://cloud.belabox.net/#relays)** Page  
 - go to **SRT(LA) relays** and
 - scroll down until you see **OBS Media Source Settings**

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/d6669e01-035c-4879-aa2e-df7ebe333b9a" width="600">

4.1.g - **Go back** to **OBS** and **set** the **same settings**
 - Uncheck Local File
 - Set Network Buffering to 1 MB
 - Copy Input from Belabox Cloud Page
 - Set Reconnect Delay to 2S
 - Check Close file when inactive

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/fb5d68c6-b45b-4b40-8f70-ad1aaf224e78" width="600">

4.1.h - Right-click on the **Belabox Cloud**-Source, then **Transform** and **Fit to Screen** *(or select it and hit CTRL+F)*  

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/c993bb43-a3ea-4bc5-a75a-c46858d2305e" width="600">

4.1.i - Then Copy *(CTRL+C)* the **Bellabox-Cloud**-Source over to the **Low** Scene  
4.1.j - Go To **Settings** on the bottom right. In the new Video select **Audio** and **Disable all Global Audio Devices**  

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/20b58802-fc64-491d-9d74-3bd0aef2d93d" width="500">
<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/87a30f26-a525-47c2-9427-b0a1ffbe7067" width="500">

4.1.k - On the top menu bar click on **Tools** then on **Websocket Server Settings**. Check the **Enable WebSocket Server** and hit **OK**  

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/cec9078c-a2e2-45dc-9bec-24041f19a98f" width="500">
<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/918e7d93-3191-4080-b5e3-3d1c8c4b9d85" width="500">

---
## 4.2 NOALBS
> [!NOTE]  
> This is the Program that controls OBS via Chat-Commands and automatically switches Scenes if Stream from the Phone is detected or lost

4.2.a - **Download [NOALBS](https://github.com/NOALBS/nginx-obs-automatic-low-bitrate-switching/releases)** for your System and unpack them to a location of your liking *(i recommend making a Stream and then a NOALBS Sub-Folder)*  
4.2.b - Inside this Folder you should have now the following 3 files
 - .env
 - config.json
 - noalbs

4.2.c - For NOALBS to respond to our Chat commands we need to give access to a Twitch Account. Once you logged in with your preferred Account in Twitch, click on this **[Link](https://b3ck.com/twitch/oauth)**, then hit **Authorize with Twitch** and copy the whole Code from the website

<img src="https://github.com/user-attachments/assets/d668b651-5f7e-45b3-9e1a-e26eb5174b19" height="200">
<img src="https://github.com/user-attachments/assets/44ca3f4b-4ea8-47a8-868e-180fc5c62ba7" height="180">

4.2.d - **Open** the **.env** File with a Text-Editor
 - replace everything with your copied data

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/33dabd80-1a70-4ac1-8451-b942200767b0" height="40">

 - save and close the file
[config.json](config.json)  

4.2.f - **Open** the **config.json** File with a Text-Editor  
 - replace all 3x of *REPLACE_STREAMER_NAME* with your Twitch Account Name

4.2.g - open the Open the **[Belabox Cloud](https://cloud.belabox.net/#relays)** Page and go to **SRT(LA) relays**  
 - Scroll down to **NOALBSv2 configuration**
 - replace *REPLACE_BELLABOX_URL* with the URL from the Belabox Page
 - replace *REPLACE_BELLABOX_INGEST_KEY* with the last Part of the URL

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/fe194e73-c223-4327-9680-af1b570869b1" height="350">

4.2.h - Go back to OBS into the Websocket Settings and click on **Show Connect Info**. 
 - Copy the **Server Password**
 - replace *REPLACE_OBS_WEBSOCKET_PASSWORD* with the copied data

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/ab6652a4-7ff0-41f6-8746-1290e2d243ba" height="200">
<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/7f04f75c-0611-43d6-8831-5fc8487981db" height="300">
<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/f16885ce-8c51-4bb4-92fa-b0e7311f3b41" height="100">

4.2.i - Save and close the file. *Detailed Infos [NOALBS Github](https://github.com/NOALBS/nginx-obs-automatic-low-bitrate-switching)*  
4.2.j - Start the **noalbs** programm. It should look like the picture below. Errors are also shown here  

<img src="https://github.com/Naginreed/irl-cae-setup/assets/71943093/0329e383-07f3-40e8-8f80-de3d0fa3391d" height="270">

4.2.k - You can create a Shortcut by right-clicking the noalbs file and hit **Create Shortcut** and drag the Shortcut for example on Desktop for easier access  

---
# 5 - Make OBS pretty
We are finished with the basic Setup, but the Scenes are pretty emtpy.
Following is an Explanation on what Scene is used for what and what People normally put in. 
> [!NOTE]  
> Following are just recommendations. Feel free to design however you want.

**Start**
- Every time the Stream starts with this scene until the phone is live
- Video+Music is often used as Background
- simple Text "Starting Soon ..."

**Live**
- As soon as there is a connection from the Phone to OBS this will be shown
- No additional things needed, since Overlays should run on the Phone

**Low**
- When connection to the Phone is bad quality
- simple Text "low bitrate"
  
**Brb**
- When the connection to Phone is lost completely or you end the livestream in IRLPro on purpose *(for privacy)*
- old VODs or Clips are often used (For Clips i recommend a Folder named Clips and adding a VLC Media Source *requires [VLC Media Player](https://www.videolan.org/vlc/)*)
- simple Text "Be right back"
- Can be switched to when you go to Toilet or have private Conversation for a few Minutes
  
**End**
- Can be activated by writing !end in Twitch-Chat
- Similar to Starting Video+Music
- Simple Text "Ending Stream"

---
# 6 - Normal Operation 
> [!NOTE]  
> Before **every** IRL-Stream you need to do the following

6.a - **Start** your **PC** at Home an make sure it has a Internet Connection and that the PC doesn't turn off automatically  
6.b - **Start OBS & NOALBS** on your PC  
6.c - **Go outside** to where you want to start your IRL-Stream  
6.d - Enter `!start` in **Twitch-Chat** to start Stream to Twitch  
6.e - **Go Live in IRL Pro** -> after a few seconds you are switched to **Live-Scene**  
6.f - If you stop or loose connections on the Phone -> after a few seconds you are switched to **Brb-Scene**  
6.g - As soon as connection from Phone to Internet is restored -> after a few seconds you are switched back to **Live-Scene**  
6.h - End/Start the Livestream manually in IRLPro to switch between `!brb` and `!live`  
6.i - **Stop the Stream** automatically if you raid someone or with Chat command `!stop`  

> [!IMPORTANT]  
> With every Scene Change in OBS you will see a text Message in Chat
---
# 7 - 2nd Internet Connection  
> [!NOTE]  
> This is optional and improves stream stability alot in many cases. But it doesnt prevent outtages in No Service Areas like deep into the Mountains or Tunnels.

As seen in the [Map](#map) there can be 2nd Internet Connection for your phone to reduce the chance of outtages for the Live Stream.  
Either a Mobile WiFi Router or a Second Phone with Mobile Hotspot active.  

> [!IMPORTANT]  
> For this second SIM a different Provider is highly recommended.
> The 2nd Sim will also consume about ~50% of the overall Data
---
# 8 - Stream directly to twitch  

If for whatever reason the Relay or Home PC is not working you can easily switch back to direct Streaming in the Moblin App. 
Check out this Youtube Video: [Moblin to Twitch (Direct) - Basic Setup Guide
](https://www.youtube.com/watch?v=GbR0xfpJXJE)

8.a - Got to **Settings** > **Connections** and Switch **Belabox off** and **Twitch on**  
<details>
<img src="https://github.com/Naginreed/irl-cae_Android-Win/assets/71943093/452ea3a0-76e7-4cf1-8f16-4e9f531f2923" height="600">
<img src="https://github.com/Naginreed/irl-cae_Android-Win/assets/71943093/45b2d58a-e62e-426f-bc2c-e0af3e1d582b" height="600"> 
</details>

8.b - Go back to **Settings** then **Video**. Scroll down and turn **Bitrate matches resolution** back on and **Format** to Auto.  
<details>
<img src="https://github.com/Naginreed/irl-cae_Android-Win/assets/71943093/011c5d28-461d-4c5a-a0ff-9f09bcf24de6" height="600">
<img src="https://github.com/Naginreed/irl-cae_Android-Win/assets/71943093/f2bbe20d-c1d8-408f-90c0-7e54a56b2936" height="600">
</details>

---
# 9 - Additional Help  
### Moblin App 
Here is their [Discord](https://discord.gg/Tm6kf778)
### OBS 
you can check their [Forum](https://obsproject.com/forum/) or just look up one of the hundreds of Youtube Tutorials
### NOALBS
Here is the Guide on [Github](https://github.com/NOALBS/nginx-obs-automatic-low-bitrate-switching) and their [Discord](https://discord.gg/efWu5HWM2u)
