```
mkvinfo something.2019.S01E01.mkv | grep -A5 "Track type: subtitles" | grep -e Language -e Name
```
gives
```
|  + Language: cze
|  + Name: Czech
|  + Language: dan
|  + Name: Danish
|  + Language: ger
|  + Name: German
|  + Language: gre
|  + Name: Greek
|  + Name: English
|  + Language: spa
|  + Name: European Spanish
|  + Language: spa
|  + Name: Spanish
|  + Language: fin
|  + Name: Finnish
|  + Language: fre
|  + Name: French
|  + Language: ind
|  + Name: Indonesian
|  + Language: ita
|  + Name: Italian
|  + Language: nor
|  + Name: Norwegian
|  + Language: dut
|  + Name: Flemish [Original] (Forced)
|  + Language: dut
|  + Name: Dutch
|  + Language: pol
|  + Name: Polish
|  + Language: por
|  + Name: Brazilian Portuguese
|  + Language: por
|  + Name: Portuguese
|  + Language: rus
|  + Name: Russian
|  + Language: swe
|  + Name: Swedish
|  + Language: tur
|  + Name: Turkish
|  + Language: dut
|  + Name: Flemish
```
