Basic ruby podcast alarm script. Very new. Still testing. will:
  1. put computer to sleep for a specified time
  2. wake up and play a podcast:
     - If user turns off podcast, it will keep time of podcast for next use
     - If podcast plays out, it will play music to ensure user awake, and mark podcast completed

- requires vlc from which it uses cvlc
- requires ubuntu from which it uses amixer, rtcwake
- requires ruby
- requires folder with podcasts in it (settable under podlarm.json)
- requires backup folder with music in it (settable under podlarm.json)
- requires custom setup in podlarm.json

setup:

  - podcasts downloaded, I highly recomend vlc and earwolf rss for downloading podcasts,
    but any vlc media file works aslong as it in the right direcory.
   
  - music in another folder that will play after podcast (for instance if podcast was almost over and it plays out)
   folders customset in podlarm.json

Optional download steps for podcasts:
   - Podcast downloading with vlc: https://www.vlchelp.com/how-subscribe-podcasts-vlc-media-player/
   - obtaining Earwolf rss links for the above vlc podcast subscription
     1. go to podcast page (https://www.earwolf.com/show/hello-from-the-magic-tavern/)
     2. right click rss button, looks like https://github.com/LukeClancy/podlarm/blob/master/Screenshot%20from%202020-06-25%2015-20-18.jpg
     3. copy link location, and use that in vlc

call the utility like "podlarm 8 15" for 8 hours 15 minutes of sleep. note podcasts will be played in ascii alphabetical order. I wrote this for myself to improve my morning by waking up to some totally-not-real people in a "magic" tavern (so they say...) and other podcasts.

If you find a way to listen to daily podcasts (for instance news) as they come out through the podlarm script, tell me how you did it by editing this README! I will find that useful in the future. I dont think vlc has a feature to automatically download podcasts.
