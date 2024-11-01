# If you use as package

......

# YouTube Data Scraper

A simple Node.js package that uses Puppeteer to scrape PO Token and visitor data from YouTube video embeds without opening a browser window.

## Features

- Extracts PO Token and visitor data from YouTube embed URLs.
- Runs in headless mode, making it efficient for server-side usage.
- Easy to integrate into existing Node.js projects.

## Installation

Install the package using npm:

```bash
npm install auto-youtube-scraper-data
```

## Usage

Import the package and use the scrapeYouTubeData function to scrape data from a YouTube embed URL.

```javascript
import scrapeYouTubeData from "auto-youtube-scraper-data";

scrapeYouTubeData(videoId, ({PO_TOKEN, VISITOR_DATA }) => {
    //Whatever you want
});
```

## Output

The function will log the extracted PO Token and visitor data to the console:

```bash
PO_TOKEN: <PO_TOKEN_HERE>
VISITOR_DATA: <VISITOR_DATA_HERE>
```

## API

`scrapeYouTubeData(videoId, callback({PO_TOKEN, VISITOR_DATA }))`

videoId: string - The URL of the YouTube embed from which you want to scrape data.
This function launches a headless browser, navigates to the specified YouTube embed URL, and logs the PO Token and visitor data to the console.



## Edit from Fork

Added a callback that enables you to get the tokens from your code