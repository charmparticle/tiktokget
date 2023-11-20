tiktokget hasn't been working for some time now, as tiktok has updated their web page to block selenium with captchas and other such nonsense. Thus, I'm reverting to a basic shellscript, with simpler functionality.

# tiktokget
A tiktok downloader bash script for Linux (and probably all other POSIX-compatible systems). Downloads tiktok videos using yt-dlp

**Prerequisites**

You'll need:

 * [yt-dlp](https://github.com/yt-dlp/yt-dlp/) and [most of it's dependancies (pycryptodomex not required)](https://github.com/yt-dlp/yt-dlp/blob/master/requirements.txt) for getting videos without watermark
 * a linux userland with the usual utilities (bash, grep, tr) -- if you're on windows, your best bet is to use wsl.

I have replaced my python script with a simpler bash script. This script can be invoked as follows:

1. place tiktok videos you want to download in a plain text file, with 1 url per line
2. invoke tiktokget: `./tiktokget thefile`, where thefile is the hypothetical name of the text file you created.

bear in mind, since this is a bash script, you have to be mindful of spaces. Don't put spaces in the filename, or at least quote the filename if you do that.

