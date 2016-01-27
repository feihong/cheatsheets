Copy the input video from 14:43 to 16:55 and output it to a file called cut.mp4

```
ffmpeg -i movie.mp4 -ss 00:14:43 -to 16:55  -acodec copy -vcodec copy -async 1 cut.mp4
```
