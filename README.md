![ZenBlock Logo](https://media.discordapp.net/attachments/1289219665913970700/1290017598406135818/icon-120x120.png?ex=66faee02&is=66f99c82&hm=5765f664a2bb8a9faa7d70d5916adb32afa1043bd7403d16a301ff386e341259&=&format=webp&quality=lossless)

# Zenblock: Friendly Youtube™ Adblock
This was posted over Reddit a few months ago, [Apparently Ad Blockers are not allowed on Youtube. Is this a new thing they've implemented?](https://www.reddit.com/r/youtube/comments/13cfdbi/apparently_ad_blockers_are_not_allowed_on_youtube/?rdt=64832) and judging by all the recent comments and posts all over [r/youtube](https://www.reddit.com/r/youtube/), this change was just rolled out on a larger scale.

This blocker is designed to monitor advertisements, automatically seek the ads, and skip them. It's important to note that this doesn't classify as traditional ad blocking, as the ad content is technically "loaded".

Nevertheless, the extension's underlying logic enables it to fast-forward through the ad content to its conclusion. The entire process is optimized to occur within an extremely brief timeframe, typically <=100 milliseconds, ensuring a smooth and uninterrupted user experience.

The upcoming version will utilize a custom 
```MutationObserver```with polyfill to ensure compatibility with older browsers. This was the initial reason for not implementing ```MO``` from the start.

The next version will expand onto YouTube Music 🎉 and will have a 
__"Blocked Ads"__ Counter while including other niche features as well as proposed bug fixes.

As this project has demanded a substantial amount of time, the repository will transition to an  _open-core model for ongoing maintenance and updates._ 
 
## Features
This extension effectively eliminates all categories of YouTube advertisements:

__Category 1:__ Ads visible on the homepage.

__Category 2:__ Ads overlaid atop the suggested video list.

__Category 3:__ Ads displayed below the video description.

> Starting on April 6th, 2023, the “Overlay ads” ad format will no longer appear on YouTube to help improve the viewer experience and shift engagement to higher-performing ad formats on desktop and mobile devices. Overlay ads are a legacy ad format that is only served on desktops and are disruptive for viewers.

__Category 4:__ Skippable 5-second-must-be-watched video ads, which may be positioned at the video's start, midway, or at the end.

__Category 5:__ Ads similar to Category 4, but with two consecutive video ads instead of one.

__Category 6:__ Inescapable 10-second video ads, which must be watched.

## FAQ
### 1. __It is not working!__

You will have to __disable other adblockers as they are getting detected.__ It's not due to ZenBlock as the technique it uses is completely different than other adblockers. It's hacky but it works and Google can't do jack _(for the most part)._

Some of the extensions that do not and do work with ZenBlock are listed down below,

| Name of the extension  | Getting detected |
| ------------- | ------------- |
| uBlock Origin  | ✔️ |
| Enhancer For Youtube | ✔️  |
| SponsorBlock for YouTube  | ❌ _(probably)_ |
| Return YouTube Dislike | ❌  |
| Malwarebytes extension | ✔️ |
| Brave in-built adblock | ✔️  |
| Firefox in-built adblock | ✔️ |

> You can also add youtube.com to the exception list for domains on other adblockers (uBlock Origin, AdBlock) and then download ZenBlock to override regular Adblock being prioritized on YouTube while the conventional adblocker will work across the remainder of the Internet.

Note: If you're still getting YouTube's Adblock warning, look at your extensions, and disable extensions one by one until you find your culprit. If you still can't find it, change your browser to Chrome (as it has no built-in adblocker) and test again. If it still doesn't work, then and only then create an [issue](https://github.com/T4bzzz/ZenBlock-YouTube-AdBlock/issues).

### 2. Why there's no privacy policy?
There’s no privacy policy as there’s no data collection at all, not even analytical data for error reporting. Everything happens locally. No remote connections are made, nada!

### 3.How do I use it for my phone?
Unfortunately, there’s no app or anything. You cannot install Chrome extensions on the Chrome browser on Android, but several Chromium-based third-party browsers support extensions (e.g. Brave Browser).

> Note: You will have to leave the YouTube app and watch over a browser (not very elegant, sorry)

## Install ZenBlock to Opera, Edge, Brave and Safari
This section explains how to install the extension utilizing the developer mode as well as Chromium-based browsers, 
![installing chrome extension in dev mode](https://camo.githubusercontent.com/32cef14259cb081f2c2b081a4611206c12b871bfa22c8f98fc8c90863612f343/68747470733a2f2f62617368766c61732e636f6d2f626c6f672f696e7374616c6c2d6368726f6d652d657874656e73696f6e2d696e2d646576656c6f7065722d6d6f64652f6578616d706c652e676966)

### Opera & Edge
Go to the extensions manager page for Opera (opera://extensions) or Edge (edge://extensions), turn on developer mode, and click on Load Unpacked.

### Brave Browser
You can visit the Chrome Web Store and download the extension.

### Install on Safari @ macOS
1. Download the Userscripts from the App Store

2. To open Userscripts and enable Safari extensions settings, open Userscripts (```userscriptsurlscheme://```), then select the checkbox next to Userscripts.

3. Click on the Userscripts icon at the top of Safari to open the script editor and create a new JS file. Then, copy the code from fadblock.user.js and paste it into the newly created JS file.

## Show your support
Think about making a tiny one-time contribution to keep enjoying ZenBlock with extended support.
Star (⭐) this repository and consider following me on GitHub if you're using the free version.

## Disclaimer
This software is provided for educational purposes only and is provided "AS IS", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and non-infringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software or the use or other dealings in the software.
