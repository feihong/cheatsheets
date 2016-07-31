Copy the input video from 14:43 to 16:55 and output it to a file called cut.mp4

```
ffmpeg -i movie.mp4 -ss 00:14:43 -to 16:55 -acodec copy -vcodec copy -async 1 cut.mp4
```

Extract audio from MP4 video into an M4A audio file

```
ffmpeg -i movie.mp4 -vn -acodec copy audio.m4a
```

Extract image from the first frame of 00:19 of mp4 file

```
ffmpeg -i movie.mp4 -ss 19 -frames:v 1 image.jpg
```

Add metadata to an m4a file

```
ffmpeg -i audio.m4a -metadata title="Bang Bang" -metadata artist="程思佳" -c copy audio2.m4a
```

Add cover artwork to an m4a file (cannot do this with ffmpeg)

```
AtomicParsley audio2.m4a --artwork image.jpg --overWrite
```
