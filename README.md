<!--- Special Thanks to Sam (https://github.com/Scherso) for creating a beautiful formatting template for Lilith tutorials --->
<!--- He is a really cool guy with amazing markdown skills and you should check out his incredible work --->
<h1 align="center">

  [Lilith](https://github.com/GhqstMC/LilithReleases) Setup for Windows
  
</h1>

<h4 align="center">

Please note that before doing anything, all files should stay in your Downloads folder; this should be done automatically upon downloading any files associated with Lilith. 

</h4>

---

## Install Lilith in the proper location
- You can download Lilith for windows [Here][lilithdownload] if you haven't already. You can idenitfy it via the green icon next to its name.
- Go to your desktop and right click on an empty space and create a new folder called Lilith
- Drag and drop the executable file you just downloaded into that folder you created. 
-Note: Lilith WILL NOT work if it isn't in its own dedicated folder. Do not skip this step. Additionally, if you accidentally downloaded the Lilith executable more than once it may have something like a (1) at the end of the name that windows automatically gave it. If this is the case, please right click on the executable in your folder, select rename, and then remove the unwanted (1) from the end of it.


## Linking Lilith to Your Discord
- Go into your Lilith folder and double click on the exectuable to run it. A new black window should pop up on your screen.
- Inside this window, there will be a blue link. Please copy and paste that link into a browser of your choice and hit enter. Follow the instructions in your browser to properly link your discord. Do not close Lilith while you are doing this.
- Note: You may be asked to give Lilith access to your username and avatar. Just click yes, this is simply to link your discord account with the Lilith. 
- When you are finished, there should be a green box that says "Hardware Verified". Just be patient and wait a few seconds for Lilith to download all of the necessary files into your Lilith folder. When it is finished, red text will pop up in the console.
- Now that it is safe to close your Lilith console window, please do so.

## Configuring Your TOML File

# Choosing your settings
- Inside of your lilith folder there should be three files: the executable which will be used to run Lilith, a Lilith.log file which is helpful for debugging/troubleshooting, and a toml file. Find the toml file and open it with notepad by right clicking it, selecting "Open with", and choosing Notepad from the list of programs. This should open the Lilith toml file with notepad.
- At the top of your toml file you will find a list of bypasses Lilith has. Although Lilith is not detectable by Hypixel and no one has ever gotten banned for using it, all modifications which could be considered a cheat are turned off by default.
- To renable freelook and autotexthotkey on Lunar Client for Hypixel set `lunar = false` to `lunar = true`
- To enable 1.7 hits for better hit regeistration on Lunar Client set `LunarHitReg = false` to `LunarHitReg = true`
- To enable Lunar Client staff mods like an X-ray module built into Lunar set `LunarCheats = false` to `LunarCheats = true`
- The default stat checking mode of Lilith is to show the overall gamemode stats. For example, if you were to queue a solo bridge game Lilith will show the opponent's bridge overall stats. If you would like to set the stat checking mode to all duels gamemodes overall set `overall = false` to `overall = true`. You will have to scroll down a bit to find this.

# Inserting your credentials
- Scroll down your toml file until you see a line titled `[server.authentication]`. This is where you will input your credentials

<details>
  <summary>
       For Microsoft Accounts</summary>
     
  ## Microsoft Authentication 
  1. **You will see** `ExampleMicrosoftAccount = ['microsoft.account.email@example.com', '', 'microsoft']`
  2. **Replace** `ExampleMicrosoftAccount` **with your Minecraft Account Username, also known as your In Game Name.** 
  3. **Replace** `microsoft.account.email@example.com` **with your email address accociated with your Microsoft Account.**
  
     **Note: do NOT replace** `microsoft` **or the blank field** `''` **with any other text.**
  
</details>

<details>
  <summary>
       For Mojang Accounts</summary>
     
  ## Mojang Authentication 
  1. **You will see** `ExampleMojangAccount = ['mojang.account.email@example.com', 'password goes here!']`
  2. **Replace** `ExampleMojangAccount` **with your Minecraft Account Username, also known as your In Game Name.** 
  3. **Replace** `mojang.account.email@example.com` **with your email address accociated with your Mojang Account.**
  4. **Replace** `password goes here!` **with the password you use to log into your Mojang Account.**
  
</details>





[lilithdownload]: https://github.com/GhqstMC/LilithReleases/releases/download/0.6.0-alpha.3/lilith-win-0-6-0-alpha-3