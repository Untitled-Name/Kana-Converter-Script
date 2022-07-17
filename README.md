# Kana-Converter-Script

## Introduction

This is a Tampermonkey script for randomly converting kanji on Japanese webpages to kana. 

This script uses the gooLabs [Hiragana convert API (ひらがな化API)](https://labs.goo.ne.jp/api/jp/hiragana-translation/) *(Japanese)*.

## How to use

This script can be installed via the [Tampermonkey browser extension](https://www.tampermonkey.net/) by creating a new script and copying the code into the file.

Since this script uses the gooLabs API, it requires a key which can be created for free via [the steps listed on this page](https://labs.goo.ne.jp/apiusage/).

This key can be inserted into `APIKEY` in the config section of the script. The probability for conversion and highlighting characters can also be changed there.

## Purpose

This was created as a response to a request for practice reading Japanese without the aid of kanji. Although many Japanese learners struggle with kanji, many learners who have learned kanji can become reliant on them to the point of struggling with listening to Japanese or reading kana-only Japanese. This script is a passive way to give more kana comprehension practice.

## Issues

Theoretically this script could work on any webpage with Japanese text, but in practice it has not been tested on many sites. It has mainly been tested on Wikipedia, and briefly on NHK news. If used, many sites may needed to be added to the exclusion list if displaying kanji is necessary.

The API call is quite slow so even as few as 30 changes can take several seconds. Hundreds of changes on a webpage may take minutes. The API will also occassionally return an error, but if this is done, the item will be skipped.
