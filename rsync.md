# rsync

```
rsync -aHxv --numeric-ids --progress ~/reference <dest_ip>:~/reference
```

Note that -A and -X options are not available for the system version of rsync on MacOS 10.12.

Source: https://gist.github.com/KartikTalwar/4393116
