![lyrics-scraper-example](https://user-images.githubusercontent.com/96835724/228140459-6797637f-6911-4582-94a1-43601bee63c4.gif)


<h1 align="center"> <a href="https://github.com/FantoX001/lyrics-scraper">@fantox01/lyrics-scraper </a>
</h1>

<h4 align="center"> The simplest yet most powerful <a href="https://genius.com/">Genius Lyrics </a> scrapper
</h4>

<br>
<p align="center">

<a href="https://www.codefactor.io/repository/github/fantox001/lyrics-scraper">
<img src="https://www.codefactor.io/repository/github/fantox001/lyrics-scraper/badge" alt="CodeFactor" width="120px" /></a>

</p>

<p align="center">
<a href="https://www.npmjs.com/package/@fantox01/lyrics-scraper">
    <img src="https://upload.wikimedia.org/wikipedia/commons/d/db/Npm-logo.svg" width="140px">
</a>
  
</p>

<br>

## 💠 Description:
- This is a Scraper which can scrap and give you lyrics of any song that's available on [Genius Offitial Site](https://genius.com/). 
- This can return both album thumbnail and lyrics if they are available through thw power of web scraping.
- Scraping an website is not always allowed by the website owners. This project is made for educational purposes only.

<br>

## 💫 Installation:

```
npm i @fantox01/lyrics-scraper
```

## 🧩 Usage:
- Make sure to always use an asynchronous function to fetch

### Metod 1:

```js
const {getThumbnail, getLyrics} = require('@fantox01/lyrics-scraper');

async function main() {
    const query = "Heat Waves";
    const thumbnailUrl = await getThumbnail(query);
    const lyrics = await getLyrics(query);

    console.log(thumbnailUrl+"\n\n");
    console.log(lyrics); 
  }
  
  main();
  
```

### Method 2:

```js
const {getThumbnail, getLyrics} = require('@fantox01/lyrics-scraper');

const query = "Heat Waves";

getThumbnail(query).then((thumbnailUrl) => {
    console.log(thumbnailUrl);
});

getLyrics(query).then((lyrics) => {
    console.log(lyrics);
});

```
