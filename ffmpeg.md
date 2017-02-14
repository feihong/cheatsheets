# FFmpeg Cheatsheet

## Concatenate two videos together

```
# Generate text file containing .mp4 files to concatenate:
for f in ./*.mp4; do echo "file '$f'" >> mp4list.txt; done
# Concatenate the files to produce output.mp4
ffmpeg -f concat -safe 0 -i mp4list.txt -c copy output.mp4
```

Source: [Concatenation of files with same codecs](https://trac.ffmpeg.org/wiki/Concatenate#samecodec)

## Copy the input video from 14:43 to 16:55 and output it to a file called cut.mp4

`ffmpeg -i movie.mp4 -ss 00:14:43 -to 16:55 -acodec copy -vcodec copy -async 1 cut.mp4`

## Extract audio from MP4 video into an M4A audio file

`ffmpeg -i movie.mp4 -vn -acodec copy audio.m4a`

## Extract image from the first frame of 00:19 of mp4 file

`ffmpeg -i movie.mp4 -ss 19 -frames:v 1 image.jpg`

## Add metadata to an m4a file

`ffmpeg -i audio.m4a -metadata title="Bang Bang" -metadata artist="程思佳" -c copy audio2.m4a`

Note that AtomicParsley is still better for this kind of thing.

## Trim the given m4a file from 0:10 to 3:40

`ffmpeg -i audio2.m4a -ss 10 -to 3:40 -acodec copy cut.m4a`

Note that this will not preserve artwork; even using -c copy will not copy it over.

## Add cover artwork to an m4a file

`AtomicParsley audio2.m4a --artwork image.jpg --overWrite`

Note that there is no way to do this with ffmpeg.

## Extract cover artwork from m4a file

`ffmpeg -i audio2.m4a cover.jpg`
