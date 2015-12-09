# ffmpeg
Settings to run ffmpeg for mp4, ogv, and webm

fmpeg -i nameOfSource.mov  -vf  scale=640:360 -c:v libx264 -b:v 400K nameOfSource_400kbps.mp4
ffmpeg -i nameOfSource.mov  -vf  scale=640:360  -c:v libvpx -b:v 400K nameOfSource_400kbps.webm
ffmpeg -i nameOfSource.mov  -vf  scale=640:360  -c:v libtheora -c:a libvorbis -b:v 400K nameOfSource_400kbps.ogv
