## scraper-sosmed

[![NPM Version](https://img.shields.io/npm/v/scraper-sosmed.svg)](https://www.npmjs.com/package/scraper-sosmed)

## install module

- Here's how to install the package:

```bash
npm install anton-uploader
```

- if you want to directly use the package in the terminal follow these steps:

```bash
npm install -g scraper-sosmed
```

### usage

```bash
dlp https://vt.tiktok.com/ZS6MNC8Yk
```

## example in code

- FACEBOOK

```javascript
const ton = require("scraper-sosmed");

(async () => {
   ton.fbdl("https://www.facebook.com/share/r/yDEyvFLnCWsnA4nt/?mibextid=rS40aB7S9Ucbxw6v")
      .then(data => consol.log(data))
      .catc(err => console.log(err))
})();
```

- FACEBOOK2

```javascript
const ton = require("scraper-sosmed");

(async () => {
   ton.fbdlV2("https://www.facebook.com/share/r/yDEyvFLnCWsnA4nt/?mibextid=rS40aB7S9Ucbxw6v")
      .then(data => consol.log(data))
      .catc(err => console.log(err))
})();
```

- INSTAGRAM

```javascript
const ton = require("scraper-sosmed");

(async () => {
   ton.igdl("https://www.instagram.com/reel/DD_RN94Sy-0/?igsh=MTRwZGZhc2Z6cjVtcQ==")
      .then(data => consol.log(data))
      .catc(err => console.log(err))
})();
```

- TIKTOK

```javascript
const ton = require("scraper-sosmed");

(async () => {
   ton.ttdl("https://vt.tiktok.com/ZS6MNC8Yk/")
      .then(data => consol.log(data))
      .catc(err => console.log(err))
})();
```
