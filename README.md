# BluRaytoMKV
BluRay to MKV Automation

* Rip BluRay using MakeMKV, https://www.makemkv.com/
* MKVToolNix needs to be installed, https://mkvtoolnix.download/downloads.html

# Setup
* Source -        Contains the Source MKV
* Transcoded -    Contains x264 transcoded video
* Converted -    Contains the Source MKV after a Merge
* Converted/Transcoded -    Contains x264 transcoded video after a Merge
* Merged -        Contains mkvmerged subtitle, Transcoded Video and Audio

# Variables to change
* MAINPATH = '/share/MakeMKV/'
* USER_PERMISSION = 'youruser'
* GROUP_PERMISSION = 'yourgroup'

Script will look for that largest share out of DVD and BluRay Dictionary to move the Merged File into.
Modify the share, path and media of STORAGE Dictionary, the script looks for the share and path,  if the Merged MKV has DVD in the filename, it will move the merged file into the DVD path.
The same goes for BluRay names.

* STORAGE  = [
*        {'freeSpace' : None, 'share' : '/share/3000gb-1', 'path' : '/Movies/', 'media': 'BluRay'},
*        {'freeSpace' : None, 'share' : '/share/3000gb-2', 'path' : '/Movies/1080P/', 'media': 'BluRay'},
*        {'freeSpace' : None, 'share' : '/share/4000gb-2', 'path' : '/Movies/', 'media': 'BluRay'},
*        {'freeSpace' : None, 'share' : '/share/4000gb-3', 'path' : '/Movies/', 'media': 'BluRay'},
*        {'freeSpace' : None, 'share' : '/share/4000gb-4', 'path' : '/Movies/', 'media': 'BluRay'},
*        {'freeSpace' : None, 'share' : '/share/4000gb-4', 'path' : '/MoviesDVD/', 'media': 'DVD'}
*        ]

