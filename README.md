# Scraper Sosmed  

[![NPM Version](https://img.shields.io/npm/v/scraper-sosmed.svg)](https://www.npmjs.com/package/scraper-sosmed)  
[![Linux Support](https://img.shields.io/badge/platform-Linux-blue.svg)](https://www.npmjs.com/package/scraper-sosmed)  
[![Windows Support](https://img.shields.io/badge/platform-Windows-blue.svg)](https://www.npmjs.com/package/scraper-sosmed)  
[![License](https://img.shields.io/github/license/AntonThomzz/scraper-sosmed)](LICENSE)  

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
   ton.twdl("https://www.tiktok.com/@omagadsus/video/7025456384175017243?is_from_webapp=1&sender_device=pc&web_id6982004129280116226")
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

## Features  
- Supports terminal CLI and code integration.  
- Compatible with multiple social media platforms.  
- Easy to integrate with other projects.  

## License  
This module is licensed under the [Anton License](LICENSE), which prohibits modifying the source code without written permission.
