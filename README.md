# hrejterzy-subs
A community effort to make subtitles for videos of the HRejterzy YouTube channel

# Format
Currently I'm using SubRip files, synced to videos downloaded from YouTube with [`youtube-dl`](https://youtube-dl.org/).

# How to make subtitles
I use [GNOME subtitles](http://www.gnomesubtitles.org/), but the software isn't important. Download the video, open it in your editor and start writing. After you're done, just fork the repository, add the new file and send a pull request.

# Languages
Feel free to add any language you want, but I can't guarantee quality for languages other than English.

# How to add subtitles to downloaded videos
You need to have [`ffmpeg`](https://ffmpeg.org/) installed. Just execute `ffmpeg -i "video.mkv" -i "subtitle.srt" -vcodec copy -acodec copy "video (sub).mkv"`, where `video.mkv` is the file you downloaded and `subtitle.srt` is the file you created.