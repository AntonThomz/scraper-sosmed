<h1 align="center">
<br>
<br>
<img width="100%" src="https://i.imgur.com/U68ak1j.jpeg" alt="scraper-sosmed">
<br>
<br>
<br>
</h1>

# Scraper Sosmed  

[![NPM Version](https://img.shields.io/npm/v/scraper-sosmed.svg)](https://www.npmjs.com/package/scraper-sosmed)  

## About  
Scraper Sosmed is a **Node.js** module designed to download social media data, including videos, audio, or metadata, from platforms like **Facebook**, **Instagram**, **TikTok**, and others. It can be used directly in the terminal or integrated into your code.  

## Installation  

### For Code Usage  
```bash
npm install scraper-sosmed
```  

### For Terminal Usage  
```bash
npm install -g scraper-sosmed
```  

## Usage in Terminal  
Use the `dlp` command:  
```bash
dlp https://vt.tiktok.com/ZS6MNC8Yk
```
## Screenshot Website
Apart from the social media scraping feature, we also have a feature for taking website image
```bash
ssweb -hp https://www.antoncodder.online
ssweb -pc https://www.antoncodder.online
```

## Example in Code  

### Facebook Downloader  
```javascript
const ton = require("scraper-sosmed");

(async () => {
   ton.fbdl("https://www.facebook.com/share/r/yDEyvFLnCWsnA4nt/?mibextid=rS40aB7S9Ucbxw6v")
      .then(data => console.log(data))
      .catch(err => console.log(err));
})();
```  

### Facebook Downloader V2  
```javascript
const ton = require("scraper-sosmed");

(async () => {
   ton.fbdlV2("https://www.facebook.com/share/r/yDEyvFLnCWsnA4nt/?mibextid=rS40aB7S9Ucbxw6v")
      .then(data => console.log(data))
      .catch(err => console.log(err));
})();
```  

### Instagram Downloader  
```javascript
const ton = require("scraper-sosmed");

(async () => {
   ton.igdl("https://www.instagram.com/reel/DD_RN94Sy-0/?igsh=MTRwZGZhc2Z6cjVtcQ==")
      .then(data => console.log(data))
      .catch(err => console.log(err));
})();
```  

### TikTok Downloader  
```javascript
const ton = require("scraper-sosmed");

(async () => {
   ton.ttdl("https://vt.tiktok.com/ZS6MNC8Yk/")
      .then(data => console.log(data))
      .catch(err => console.log(err));
})();
```

### YouTube Downloader
```javascript
const ton = require("scraper-sosmed");

(async () => {
   ton.ytdl("https://youtube.com/watch?v=JkyrI4Kp7PE")
      .then(data => console.log(data))
      .catch(err => console.log(err));
})();
```

### Twitter Downloader
```javascript
const ton = require("scraper-sosmed");

(async () => {
   ton.twdl("https://twitter.com/gofoodindonesia/status/1229369819511709697")
      .then(data => console.log(data))
      .catch(err => console.log(err));
})();
```  

## Supported Platforms  
- Facebook  
- Instagram  
- TikTok  
- Twitter  
- YouTube

## website screenshot
 Apart from the social media scraping feature, we also have a feature for taking website image

- SSHP 

```javascript
const ton = require("scraper-sosmed");

(async () => {
  ton.sshp("http://www.antoncodde.online")
     .then(data => consol.log(data))
     .catc(err => consol.log(err))
})();
```
- SSPC 

```javascript
const ton = require("scraper-sosmed");

(async () => {
  ton.sspc("http://www.antoncodde.online")
     .then(data => consol.log(data))
     .catc(err => consol.log(err))
})();
```

## License  
This module is licensed under the [Anton License](LICENSE), which prohibits modifying the source code without written permission.
