# tiktokget
A tiktok downloader. Downloads all tiktok videos for a username.

**Prerequisites**

You'll need:

 * [Firefox](https://www.mozilla.org/en-US/firefox/new/)
 * [gecko-driver](https://github.com/mozilla/geckodriver/releases)
 * [python](https://www.python.org/)
 
 Simply install python 3.x using your package manager or the standard distribution, then install tiktokget with:
 
     pip3 install tiktokget
     
 or in Windows:
 
     py -m pip install tiktokget
 
 Invocation is simple:
 
     tiktokget username
 
 will download every video by username, into a folder, also named username.
 The videos will be titled their title in tiktok, prefixed by their sequence number.
 
