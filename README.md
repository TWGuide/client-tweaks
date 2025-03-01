This guide has been moved from Discord to Github to avoid potential issues and limitations.  
This is the reason for the somewhat strange structure and steps splitting in this guide, but it works just as well either way, so no biggie!  

# Welcome to the Vanilla WoW (1.12.1) client tweaks guide!

The Vanilla WoW 1.12.1 client that Turtle WoW is built upon is now nearly 20 years old, and it's far from flawless. The following "client mods" or "client tweaks" aim to provide you a better gameplay experience by fixing issues and adding some features we've come to expect over the years.  

Information regarding each individual tweak/mod can be found via the links provided below.  

> This guide assumes you are using an **_AMD_** or **_Nvidia_** graphics card.  
> For _Intel HD Graphics_ users (usually laptops) the Async Patch in Step 7 and Step 8 **_will NOT work_.**  
> You're free to try these tweaks regardless, but things might break if you are not using AMD/Nvidia GPUs from ~2014 or later.  


### This guide includes step-by-step guidance on how to install the following tweaks/mods:  
* [VanillaFixes](<https://github.com/hannesmann/vanillafixes>) (+ [DXVK](<https://github.com/doitsujin/dxvk>) which already comes bundled with VanillaFixes)  
* [Vanilla-Tweaks](<https://github.com/brndd/vanilla-tweaks>)  
* [SuperWoW](<https://github.com/balakethelock/SuperWoW>) (+ [SuperAPI](<https://github.com/balakethelock/SuperAPI>) for in-game options)  

There are several additional tweaks/mods out there, but these are the most essential ones that I would recommend to every single player.  

<details>
<summary> Step 1 - Disable AV </summary>

## Client Tweaks - Step 1

Before we start we must disable our Antivirus software and add TurtleWoW's game folder to exclusions.  
This is to ensure that Windows Defender (or any other antivirus software you may have) doesn't delete any of the files.  

**The explanation for why AV software false flags VanillaFixes can be found on the [VanillaFixes - Releases](<https://github.com/hannesmann/vanillafixes/releases>) page.**  

> In short, there's no way for antivirus software to differentiate between VanillaFixes, which *we want* to inject the mod DLL's into our game, and a malicious DLL injector that would be used for nefarious purposes. As a result it considers VanillaFixes a virus/malware even though it's not. 

### These are the steps shown in the video below:
1. Open **Windows Defender** / **Windows Security**
2. Under **Virus & threat protection**, click **Manage settings**
3. Set **Real-time protection** to **Off**
4. Scroll down to **Exclusions** and click **Add or remove exclusions**
5. Click **+ Add an exclusion** and select **Folder**
6. Navigate to your TurtleWoW installation folder and hit **Select Folder**
> for example "G:\TWoW\twmoa_1172" as seen in the video below
7. Confirm in **Exclusions** list that the game folder was added successfully


[![Video](https://github.com/TWGuide/client-tweaks/Media/Step1.png)](https://github.com/user-attachments/assets/a9a1e95a-dd7f-454e-97ce-10fe912f5f5e)

</details>


<details>
<summary> Step 2 - Download VanillaFixes </summary>

## Client Tweaks - Step 2
Now, let's download our first actual client tweak, we'll start with VanillaFixes!

Confirm that your antivirus software is still temporarily **disabled** during the download and installation of **VanillaFixes**

### These are the steps shown in the video below:
1. Head on over to **GitHub** and download the latest version of [**VanillaFixes**](<https://github.com/hannesmann/vanillafixes/releases>) 
> (*DXVK version highly recommended, if it doesn't work you can just delete d3d9.dll from your TurtleWoW game folder later*)
2. Save the VanillaFixes zip file somewhere you will be able to find it for the next step

[![Video](https://github.com/TWGuide/client-tweaks/Media/Step2.png)](https://github.com/user-attachments/assets/9424cdbc-5721-4c86-a063-650d5fd7ffcb)
</details>


<details>
<summary> Step 3 - Extract VanillaFixes </summary>

## Client Tweaks - Step 3
Time to extract VanillaFixes and place it in the game folder!

Confirm that your antivirus software is still temporarily **disabled** during the download and installation of **VanillaFixes**

### These are the steps shown in the video below:
1. **Locate** the **VanillaFixes** zip file you downloaded during Client Tweaks - Step 2
2. **Extract** the zip file contents
3. **Move**/**copy** the extracted files over to your **TurtleWoW game folder**
4. If everything was done correctly, **VanillaFixes/VanillaFixes-DXVK is now successfully installed**

**Important note:** From now on we will use VanillaFixes.exe to start the game, otherwise all of these tweaks and mods will not be enabled!

[![Video](https://github.com/TWGuide/client-tweaks/Media/Step3.png)](https://github.com/user-attachments/assets/c6c09a0f-95f5-4e80-93b5-3c4e864ae25e)
</details>

<details>
<summary> Step 4 - Download Vanilla-Tweaks </summary>

## Client Tweaks - Step 4  
Now let's download Vanilla-Tweaks  
> Although Vanilla-Tweaks is now built into the launcher, we'll do a regular installation for the sake of consistency and avoid the TurtleWoW.exe launcher  

For this step it **doesn't matter** whether your antivirus software is **enabled** or **disabled**  

### These are the steps shown in the video below:
1. Head on over to **GitHub** and download [**Vanilla-Tweaks**](<https://github.com/brndd/vanilla-tweaks/releases>) for Windows
2. **Save** the zip file to your computer
3. **Locate** and **extract** the Vanilla-Tweaks zip file

[![Video](https://github.com/TWGuide/client-tweaks/Media/Step4.png)](https://github.com/user-attachments/assets/ab156f4b-ea97-4e80-b1ee-d301dc1b271f)
</details>

<details>
<summary> Step 5 - Apply Vanilla-Tweaks </summary>

## Client Tweaks - Step 5
Now let's install/apply Vanilla-Tweaks 
> Although Vanilla-Tweaks is now built into the launcher, we'll do a regular installation for the sake of consistency and avoid the TurtleWoW.exe launcher

For this step it **doesn't matter** whether your antivirus software is **enabled** or **disabled**

### These are the steps shown in the video below:
1. **Copy** your **WoW.exe** file from TurtleWoW game folder **into the Vanilla-Tweaks folder**
2. **Drag** & **drop** the original **WoW.exe** onto **Vanilla-Tweaks.exe**
3. A new file named **WoW_Tweaked.exe** will appear in your **Vanilla-Tweaks folder**
4. **Move/copy** the new **WoW_Tweaked.exe** over to your **TurtleWoW game folder**
5. **Rename** the old **WoW.exe** to **WoW_OLD.exe** or something similar
6. **Rename** the new **WoW_Tweaked.exe** file to **WoW.exe**
7. If everything was done correctly, **Vanilla-Tweaks is now installed successfully**

[![Video](https://github.com/TWGuide/client-tweaks/Media/Step5.png)](https://github.com/user-attachments/assets/475d4148-d0c1-497f-82a1-5c5c35e524f7)
</details>

<details>
<summary> Step 6 - SuperWoW </summary>

## Client Tweaks - Step 6
Now let's download and install SuperWoW

Your Antivirus software must be **disabled** during the download and installation of **SuperWoW**
> If you need a reminder on how to disable Windows Defender, scroll back up and refer to the **Client Tweaks - Step 1** part of the guide

### These are the steps shown in the video below:
1. Head on over to **GitHub** and download the latest version of [**SuperWoW**](<https://github.com/balakethelock/SuperWoW/releases>) 
> Ignore the "SuperWoW mpq patch"
2. **Extract** the SuperWoW zip file contents
3. **Move/copy** only **SuperWoWHook.dll** over to the **TurtleWoW game folder**
> We do not need the SuperWoWLauncher since VanillaFixes will already detect and load SuperWoWHook.dll
4. If everything was done correctly, **SuperWoW is now successfully installed**
> Although in order to see the in-game configuration menu, you also need to download and install the [SuperAPI](<https://github.com/balakethelock/SuperAPI>) addon
> Install SuperAPI like any regular addon. Extract and place files into twow > interface > addons, or by using the [GitAddonsManager](<https://woblight.gitlab.io/overview/gitaddonsmanager/>) (recommended)
> GitAddonsManager install + usage info can be found [here](<https://turtle-wow.fandom.com/wiki/Addons#How_to_Install_Addons>)


[![Video](https://github.com/TWGuide/client-tweaks/Media/Step6.png)](https://github.com/user-attachments/assets/97e6850a-41a9-4263-9de5-0addc3ca84a6)
</details>

<details>
<summary> Step 7 - Download DXVK "Async Patch" </summary>

## Client Tweaks - Step 7
Now we'll add the **optional** "Async Patch" to our previously installed DXVK from Client Tweaks - Step 1-3
> Although this is a completely optional step, I strongly recommend that you try it out as it gives a very significant performance boost (big bump up in FPS, and a much smoother/more responsive game)

It doesn't matter whether your antivirus software is enabled or disabled for these steps

### These are the steps shown in the video below:
1. **Download** and **extract** the [**DXVK Async Patch**](https://tretrauit.me/dxvk-async-builder/) 
> If the link above is broken, try **[this](<https://tretrauit.gitlab.io/dxvk-async-builder//>)** instead
2. **Open** the **extracted folder** and find the folder inside named **x32**
3. Inside the **x32** folder, **copy d3d9.dll**
4. Place **d3d9.dll** into your **TurtleWoW game folder**
5. If prompted, select **Yes/Replace** when asked if you'd like to **replace** the existing **d3d9.dll** that came bundled with **VanillaFixes-DXVK**


[![Video](https://github.com/TWGuide/client-tweaks/Media/Step7.png)](https://github.com/user-attachments/assets/8c9dedf0-dec5-4f4d-9b22-db7fd140751b)
</details>

<details>
<summary> Step 8 - DXVK Config </summary>

## Client Tweaks - Step 8
This is the final step of the entire guide! 
Lastly we will adjust the DXVK configuration file to actually enable Async and some other stuff!

It doesn't matter whether your antivirus software is enabled or disabled for these steps

### These are the steps shown in the video below:
1. **Navigate** to your **TurtleWoW game folder**
2. **Open/edit** the **dxvk.conf** file with a text editor such as **Notepad**
3.  **Replace** all the text inside the file with the text found [**here**](<https://pastebin.com/SgsqegeQ>)
> The above configuration should work for most users without any issues. However, do NOT increase the framerate limit to higher than 245 as this will cause graphical issues.
> If you prioritize energy savings over performance, lower the d3d9.maxFrameRate = 245 to match your monitor's refresh rate (common refresh rates are 60, 120, and 144).
4. **Save** and close the **text editor**
5.  If done correctly, **DXVK Async Patch is now successfully installed**

**If you for some reason wish to revert the Async Patch, set** `dxvk.enableAsync = True` **to** `dxvk.enableAsync = False`


[![Video](https://github.com/TWGuide/client-tweaks/Media/Step8.png)](https://github.com/user-attachments/assets/ae81090e-f6f9-4515-8430-72bbf34bd8ce)
</details>

<details>
<summary> Step 9 - Done </summary>

### Thanks for checking out my guide, I really hope it helped you and I also hope you liked it!

Don't forget to re-enable your **Anti-virus software** once you've downloaded and installed these mods, and excluded/whitelisted the turtlewow game folder!

Also remember that from now on ***VanillaFixes.exe should be used to start the game***, otherwise all of these tweaks and mods will not be enabled!

-Peachoo/Ieaiaio

</details>

<details>

---

<summary> Additional Mods </summary>

As mentioned, there are other mods out there which can be added very easily now that we have VanillaFixes installed.  

**Great additional Tweaks/Mods:**  
* **[Interact](<https://github.com/luskanek/Interact>):** Adds the "Interact Key" feature from modern WoW to the 1.12 client  
> This mod was primarily made for use with the Steam Deck, but it can be useful to anyone!  

* **[Nampower](<https://github.com/pepopo978/nampower>):**  Fixes a flaw in the 1.12 client which can lead to a DPS increase for casters with high ping  
> The above link is a forked version which is in it's beta phase, the original can be found [here](<https://github.com/namreeb/nampower>)  
> I suggest trying pepopo978's fork (the bold link above), as it has more features and a [companion addon](<https://github.com/pepopo978/nampowersettings>) for in-game configuration!  

* **[VanillaMultiMonitorFix](<https://github.com/Mates1500/VanillaMultiMonitorFix>):** Fix for multi monitor setups with differing resolutions for the 1.12 client  
> Adding this to the list just in case VanillaFixes didn't already fix this issue for you. I didn't personally need this fix, but maybe some do.  

* **[UnitXP SP3](<https://github.com/allfoxwy/UnitXP_SP3>):** Attempts to modernize the Vanilla 1.12 client
> Adds features like nameplates that hide when not in line of sight, better tab target functionality, and more!  
> Comes with a [companion addon](<https://github.com/allfoxwy/UnitXP_SP3_Addon>) for in-game configuration  

**VanillaMultiMonitorFix.dll** & **nampower.dll** can simply be dropped into TurtleWoW game folder **without** further configuration, as they are already included in the **dlls.txt** file out of the box.  
**UnitXP & Interact** requires their DLL files to be added to the **dlls.txt** file in your TurtleWoW game folder, simply add `interact.dll` & `unitxp_sp3.dll` to the bottom of the text file.
</details>
