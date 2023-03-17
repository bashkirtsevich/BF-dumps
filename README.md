# 🐝 Betaflight cli dumps
Local betaflight dumps with version history.

## Partial

### 📺 Analog
* [OSD config](analog-osd.txt)
* [VTX table](vtx-table.txt)

## Dumps list
* Mobula7
* Nazgul5 v2
* Pavo25
* PinkyCrux
* Thinking P16
* UZ-65
* Alpha A85 HD
* Baby Nazgul
* Crux3
* Foxwhoop 25
* Mobeetle6
* Mobula6
* HexNano

## Git export
```
find /path/to/dumps -type f -iname '*stock*.txt' -exec bash -c 'fname="{}"; dirname="$(basename "$(dirname "$fname")")"; basename="$(basename "$fname")"; mkdir -p $(pwd)/"$dirname"; cp "$fname" $(pwd)/"$dirname"/"$basename"; git add *; git commit -m "$basename";' \;
find /path/to/dumps -type f -iname '*cli*.txt' -exec bash -c 'fname="{}"; dirname="$(basename "$(dirname "$fname")")"; basename="$(basename "$fname")"; mkdir -p $(pwd)/"$dirname"; cp "$fname" $(pwd)/"$dirname"/dump.txt; git add *; git commit -m "$basename";' \;
```

