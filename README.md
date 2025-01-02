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

## Example of TikTok output  

```bash
{
  status: 200,
  owner: 'AntonThomzz',
  Issues: 'https://github.com/AntonThomz',
  data: {
    id: '7025456384175017243',
    title: 'Rick roll 😱#fyp #foryoupage #meme #sus #rickroll #superidol #😱😱😱😱😱😱😱 😱😱😱',
    play: '1.2M',
    likes: '123.1k',
    comment: '3.3k',
    share: '12.1k',
    download: '13.3k',
    favorit: '5.4k',
    upload: '2021-11-01T04:38:52.000Z',
    region: 'Indonesia',
    duration: '0 menit 18 detik',
    size: '2.8 MB',
    wmsize: '3.0 MB',
    url: 'https://v16m-default.akamaized.net/2fd37b2885b8f10f32ee403a054615f5/677725dd/video/tos/useast2a/tos-useast2a-pve-0037-aiso/386945f914fd4802b14270d18bba7321/?a=0&bti=OUBzOTg7QGo6OjZAL3AjLTAzYCMxNDNg&ch=0&cr=0&dr=0&er=0&lr=all&net=0&cd=0%7C0%7C0%7C0&cv=1&br=2384&bt=1192&cs=0&ds=6&ft=XE5bCqT0majPD12CldNJ3wUOx5EcMeF~O5&mime_type=video_mp4&qs=0&rc=ZGlnM2g6PDY2aTZpODlmOUBpMzNwZjo6ZmlwODMzZjgzM0AwX2IyXmIwXjIxLl9eNC8wYSNqXl4xcjRfcnNgLS1kL2Nzcw%3D%3D&vvpl=1&l=20250102174826B4CFFE87B3ED2C34E91B&btag=e000b8000',
    wmplay: 'https://v16m-default.akamaized.net/250458e05fb1c3c7930d598c8a2ef7cd/677725dd/video/tos/useast2a/tos-useast2a-pve-0037-aiso/c01db01fef1f4c0a969397060facc459/?a=0&bti=OUBzOTg7QGo6OjZAL3AjLTAzYCMxNDNg&ch=0&cr=0&dr=0&er=0&lr=all&net=0&cd=0%7C0%7C0%7C0&cv=1&br=2544&bt=1272&cs=0&ds=3&ft=XE5bCqT0majPD12CldNJ3wUOx5EcMeF~O5&mime_type=video_mp4&qs=0&rc=OWdkZWU0OGY5ODo2OjU3OkBpMzNwZjo6ZmlwODMzZjgzM0BfMGFhNDQ1X2MxLjUxYzRhYSNqXl4xcjRfcnNgLS1kL2Nzcw%3D%3D&vvpl=1&l=20250102174826B4CFFE87B3ED2C34E91B&btag=e000b8000',
    music: 'https://sf16-ies-music.tiktokcdn.com/obj/ies-music-aiso/7018923958166752027.mp3',
    info_music: {
      id: '7018924035446786843',
      play: 'https://sf16-ies-music.tiktokcdn.com/obj/ies-music-aiso/7018923958166752027.mp3',
      title: 'Duy Anh Nhái Superidol kiểu',
      cover: 'https://p16-sign-useast2a.tiktokcdn.com/tos-useast2a-avt-0068-giso/f3ae80ca20e8073976c8f0582c10708c~tplv-tiktokx-cropcenter:1080:1080.jpeg?dr=14579&nonce=6923&refresh_token=b0870e5113c7b9298e0920a10106a5d9&x-expires=1735923600&x-signature=OZNryYg%2FxVubrB2lnV444tMHAj0%3D&idc=maliva&ps=13740610&shcp=d05b14bd&shp=45126217&t=4d5b0474',
      author: 'Quang khuất bị ngu',
      duration: '0 menit 14 detik',
      album: '-'
    }
  }
}
```

## Example of Facebook output

