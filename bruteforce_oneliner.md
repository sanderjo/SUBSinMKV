Without any knowledge of or tool for MKV, and just mainstream linux tools ... here's a bruteforce method to see the subtitles:

```
$ strings something.2019.S01E01.mkv  | head -200 | grep -A2 TEXT | grep -v TEXT | grep -v Sn | sort -u
```
gives output
```
--
Brazilian Portuguese
Czech
Danish
Dutch
English
European Spanish
Finnish
Flemish
Flemish [Original] (Forced)
French
German
Greek
Indonesian
Italian
Norwegian
Polish
Portuguese
Russian
Spanish
Swedish
Turkish
```
