![lyrics-scraper-main](https://user-images.githubusercontent.com/96835724/228019346-457f6ade-41ed-43a7-affa-0dbab41d694c.gif)


<h1 align="center"> <a href="https://github.com/FantoX001/lyrics-scraper">@fantox001/lyrics-scraper </a>
</h1>

<h4 align="center"> The simplest yet most powerful <a href="https://genius.com/">Genius Lyrics </a> scrapper
</h4>

<br>

## 💠 Description:
- This is a Scrapper which can scrap and give you lyrics of any song that's available on [Genius Offitial Site](https://genius.com/). 
- This can return both album thumbnail and lyrics if they are available through thw power of web scraping.
- Scraping an website is not always allowed by the website owners. This project is made for educational purposes only.

<br>

## 💫 Installation:

```
npm i @fantox001/lyrics-scraper
```

## 🧩 Usage:
- Make sure to always use an asynchronous function to fetch

### Metod 1:

```
const {getThumbnail, getLyrics} = require('@fantox001/lyrics-scraper');

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

```
const {getThumbnail, getLyrics} = require('@fantox001/lyrics-scraper');

const query = "Heat Waves";

getThumbnail(query).then((thumbnailUrl) => {
    console.log(thumbnailUrl);
});

getLyrics(query).then((lyrics) => {
    console.log(lyrics);
});

```