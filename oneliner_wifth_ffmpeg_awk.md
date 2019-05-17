Combining ffmpeg with awk:

```
$ ffmpeg -i blabla.DVDRip.AC3.x264-MandR.mkv 2>&1 | awk -F"[()]"  '/Subtitle/ { printf $2 " " } END { print "" } '
```
gives
```
eng tur dan fin nor swe
```
So: the three-letter abbreviations for the subtitle languages.

Based on this brute force output:

```
    Stream #0:3(eng): Subtitle: dvd_subtitle, 720x576 (default)
    Stream #0:4(tur): Subtitle: subrip
    Stream #0:5(dan): Subtitle: dvd_subtitle, 720x576
    Stream #0:6(fin): Subtitle: dvd_subtitle, 720x576
    Stream #0:7(nor): Subtitle: dvd_subtitle, 720x576
    Stream #0:8(swe): Subtitle: dvd_subtitle, 720x576
```

