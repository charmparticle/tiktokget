# tiktokget
A tiktok downloader for Linux (and probably all other POSIX-compatible systems). Downloads all the TikTok videos of a user via providing their username, with or without watermark.

**Prerequisites**

You'll need:

 * [Firefox](https://www.mozilla.org/en-US/firefox/new/)
 * [gecko-driver](https://github.com/mozilla/geckodriver/releases)
 * [Python 3.x](https://www.python.org/)
 * [yt-dlp](https://github.com/yt-dlp/yt-dlp/) and [most of it's dependancies (pycryptodomex not required)](https://github.com/yt-dlp/yt-dlp/blob/master/requirements.txt) for getting videos without watermark
 
 Simply install python 3.x using your package manager or the standard distribution, then install tiktokget with:
 
     pip3 install tiktokget
 
 Invocation is simple:
 
     tiktokget username
 
 Will download every video (without watermarks) by username, into a folder, also named after their username.
 The videos will be titled their title in tiktok, prefixed by their ID number.

 To download with watermarks, or without the use of yt-dlp, use:

     tiktokget -w username

or

    tiktokget username -w

Whichever one floats your boat.
 
to get help with usage, simply invoke tiktokget without any arguments, ie:

    tiktokget

I recently added -f, which runs selenium in GUI mode, so you can interact with the browser. This should help with failed downloads.
