# Chichewa Bible npm Package

![Static Badge](https://img.shields.io/badge/m2kdevelopments-purple?style=plastic&logo=github&logoColor=purple&label=developer&link=https%3A%2F%2Fgithub.com%2Fm2kdevelopments)
![Static Badge](https://img.shields.io/badge/MIT-green?style=plastic&logo=license&logoColor=green&label=license)
![Static Badge](https://img.shields.io/badge/buy_me_a_coffee-yellow?style=plastic&logo=buymeacoffee&logoColor=yellow&label=support&link=https%3A%2F%2Fwww.buymeacoffee.com%2Fm2kdevelopments)
![Static Badge](https://img.shields.io/badge/paypal-blue?style=plastic&logo=paypal&logoColor=blue&label=support&link=https%3A%2F%2Fpaypal.me%2Fm2kdevelopment)


The **Chichewa Bible** npm package is an open source project that provides developers with a convenient way to access and work with the Chichewa translation of the Bible within their Node.js applications. This package aims to simplify the integration of Chichewa Bible text into various projects, such as language learning apps, Bible study tools, and more.

## Features

- Access verses, chapters, and books of the Chichewa Bible programmatically.
- Retrieve text content in Chichewa for quoting, referencing, and display.
- Flexible search functionality for finding specific passages or keywords.
- Lightweight and easy-to-use API for seamless integration into Node.js applications.
- Continuously updated to reflect the latest versions of the Chichewa Bible text.

## Installation

You can install the Chichewa Bible npm package using npm:

```
npm install chichewa-bible
```
OR
```
yarn add chichewa-bible
```

## Examples
To use the bible-chichewa library to retrieve a verse from the Chichewa Bible, follow these steps:

### Example: Retrieving a Bible Verse
```
const { getVerse, BOOK } = require('bible-chichewa');
const book = BOOK.Genesis;
const chapter = 1;
const verse = 1;

const verseText = getVerse(book, chapter, verse);
console.log(`Verse ${book} ${chapter}:${verse}: ${verseText}`);
```


### Example: Retrieving a Bible Chapter

```
const { getChapter, BOOK } = require('bible-chichewa');

const book = BOOK.Genesis;
const chapter = 1;

const chapterVerses = getChapter(book, chapter);

console.log(`Chapter ${book} ${chapter}:`);
chapterVerses.forEach((verse, index) => {
  console.log(`${index + 1}: ${verse}`);
});

```

### Example: Retrieving a Bible Verses within Range
```
const { getVerses, BOOK } = require('bible-chichewa');

const book = BOOK.Exodus;
const chapter = 20;
const verseStart = 1;
const verseEnd = 5;

const verses = getVerses(book, chapter, verseStart, verseEnd);

console.log(`Verses ${book} ${chapter}:${verseStart}-${verseEnd}:`);
verses.forEach((verse, index) => {
  console.log(`${verseStart + index}: ${verse}`);
});

```


<a href="https://www.buymeacoffee.com/m2kdevelopments" target="_blank">
<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
</a>