```bash
{                                                                                          status: 200,
  owner: 'AntonThomzz',
  issues: 'https://github.com/AntonThomz',
  data: {
    HD: {
      quality: '720p (HD)',
      url: 'https://ssscdn.io/getmyfb/NDIzMjExMjM0NTYzMjEzM2dNRUhLdVRycXVLSXhVdGZHMXFsV1pIK0hWTXlRK3oxaE1IVEZRclFrYnoyR2tZRjdzQU1rekkrRUtWL1REUTM2NjMrRlNxT2h2N2hpR1psRnlkVC94MmFoSXRRU0x6bmhPcm4rdkRmVURWZ3FIN1F4dmVPcGcycjRiZjZIejhUd3hmclVlbmFZS3NhbnRrTzVpMGUwSCsvc2g4NkFsRXNZVy8xekZVU2RTZS9YZ0VlWE1BV3JBemgwYW1CL1Fsb3pRekZRVmFoS2t3OWhvQUVsUTJiNzFIc2ZXakhRbGpuaVV5UHk0OFFWU0F1NmN1c1FTV205YTJPWkNVNnZBSXYyazZjdDFld0swaGhoNHVKOGRrRjVyMng3RnZnNFFlSGVIbDMvSi9PZitYT3d5c0NCQkVqeTBGeXpaNW5STFNSWXEvWDFsUGYwTE5xQUkvWmFsMXVPbmdOa3crRU5Wc2VKbUNDa2p4cXJzZkJNUU9MV2p6RHZ1UjJnVkI1VW1iU01zTm5SV1RBdi9SZGYrT3d6T0tKdE1QNml5Z1lxejgxdm9mUVJ1VmNFenJrK0x5QnZsZDZGV2gvMXlhUzVKQnpFUXJpWC9QUmNQaEwrK1VsMlV5M3JvSjE0YjFkdXB2dnhONVFhMHJFak5QYU1PQjFxck53VmptdkZLNWUwYTRCMnVRQm9iTTAvM3UyV296OFFPTjZQOVV1WDJGWkdrVVZZSTlpVUVoazIzZE1wbk1DR2NpOGhqcy9NcmZoK3NLTWY1aThJUGptMzFKRWd4Nk9UTm5PN3ZKLzNoZnFXbnBkR295RmZrbm9rV2Q3ZVFySFFCTmxyb1BmLzhGaWk5Q1p4TWtyTnhmZktNdEdUR2FVSEFvbC92ZThvVlJTdnQ2WSt3MXYxWnByWUxKMTlZQ3FVRjNQSnhKcTdQUUpqbU1iVk9pcXhoZVdmeVFkSU1lMGhBNnlsREJMN0c4blZWYXZ3Y20reEtZUWtldW0xQW1PcDdQbi8vY28ybUI4SVhHcitKVzNCd0pYZEUrd3RyWXc2eEtXUEJsamU1NFRIUmo2bjZVNTltb0lyVnQ3d3VENU5VWm1ERlpWQjd0KzlMQWpsckJldjlEdkZTUVBlYksyWE1wOTdhVHFRdHdBczI1QXFZKzhuMmNTTGFOTGJQcGF1NG0wdkMycU1CNU9Lc29qUXNDczU5L0h5OWQxN1JodERJeDNac2RHb3RGakUvS2FVWm90UURGZVB6eDZ0VVIraitwU2ZXY21jeEhTT25pZTROekI1V2pVZGJnNDE1SjRsWnBUUmN5T0RjVjJsL1Mrd05teERuK1hWTVNTaStaS0s1eExHbG13L01aNldERTVPajE4WitxMGxkNlNoUU9ReVgxWWxRPT0='
    },
    SD: {
      quality: '360p (SD)',
      url: 'https://ssscdn.io/getmyfb/NDIzMjExMjM0NTYzMjEzM2dNRUhLdVRycXVLSXhVdGZHMXFsV1pIK0hWTXlRK3oxaE1IVEZRclFrYnoyR2tZRjdzQU1rekkrRUtWL1REUTMxZi9jbFYyMFo5OGl0OTgzem9DYUV0SlVQdldsMnJpOHBReTI0VHlMM1orOENKSFhzVzFSdXAvV3FyelJjVnpoU043YXNoUEJ1dTRUV1AwY3JMT0tRM0x3TW5RQ3hJc0lzbTMxVUUrY0VnaWZCb0NzbVFFc1U3OEJHVWh3dHJ2akVBVFRLWmdrR0FrVnNUT0hsQ0U5ZEVCTjNHQkhsekZjVFV3MjhkV2dOL1VrZnlCamJ1bnFHNlpCK0s3TGVqaGVYcW15RVh0dlRrL0p6eDl4V2dXekZkSStxQVk1d3lOTVVXREpIYUtzeHBvT3p4Rmxra09Uc1lvNkUrL1VGMjlFRHo4RG80cXIyTHFYWGVDc3gyVWRIZ3hqNXYxQTBNd2d1UG90RFpMWTJxNElTRi9GSUtYdkNrNmFKdGpaU2h1MGpKWmc4ZERYTnYzcWlBK0EvaktTNnUzK0JUcE4wZWxDbEswWnBpdmRLWXZrNFRibVlYTS9wMGNYYnk4K2tZbjhwaE9JY2pxOEhjNjd5ZUdWRGRkcSs4RFpjand0eUZrOXpPK1dUbGp2b0RjdVJSak5WbmJvOEszUUVuRlhOS00rekZIeitBREdRN3dKcE9IRTEwbUdFUUVDSGhEL2creGxMVWFETkdDYTdPYmRVQkNjZ0FYOXBTREUwNTJudWlBUnpXV2lPbWNjdlYxZjNwWnY1Znh6aVRscFN6eGNuWERTUEN5L3hNdEo3bXdWbGpodFBaL0hZdUZTOCtnSTh2cnM='
    }
  }
}
```
## License  
This module is licensed under the [Anton License](LICENSE), which prohibits modifying the source code without written permission.
