# Youtube dll Config
These steps are only tested with windows. Not sure if this will work with any other OS.

## Initial Steps To follow -

1. Install python (latest version).

2. Download youtube-dl (Latest)
	[Download Page](https://rg3.github.io/youtube-dl/download.html)

	* Here download "windows.exe".

3. Copy the youtube-dl file to floder where u want to download the video/s.

4. "shift+RightClick" on the folder for options menu.

5. Select "open command Window here" in menu.

6. Paste & Run desired command in the cmd-promt after configuring them.
**********************************************************************


## COMMANDS

## Single Video
```
youtube-dl "Paste playlist link here within double quotes"
```



## Playlist

### 1. - To download the full playlist with proper name and order
```
youtube-dl -icAt "Paste playlist link here within double quotes"
```



### 2. - To download with name and index but starting from 00000
```
youtube-dl -ic -o %(autonumber)s-%(title)s.%(ext)s "Paste playlist link here within double quotes"
```



### 3. - To download whole playist with name and index
```													 
youtube-dl -ic -o %(playlist_index)s-%(title)s.%(ext)s "Paste playlist link here within double quotes"
```


### 4. - To start from mid to the end of playlist
```
youtube-dl -ic -o %(playlist_index)s-%(title)s.%(ext)s --playlist-start <Video Number Here without brackets> "Paste playlist link here within double quotes"
```




## Link for other option explanation

http://paste.ubuntu.com/6967883/
