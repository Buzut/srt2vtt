# srt to vtt converter
A PHP **command line** script to convert subtitles from SubRip to WebVTT format.

This tool is based on [WebVTT-to-SRT](https://github.com/tunggnu/WebVTT-to-SRT). It just does the contrary.

## Usage
Just provide source and destination files path.
`php srt2vtt.php </some/path/original.srt> <other/path/result.vtt>`

Exemple:

```
php srt2vtt.php my-movie.srt my-movie.vtt
```

Don't hesitate to use bash `for` loops to convert many files in in a row.

```
for f in *.srt; do fn=`echo $f | sed 's/srt/vtt/'`; php srt2vtt.php "$f" "$fn"; done
```
