# ffmpeg
Settings to run ffmpeg for mp4, ogv, and webm

ffmpeg -i nameOfSource.mov  -vf  scale=640:360 -c:v libx264 -b:v 310K nameOfSource_310kbps.mp4
ffmpeg -i nameOfSource.mov  -vf  scale=640:360  -c:v libvpx -b:v 350K nameOfSource_350kbps.webm
ffmpeg -i nameOfSource.mov  -vf  scale=640:360  -c:v libtheora -c:a libvorbis -b:v 330K nameOfSource_330kbps.ogv
