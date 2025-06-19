<h1 align="center">
  <br>
  <a href="https://play.google.com/store/apps/details?id=com.banglalink.toffee">
    <img src="https://github.com/Jeshan-akand/Toffee-Channels-Link-Headers/blob/main/images/toffee_logo.jpeg" alt="🔥 Toffee 🔥" width="200">
  </a>
  <br>
  🔥 Toffee Channels Auto-Updater 🔥
  <br>
</h1>

<h2 align="center">Auto-updating script for Toffee App Channel Links and Headers (every 30 minutes)</h2>

<p align="center">
  <a href="https://www.python.org/">
    <img src="https://img.shields.io/badge/Made_With-Python_3.12%2B-blue" alt="Python">
  </a>
  <a href="mailto:bullredeyes@gmail.com">
    <img src="https://img.shields.io/badge/Byte_Capsule-%E2%98%BC-green.svg" alt="Byte Capsule">
  </a>
  <a href="https://play.google.com/store/apps/details?id=com.banglalink.toffee">
    <img src="https://img.shields.io/badge/App-Toffee_Live-purple" alt="Toffee App">
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Made%20in-Bangladesh_🇧🇩-green?colorA=%23ff0000&colorB=%23017e40&style=flat-square" alt="Bangladesh">
  </a>
  <a href="https://hits.seeyoufarm.com">
    <img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fbyte-capsule%2FToffee-Channels-Link-Headers&count_bg=%2379C83D&title_bg=%23555555&icon=mattermost.svg&icon_color=%23E7E7E7&title=Visitors+&edge_flat=false" alt="Visitors">
  </a>
</p>

<h1 align="center">
  <a href="https://github.com/Jeshan-akand/Toffee-Channels-Link-Headers/blob/main/images/banner.jpeg">
    <img src="https://github.com/Jeshan-akand/Toffee-Channels-Link-Headers/blob/main/images/banner.jpeg">
  </a>
</h1>

---

## 📒 Introduction

**[Toffee](https://play.google.com/store/apps/details?id=com.banglalink.toffee)** is the #1 entertainment app in Bangladesh with 10M+ downloads. This repo provides a script that auto-updates Toffee channel links and required headers like cookies, DRM tokens, and user-agents.

---

## 💥 Key Features

* ⏰ Updates every 3 minutes using GitHub Actions
* 🎥 Includes premium & standard channel streams
* ✅ Working stream links (.m3u8)
* ✉ Includes all necessary HTTP headers (Cookie, User-Agent, etc.)
* 🔸 Delivered in JSON format
* 🔎 Easy to use in your apps, players, or scripts

---

## 🕹️ How To Use (Developer Guide)

**Auto-updated JSON file:**

➡️ [Toffee Channels JSON](https://raw.githubusercontent.com/Jeshan-akand/Toffee-Channels-Link-Headers/main/toffee_channel_data.json)

```python
import requests

link = "https://raw.githubusercontent.com/Jeshan-akand/Toffee-Channels-Link-Headers/main/toffee_channel_data.json"
data = requests.get(link).json()

for channel in data["channels"]:
    url = channel["link"]
    headers = channel["headers"]
    print("\u2713 Channel Link:", url)
    print("\u2713 Headers:", headers)

    response = requests.get(url, headers=headers)
    print("\u2713 Server Response:\n", response.text)
```

> Works with **Python 3+**, but you can adapt it to any programming language.

---

---

## 🎥 How To Play

### 📱 Android

* Use **Network Stream Player** – [Download](https://play.google.com/store/apps/details?id=com.genuine.leone)
* Add playlist: [NS Player Playlist](https://raw.githubusercontent.com/Jeshan-akand/Toffee-Channels-Link-Headers/main/toffee_NS_Player.m3u)
* Short Link: [https://s.id/21HEP](https://s.id/21HEP)

### 📺 Android TV

* Use **OTT Navigator** – [Download](https://apkpure.com/ott-navigator-iptv/studio.scillarium.ottnavigator/amp)
* Add playlist: [OTT Playlist](https://raw.githubusercontent.com/Jeshan-akand/Toffee-Channels-Link-Headers/main/toffee_OTT_Navigator.m3u)
* Short Link: [https://s.id/21HEV](https://s.id/21HEV)

<h1 align="center">
 <img src="https://github.com/Jeshan-akand/Toffee-Channels-Link-Headers/blob/main/images/ns_player.jpg">
</h1>
<h1 align="center">
 <img src="https://github.com/Jeshan-akand/Toffee-Channels-Link-Headers/blob/main/images/ott_view.jpg">
</h1>

---

## 🚬 Credits

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code\&pause=100\&color=FF2C10\&background=31FF9400\&width=400\&lines=Made+By+Byte+Capsule)](https://git.io/typing-svg)

---

## 📝 Legal Notice

* ⚠️ **For educational & research purposes only.**
* ❌ Do not use this code to harm, disrupt, or bypass paid content.
* 🚫 If it violates content ownership, kindly report & we will remove it.
* 🇷🇼 **Geo-restricted content**: Only available in **Bangladesh**.

---

## 💰 Support

<a href="https://www.buymeacoffee.com/jeshanakanc" target="_blank">
  <img src="https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png" alt="Buy Me A Coffee" width="174">
</a>

---

## ✉️ Contact Me

* [GitHub](https://github.com/byte-capsule)
* [Email](mailto:jeshanakand2017@gmail.com)
* [Telegram](https://t.me/J_9X_H_9X_N)
* [Facebook Messenger](https://t.me/J_9X_H_9X_N)
