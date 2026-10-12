# XFetch

Download videos, images, and GIFs from X (Twitter) with one click.

**[Get XFetch on the Chrome Web Store](https://chromewebstore.google.com/detail/xfetch-%E2%80%94-x-twitter-video/mlnfmnjccjcbimjfblnlhidfmooocepi)**

![Download button on a tweet](https://raw.githubusercontent.com/SSalem00/assets/main/screenshot.png)

## Why XFetch

Twitter "GIFs" are actually MP4s. Most downloaders hand you that MP4 or send you to a converter site. XFetch turns them into real animated `.gif` files right in your browser. No uploads, no extra steps.

## Features

- Download button added to every tweet with video, GIFs, or images
- Real `.gif` output, converted locally
- Live conversion progress shown on the button
- Works on twitter.com and x.com

## Settings

Right-click the extension icon and choose **Options**.

- **GIF conversion**: toggle on or off (off saves the original MP4 instead)
- **Quality preset**: Low (360p, 10fps), Medium (480p, 15fps), High (720p, 24fps)
- **Filename template**: supports `{username}`, `{tweetid}`, `{date}`, `{type}`, `{index}` tokens

## Notes

- Does not work on private or protected tweets.
- Higher quality presets produce larger files and take longer. Medium is a good default.
- Uses X's public syndication endpoint. Personal use only, please respect X's ToS.

## Stack

Plain JS, Manifest V3, no build step. [gifenc](https://github.com/mattdesl/gifenc) handles GIF encoding inside an offscreen document.

## Privacy

See [PRIVACY.md](PRIVACY.md).
