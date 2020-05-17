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
piando -r -d ~/memes
```
shuffle all png files found recursively in memes directory
```
piando -r -d ~/memes -e png
```
shuffle all folders found recursively in music directory. play them with `mpv`
```
piando -r -d ~/music -f > .playlist; mpv --playlist=.playlist --loop-playlist
```
# moonphases

# suntimes

# center_string
