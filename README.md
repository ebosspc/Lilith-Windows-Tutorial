<!--- Special Thanks to Sam (https://github.com/Scherso) for creating a beautiful formatting template for Lilith tutorials --->
<!--- The majority of this text was written by FireStorm (FireStorm#1000) --->

<!--- Lilith Logo Header --->
<p align="center">
    <img src="https://github.com/GhqstMC/LilithReleases/blob/main/assets/title.png" style="width: 45%">
</p>

<h1 align="center">

  [Lilith](https://github.com/GhqstMC/LilithReleases) Setup for Windows
  
</h1>

---

## Install Lilith in the proper location

- You can download Lilith for windows [Here][lilithdownload] if you haven't already. You can idenitfy it via the green icon next to its name.
- Go to your desktop and right click on an empty space and create a new folder called Lilith
- Drag and drop the executable file you just downloaded into that folder you created. 
- Note: Lilith WILL NOT work if it isn't in its own dedicated folder. Do not skip this step. Additionally, if you accidentally downloaded the Lilith executable more than once it may have something like a (1) at the end of the name that windows automatically gave it. If this is the case, please right click on the executable in your folder, select rename, and then manually remove the unwanted (1) from the end of its name.

<br />

## Linking Lilith to Your Discord
- Go into your Lilith folder and double click on the exectuable to run it. A new black window should pop up on your screen.
- Inside this window, there will be a blue link. Please copy and paste that link into a browser of your choice and hit enter. Follow the instructions in your browser to properly link your discord. Do not close Lilith while you are doing this.
- Note: You may be asked to give Lilith access to your username and avatar. Just click yes, this is simply to link your discord account with Lilith. 
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
- Note: If you are concerned about your account security, know that any account details you enter are stored locally on your pc and can't be viewed by the Lilith developers even if they wanted to. The only data we collect and store is your unique Hardware ID and discord tag, which is used for the licensing system. For more information, see our [Privacy Policy][LilithDocsFAQ].

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

<br />

## Running Lilith
- Now that you are finished configuring your config file, go to the top left corner of notepad, click file then save. You are now safe to close the toml file.
- Relaunch the Lilith executable by double-clicking on it. This will be how you launch Lilith in the future. You should see Lilith say it loaded your customized toml file.

<br />

## Connecting to Localhost

### Creating a Localhost Server
- Note: In order for Lilith to work properly throughout your session, it needs to be running. A popular way people avoid the running Lilith console getting in their way is minimizing it to their task bar after initially launching it.
- Now in Minecraft go to `Multiplayer` -> `Add Server` and for the server name type `Lilith Proxy`. For the server address enter `localhost`. This will create a new server in your server list for you to connect to Hpixel on. 
- To connect to Hypixel with Lilith enabled, just join this new server!
- For the first time you try and connected to Hypixel, you will most likely see a screen stuck on `Downloading terrain...`. This is perfectly normal, you just haven't authenticated with Microsoft yet. Do not click disconnect.

<br/>

### Microsoft Authentication
- Alt-tab over to your running Lilith executable. You should see a message with a link to authenticate with microsoft and a correspond code after it. Copy paste the link into a search browswer of your choice and enter the the code. You may be asked if you would like to give this file access; click yes. 
- From here, please log in with the microsoft email associated with the ign you are trying to log in with. If it's prompting you to sign in with a different email, simply click the blue link that says `sign in with a different microsoft account` to sign in to the proper one. 
- After you are done signing in, you should see a big red error message in your console. Don't be alarmed, this is a good error message. Simply recconect to the localhost server you made and Lilith should work properly!
- Note: Lilith will only work if you are connected to the localhost server. If you attempt to connect to hypixel normally, it won't work.

<br/>

## Optional Enhancements

### Free

<details>
  <summary>
    Enable Hypixel Mods</summary>
  
  #### Enabling Hypixel Mods
  1. Ensure Lilith, Lunar, and all files relating to Minecraft are closed. Also ensure the Lunar Enable bypasses are off. You can do this by settings `lunar = true` to `lunar = false` in your config, if it isn't already `false`. 
  Note: If you need to use Lunar Enable we reccomend using [Lunar Client QT][LunarClientQT], an open source custom launcher for Lunar. It lets you add custom mods to Lunar called agents that are similar to forge mods in nature. Please note most forge mods won't work with it, as the only agents that will work with it are specially written ones made in [Java Byte Code][JavaByteCode]. Popular agents include an unlocker for Lunar+, every emote, and every cosmetic, similar Lunar bypasses to the ones Lilith offers, and a customizable hurtcamera.
  2. Find the search icon/bar at the bottom of your screen and type Notepad into the searchbar; you should see the Notepad app pop up as an option. DO NOT open it yet.
  3. Right-click on it ad select Run as Administrator. Youll be asked if you want to "allow this app to make changes to your device?". Click Yes
  4. Now that you are running Notepad as an admin, in the top right of the window click File then Open.
  5. Navigate to `C:` -> `Windows` -> `System32` -> `drivers` -> `etc`. This folder may appear blank at first. To show all files, click the dropdown box in the bottom-right of file explorer titled `Text Documents .txt`, then select `All Files`.
  6. **Double-Click** on hosts to open it. You may see several lines starting with `#`. Create a new line at the very bottom of the file below all of the lines starting with `#`.\
  7. Paste the following into that bottom line: `127.0.0.1 hypixel.net.hypixel.io`. Next, save your hosts file and close it.
  8. Relaunch Lilith and Lunar like normal.
  9. **Change** Your Lilith/localhost server address from `localhost` to `hypixel.net.hypixel.io` before connecting.

</details>

<details>
  <summary>
    Add Alts</summary>
  
  #### Adding Alts to Lilith
  **Note: Lilith WILL NOT support mojang accounts in 1.0**
  1. Ensure Lilith and Lunar are closed.
  2. Navigate to the TOML file in your Lilith folder where you previously entered the details of your main minecraft account. Scroll down to the `[server.authentication]` portion of your TOML file. You should see the place where you entered you main's details. You are going to enter your alt's details following the exeact same formatting you used for your main.
  3. Copy the entire line with your main's details to your clipboard by pressing `ctrl` + `c`
  4. Create a new line right underneath the line with your main's details. Paste the line you just copied into this new line.
  5. Replace the ign and email portions in this new line with your alts details following the same formatting rules as you did with your main.
  6. Save your toml file and close it. Launch Lilith and Minecraft.In Minecraft, sign into your alt and connect to the Lilith localhost server.
  7. Just like you did with your main, authenticate with Microsft with the email associated with the ign you are trying to log in with. You may have to click on `sign in with a different microsoft account` to choose the right email to sign in with.
  8. To add more alts just follow the above steps to add a new alt on each line and authenticating each one with microsoft one by one.

</details>

<br/>

### Requires Premium

<details>
  <summary>
    How to Get Premium</summary>
  
  #### Obtaining a Premium License
  - If you would like to purcahse premium please DM an admin or developer. You can contact us via the [Lilith Discord Server][LilithDiscord]. Licenses are $10 for lifetime access to all Lilith premium updates and features. Server boosters will also receive 1 month of premium for each month they boost the server.

</details>

<details>
  <summary>
    Custom Queuestats</summary>
  
  #### Making One-line Stats
  Note: This feature has been temporarily **DISABLED** until 1.0 releases.

  <br/>

  #### Custom Color Coding
  Note: This feature has been temporarily **DISABLED** until 1.0 releases.

</details>

<details>
  <summary>
    Autododge</summary>
  
  #### Customizing Autododge
  Note: This feature has been temporarily **DISABLED** until 1.0 releases.

</details>

<br/>

## Troubleshooting
- If none of the solutions below work for you, please create a ticket in the [Lilith Discord Server][LilithDiscord].

<details>
  <summary>
    Java.net connection excpetion In Game</summary>
  
  #### Lilith Isn't Running
  - When you connected to localhost you didn't make sure to have Lilith running while you were doing so. Please launch Lilith and keep it running while you are connected to localhost.

</details>

<details>
  <summary>
    End, SocketClosed</summary>
  
  #### Details Not In TOML File
  - You have not added your details to your TOML file, or if you have, they were added improperly. Please see the examples above in the `Inserting Your Credentials` section fo this guide to ensure you entered your details properly.
  - Note: If you are changing your TOML file, be sure to save it and relaunch Lilith to load your changes properly. 

</details>

<details>
  <summary>
    Bad Atom Value at line ___</summary>
  
  #### Bad TOML formatting
  - You didn't format your TOML file properly according to the `Inserting Your Credentials` section in the guide and Lilith is rejecting the improper formatting. Please see the examples above to ensure it is formatted correctly.
  - Note: If you are changing your TOML file, be sure to save it and relaunch Lilith to load your changes properly.

</details>

<details>
  <summary>
    Unexpected token in JSON at position ___</summary>
  
  #### Bad TOML formatting
  - You didn't format your TOML file properly according to the `Inserting Your Credentials` section in the guide and Lilith is rejecting the improper formatting. Please see the examples above to ensure it is formatted correctly.
  Note: If you are changing your TOML file, be sure to save it and relaunch Lilith to load your changes properly.

</details>

[LilithDownload]: https://github.com/GhqstMC/LilithReleases/releases/download/0.6.0-alpha.3/lilith-win-0-6-0-alpha-3.exe
[LunarClientQT]: https://github.com/Nilsen84/lunar-client-qt
[JavaByteCode]: https://en.wikipedia.org/wiki/Java_bytecode
[LilithDiscord]: htt[s://discord.gg/lilith
[LilithDocsFAQ]: https://docs.lilithmod.xyz/#/FAQ
