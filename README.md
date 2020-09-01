my shell snippets

# piando - 🎹

BASH script to generate a shuffled list of files in a given directory

4 options are available. 
```
-d, --directory: directory to search. default is working directory
-r, --recursive: recursively shuffle the given directory. default is off
-e, --extension: only shuffle files with the given extension. default is all files
-f, --folders: only shuffle folders
```

### examples
shuffle all files found recursively in memes directory
```
> piando -r -d ~/memes
```
shuffle all png files found recursively in memes directory
```
> piando -r -d ~/memes -e png
```
shuffle all folders found recursively in music directory. play them with `mpv`
```
> piando -r -d ~/music -f | mpv --playlist=- --loop-playlist
```
# moonphases - 🌚
script to generate the current moonphase

1 option is available
```
-s, --southern: are you in the southern hemisphere? default is no
```
### examples
```
> ./moonphases
🌘 Waning Crescent
> ./moonphases -s
🌒 Waning Crescent
```

# suntimes - 🌞
script to generate sunrise and sunset times

1 option is available
```
-l, --location: location code from weather.codes/search/ for current location. default is bay area
```
### examples
get sunrise and sunset for boston
```
> ./suntimes -l USMA0046
🌄 05:55  🌇 20:15
```
get sunrise and sunset for agra
```
> ./suntimes -l INXX0203
🌄 05:17  🌇 20:04
```

# center_string - 🧵
script to center a string by padding with whitespace to the left and right

### examples
center 'hi' between whitespace where total character count is 28
```
> ./center_string hi 28
             hi             
```
