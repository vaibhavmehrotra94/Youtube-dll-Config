# Youtube dll Config


##command to use
*****************

###Steps To follow-

1 install python (latest version).

2 download youtube-dl (Latest)
	download link - (https://rg3.github.io/youtube-dl/download.html)
	here download "windows exe".

3 copy the youtube-dl file to floder where u want to download the video/s.

4 "shift+RightClick" on the folder.

5 Select "open command Window here".

6 Paste the above provided command line
**********************************************************************



##(For Single Vid)Eg-

youtube-dl "Paste playlist link here within double quotes"
**********************************************************



##(For Playlist with index)Eg-

###1st Way(To download the full playlist with proper name and order)

youtube-dl -icAt "Paste playlist link here within double quotes"
****************************************************************



###2nd way(To download with name and index but starting from 00000)

youtube-dl -ic -o %(autonumber)s-%(title)s.%(ext)s "Paste playlist link here within double quotes"
**************************************************************************************************



###3rd way(To download whole playist with name and index)
													 
youtube-dl -ic -o %(playlist_index)s-%(title)s.%(ext)s "Paste playlist link here within double quotes"
******************************************************************************************************


###4th way(to start from mid to the end of playlist)

youtube-dl -ic -o %(playlist_index)s-%(title)s.%(ext)s --playlist-start <Video Number Here without brackets> "Paste playlist link here within double quotes"
***********************************************************************************************************




##link for option explanation

http://paste.ubuntu.com/6967883/
********************************