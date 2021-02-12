# debian-youtube-dl
Dockerfile for debian-youtube-dl

###

`docker build -t [My_Container] .` 

### Docker Run
`docker run -i -t -v [My_Download_Dir]:/Downloads chenchiwang/debian-youtube-dl /bin/bash`

### Youtube-dl Run and download file to `[My_Download_Dir]`
* `mp3 [video_website]`  convert download_file to mp3.
* `video_o [video_website]` convert download_file to mp4. 
* `video [video_website]` convert download_file (-f bestvideo+bestaudio) to mp4.  If ffmpeg get an error, could try `video_c`.
* `video_c [video_website]` convert download_file (-f bestvideo+m4a) to mp4. 
