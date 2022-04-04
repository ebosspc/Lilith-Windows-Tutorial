<!--- Special Thanks to Sam (https://github.com/Scherso) for creating a beautiful formatting template for Lilith tutorials --->
<!--- The majority of this text was written by FireStorm (FireStorm#1000) --->

<!--- Lilith Logo Header --->
<p align="center">
    <img src="https://github.com/GhqstMC/LilithReleases/blob/main/assets/title.png" style="width: 45%">
</p>

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
- Note: Lilith WILL NOT work if it isn't in its own dedicated folder. Do not skip this step. Additionally, if you accidentally downloaded the Lilith executable more than once it may have something like a (1) at the end of the name that windows automatically gave it. If this is the case, please right click on the executable in your folder, select rename, and then manually remove the unwanted (1) from the end of its name.

<details>
  <summary>
    What It Should Look Like So Far</summary>
  
  #### Example Initial Lilith Folder

</details>

<br />

## Linking Lilith to Your Discord
- Go into your Lilith folder and double click on the exectuable to run it. A new black window should pop up on your screen.
- Inside this window, there will be a blue link. Please copy and paste that link into a browser of your choice and hit enter. Follow the instructions in your browser to properly link your discord. Do not close Lilith while you are doing this.
- Note: You may be asked to give Lilith access to your username and avatar. Just click yes, this is simply to link your discord account with the Lilith. 
- When you are finished, there should be a green box that says "Hardware Verified". Just be patient and wait a few seconds for Lilith to download all of the necessary files into your Lilith folder. When it is finished, red text will pop up in the console.
- Now that it is safe to close your Lilith console window, please do so.

<br />

## Configuring Your TOML File

### Choosing your settings
- Inside of your Lilith folder there should be three files: the executable which will be used to run Lilith, a Lilith.log file which is helpful for debugging/troubleshooting, and a toml file. Find the toml file and open it with notepad by right clicking it, selecting "Open with", and choosing Notepad from the list of programs. This should open the Lilith toml file with notepad.
- At the top of your toml file you will find a list of bypasses Lilith has. Although Lilith is not detectable by Hypixel and no one has ever gotten banned for using it, all modifications which could be considered a cheat are turned off by default.

<details>
  <summary>
    Bypasses for Lunar</summary>
  
  #### Enabling Lunar Bypasses
  - To renable freelook and autotexthotkey on Lunar Client for Hypixel set `lunar = false` to `lunar = true`
  - To enable 1.7 hits for better hit regeistration on Lunar Client set `LunarHitReg = false` to `LunarHitReg = true`
  - To enable Lunar Client staff mods like an X-ray module built into Lunar set `LunarCheats = false` to `LunarCheats = true`
  
</details>

<details>
  <summary>
    Bypasses for Forge</summary>
  
  #### Enabling Forge Bypasses
  - To hide your forge mods list from Hypixel and make Hypixel think you are on vanilla keep `forge = true` as is.

</details>

<details>
  <summary>
    Bypasses for Badlion</summary>
  
  #### Enabling Forge Bypasses
  - To enable all disabled mods on Badlion on Hypixel set `Badlion = false` to `Badlion = true`.

</details>

<details>
  <summary>
    Queuestats Customizations</summary>
  
  #### Customizing Lilith Stat-checking
  - The default stat checking mode of Lilith is to show the overall gamemode stats. For example, if you were to queue a solo bridge game, Lilith will show the opponent's bridge overall stats. If you would like to set the stat checking mode to all duels gamemodes overall set `overall = false` to `overall = true`. You will have to scroll down a bit to find this.
  - If you would like to see your own stats as well as your opponent's set `ShowOwnStats = false` to `ShowownStats = true`.

</details>

<br />

### Inserting your credentials
- Scroll down your toml file until you see a line titled `[server.authentication]`. This is where you will input your credentials.
- Note: If you are concerned about your account security, know that any account details you enter are stored locally on your pc and can't be viewed by the Lilith developers even if they wanted to. The only data we collect and store is your unique Hardware ID and discord tag, which is used for the licensing system. For more information, see our Privacy Policy.

<details>
  <summary>
       For Microsoft Accounts</summary>
     
  #### Microsoft Authentication 
  1. **You will see** `ExampleMicrosoftAccount = ['microsoft.account.email@example.com', '', 'microsoft']`
  2. **Replace** `ExampleMicrosoftAccount` with your Minecraft Account Username, also known as your In Game Name. 
  3. **Replace** `microsoft.account.email@example.com` with your email address accociated with your Microsoft Account.
  
     **Note: do NOT replace** `microsoft` or the blank field `''` with any other text.
  
</details>

<details>
  <summary>
       For Mojang Accounts</summary>
     
  #### Mojang Authentication 
  1. You will see `ExampleMojangAccount = ['mojang.account.email@example.com', 'password goes here!']`
  2. **Replace** `ExampleMojangAccount` with your Minecraft Account Username, also known as your In Game Name.
  3. **Replace** `mojang.account.email@example.com` with your email address accociated with your Mojang Account.
  4. **Replace** `password goes here!` with the password you use to log into your Mojang Account.
  
</details>

<details>
  <summary>
    Example TOML File</summary>
  
  #### Sample `[server.authentication]` TOML File Section

</details>

<br />

## Running Lilith
- Now that you are finished configuring your config file, go to the top left corner of notepad, click file then save. You are now safe to close the toml file.
- Relaunch the Lilith executable by double-clicking on it. This will be how you launch Lilith in the future. You should see Lilith say it loaded your customized toml file.

<br />

## Connecting to Localhost

### Creating a Localhost Server
- Note: In order for Lilith to work properly throughout your session, it needs to be running. A popular way people avoid having the running lilith console get in their way is minimizing it to their task bar after initially launching it.
- Now in Minecraft go to `Multiplayer` -> `Add Server` and for the server name type `Lilith Proxy`. For the server address enter `localhost`. This will create a new server in your server list for you to connect to Hpixel on. 
- To connect to Hypixel with Lilith enabled, just join this new server!
- For the first time you try and connected to Hypixel, you will most likely see a screen stuck on `Downloading terrain...`. This is perfectly normal, you just haven't authenticated with Microsoft yet. Do not click disconnect.

<details>
  <summary>
    Example Localhost Server</summary>
  
  #### Example Localhost Server

</details>

<br/>

### Microsoft Authentication
- Alt-tab over to your running Lilith executable. You should see a message with a link to authenticate with microsoft and a correspond code after it. Copy paste the link into a search browswer of your choice and enter the the code. You may be asked if you would like to give this file access; click yes. 
- From here, please log in with the microsoft email associated with the ign you are trying to log in with. If it's prompting you to sign in with a different email, simply click the blue link that says `sign in with a different microsoft account` to sign in to the proper one. 
- After you are done signing in, you should see a big red error message in your console. Don't be alarmed, this is a good error message. Simply recconect to the localhost server you made and Lilith should work properly!
- Note: Lilith will only work if you are connected to the localhost server. If you attempt to connect to hypixel normally, it won't work.

<br/>

## Optional Enhancements

#### Free

<details>
  <summary>
    Enabling Hypixel Mods</summary>
  
  #### Enabling Hypixel Mods

</details>

<br/>

#### Requires Premium

<details>
  <summary>
    Customizing Questats Appearance</summary>
  
  #### Questats Customization

</details>


[lilithdownload]: https://github.com/GhqstMC/LilithReleases/releases/download/0.6.0-alpha.3/lilith-win-0-6-0-alpha-3.exe