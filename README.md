This guide has been moved from Discord to Github to avoid potential issues and limitations.
This is the reason for the somewhat strange structure and steps splitting in this guide, but it works just as well either way, so no biggie!
<-

# Welcome to the Vanilla WoW (1.12.1) client tweaks guide!

The Vanilla WoW 1.12.1 client that Turtle WoW is built upon is now nearly 20 years old, and it's far from flawless. The following "client mods" or "client tweaks" aim to provide you a better gameplay experience by fixing issues and adding some features we've come to expect over the years.

Information regarding each individual tweak/mod can be found via the links provided below.

### This guide includes step-by-step guidance on how to install the following tweaks/mods:
* [VanillaFixes](<https://github.com/hannesmann/vanillafixes>) (+ [DXVK](<https://github.com/doitsujin/dxvk>))  
* [Vanilla-Tweaks](<https://github.com/brndd/vanilla-tweaks>)
* [SuperWoW](<https://github.com/balakethelock/SuperWoW>) (+ [SuperAPI](<https://github.com/balakethelock/SuperAPI>) for in-game options)

There are several additional tweaks/mods out there, but these are the most essential ones that I would recommend to every single player.

<details>
<summary> Step 1 (Click me) </summary>

# Client Tweaks - Step 1

Before we start we must disable our Antivirus software and add TurtleWoW's game folder to exclusions.
This is to ensure that Windows Defender (or any other antivirus software you may have) doesn't delete any of the files.
**The explanation for why AV software false flags VanillaFixes can be found on the [VanillaFixes - Releases](<https://github.com/hannesmann/vanillafixes/releases>) page. **
-# In short, there's no way for antivirus software to differentiate between VanillaFixes, which *we want* to inject the mod DLL's into our game, and a malicious DLL injector that would be used for nefarious purposes. As a result it considers VanillaFixes a virus/malware even though it's not.

### These are the steps shown in the video below:
1. Open **Windows Defender** / **Windows Security**
2. Under **Virus & threat protection**, click **Manage settings**
3. Set **Real-time protection** to **Off**
4. Scroll down to **Exclusions** and click **Add or remove exclusions**
5. Click **+ Add an exclusion** and select **Folder**
6. Navigate to your TurtleWoW installation folder and hit **Select Folder**
-# for example "G:\TWoW\twmoa_1172" as seen in the video below
7. Confirm in **Exclusions** list that the game folder was added successfully


![Video](https://cdn.discordapp.com/attachments/1317115547749580824/1325992839934644244/Step-1.mp4?ex=677dce90&is=677c7d10&hm=31e5efe37b22919329add4df71a7e363883cbd2bee2349435dc3ceeeeddc46da&)
</details>

<details>
<summary> Step 2 (Click me) </summary>

## Client Tweaks - Step 2
Now, let's download our first actual client tweak, we'll start with VanillaFixes!

Confirm that your antivirus software is still temporarily **disabled** during the download and installation of **VanillaFixes**

### These are the steps shown in the video below:
1. Head on over to **GitHub** and download the latest version of [**VanillaFixes**](<https://github.com/hannesmann/vanillafixes/releases>) 
-# (*DXVK version highly recommended, if it doesn't work you can just delete d3d9.dll from your TurtleWoW game folder later*)
2. Save the VanillaFixes zip file somewhere you will be able to find it for the next step

[Video](https://cdn.discordapp.com/attachments/1317115547749580824/1325998709636595812/Step-2.mp4?ex=677dd408&is=677c8288&hm=34d5bd8f3464ddb38105809202b1501c35d1b21e45c5bf831dd1772cd9efdb9f&)
</details>

<details>
<summary> Step 3 (Click me) </summary>

## Client Tweaks - Step 3
Time to extract VanillaFixes and place it in the game folder!

Confirm that your antivirus software is still temporarily **disabled** during the download and installation of **VanillaFixes**

### These are the steps shown in the video below:
1. **Locate** the **VanillaFixes** zip file you downloaded during Client Tweaks - Step 2
2. **Extract** the zip file contents
3. **Move**/**copy** the extracted files over to your **TurtleWoW game folder**
4. If everything was done correctly, **VanillaFixes/VanillaFixes-DXVK is now successfully installed**

**Important note:** From now on we will use VanillaFixes.exe to start the game, otherwise all of these tweaks and mods will not be enabled!

[Video](https://cdn.discordapp.com/attachments/1317115547749580824/1326001882455478304/Step-3.mp4?ex=677dd6fc&is=677c857c&hm=07b9c37402a712511d4803f15821443028e897eeecbb97faa08d897709640f30&)
</details>

<details>
<summary> Step 4 (Click me) </summary>

## Client Tweaks - Step 4
Now let's download Vanilla-Tweaks 
-# Although Vanilla-Tweaks is now built into the launcher, we'll do a regular installation for the sake of consistency and avoid the TurtleWoW.exe launcher

For this step it **doesn't matter** whether your antivirus software is **enabled** or **disabled**

### These are the steps shown in the video below:
1. Head on over to **GitHub** and download [**Vanilla-Tweaks**](<https://github.com/brndd/vanilla-tweaks/releases>) for Windows
2. **Save** the zip file to your computer
3. **Locate** and **extract** the Vanilla-Tweaks zip file

[Video](https://cdn.discordapp.com/attachments/1317115547749580824/1326014509290229792/Step-6_DL_VT.mp4?ex=677de2bf&is=677c913f&hm=e09fe6a4286a8a367d3b52a2539c362401cd5d8c29fc15d66a434ee2d63e6f56&)
</details>

<details>
<summary> Step 5 (Click me) </summary>

## Client Tweaks - Step 5
Now let's install/apply Vanilla-Tweaks 
-# Although Vanilla-Tweaks is now built into the launcher, we'll do a regular installation for the sake of consistency and avoid the TurtleWoW.exe launcher

For this step it **doesn't matter** whether your antivirus software is **enabled** or **disabled**

### These are the steps shown in the video below:
1. **Copy** your **WoW.exe** file from TurtleWoW game folder **into the Vanilla-Tweaks folder**
2. **Drag** & **drop** the original **WoW.exe** onto **Vanilla-Tweaks.exe**
3. A new file named **WoW_Tweaked.exe** will appear in your **Vanilla-Tweaks folder**
4. **Move/copy** the new **WoW_Tweaked.exe** over to your **TurtleWoW game folder**
5. **Rename** the old **WoW.exe** to **WoW_OLD.exe** or something similar
6. **Rename** the new **WoW_Tweaked.exe** file to **WoW.exe**
7. If everything was done correctly, **Vanilla-Tweaks is now installed successfully**

[Video](https://cdn.discordapp.com/attachments/1317115547749580824/1326020171600629760/Step-7_Apply_VT.mp4?ex=677de805&is=677c9685&hm=9c82c4974388270accbd432f3d19b2aee269133f76bcd04aa1c523cfc2e7a2a2&)
</details>

<details>
<summary> Step 6 (Click me) </summary>

## Client Tweaks - Step 6
Now let's download and install SuperWoW

Your Antivirus software must be **disabled** during the download and installation of **SuperWoW**
-# If you need a reminder on how to disable Windows Defender, scroll back up and refer to the **Client Tweaks - Step 1** part of the guide

### These are the steps shown in the video below:
1. Head on over to **GitHub** and download the latest version of [**SuperWoW**](<https://github.com/balakethelock/SuperWoW/releases>) 
-# Ignore the "SuperWoW mpq patch"
2. **Extract** the SuperWoW zip file contents
3. **Move/copy** only **SuperWoWHook.dll** over to the **TurtleWoW game folder**
-# We do not need the SuperWoWLauncher since VanillaFixes will already detect and load SuperWoWHook.dll
4. If everything was done correctly, **SuperWoW is now successfully installed**
-# Although in order to see the in-game configuration menu, you also need to download and install the [SuperAPI](<https://github.com/balakethelock/SuperAPI>) addon
-# Install SuperAPI like any regular addon. Extract and place files into twow > interface > addons, or by using the [GitAddonsManager](<https://woblight.gitlab.io/overview/gitaddonsmanager/>) (recommended)
-# GitAddonsManager install + usage info can be found [here](<https://turtle-wow.fandom.com/wiki/Addons#How_to_Install_Addons>)


[Video](https://cdn.discordapp.com/attachments/1317115547749580824/1326025167939309598/Step-8_SuperWoW.mp4?ex=677decac&is=677c9b2c&hm=c416c662a2700231d0903603a220a3a153d685b612dca48e045beeb779023e22&)
</details>

<details>
<summary> Step 7 (Click me) </summary>

## Client Tweaks - Step 7
Now we'll add the **optional** "Async Patch" to our previously installed DXVK from Client Tweaks - Step 1-3
-# Although this is a completely optional step, I strongly recommend that you try it out as it gives a very significant performance boost (big bump up in FPS, and a much smoother/more responsive game)

It doesn't matter whether your antivirus software is enabled or disabled for these steps

### These are the steps shown in the video below:
1. **Download** and **extract** the [**DXVK Async Patch**](https://tretrauit.me/dxvk-async-builder/) 
-# If the link above is broken, try **[this](<https://tretrauit.gitlab.io/dxvk-async-builder//>)** instead
2. **Open** the **extracted folder** and find the folder inside named **x32**
3. Inside the **x32** folder, **copy d3d9.dll**
4. Place **d3d9.dll** into your **TurtleWoW game folder**
5. If prompted, select **Yes/Replace** when asked if you'd like to **replace** the existing **d3d9.dll** that came bundled with **VanillaFixes-DXVK**


[Video](https://cdn.discordapp.com/attachments/1317115547749580824/1326062405234589706/Step-4_Async.mp4?ex=677e0f5a&is=677cbdda&hm=0444aa12899797fe5b99eea424ed2acf825645586a5d863dcb1834050ac397b9&)
</details>

<details>
<summary> Step 8 (Click me) </summary>

## Client Tweaks - Step 8
This is the final step of the entire guide! 
Lastly we will adjust the DXVK configuration file to actually enable Async and some other stuff!

It doesn't matter whether your antivirus software is enabled or disabled for these steps

### These are the steps shown in the video below:
1. **Navigate** to your **TurtleWoW game folder**
2. **Open/edit** the **dxvk.conf** file with a text editor such as **Notepad**
3.  **Replace** all the text inside the file with the text found [**here**](<https://pastebin.com/SgsqegeQ>)
-# The above configuration should work for most users without any issues. However, do NOT increase the framerate limit to higher than 245 as this will cause graphical issues.
-# If you prioritize energy savings over performance, lower the d3d9.maxFrameRate = 245 to match your monitor's refresh rate (common refresh rates are 60, 120, and 144).
4. **Save** and close the **text editor**
5.  If done correctly, **DXVK Async Patch is now successfully installed**

**If you for some reason wish to revert the Async Patch, set** `dxvk.enableAsync = True` **to** `dxvk.enableAsync = False`


[Video](https://cdn.discordapp.com/attachments/1317115547749580824/1326067888255406150/Step-5_Async_Conf.mp4?ex=677e1475&is=677cc2f5&hm=184b00eae45644bc0f3b6a66312d6a03bba4bb6cc327f5e9df1384b175998eef&)
</details>
