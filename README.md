# Steganography Notes And Tools

| Table of contents |
|     :---:      |
| [Image Steganography](https://github.com/ahmed-kamal-el-maghraby/Steganography/blob/main/README.md#image-steganography)     | 
| [Files Steganography](https://github.com/ahmed-kamal-el-maghraby/Steganography/blob/main/README.md#files-steganography)       |
| [Audio Steganography](https://github.com/ahmed-kamal-el-maghraby/Steganography/blob/main/README.md#audio-steganography)       |


## Image Steganography
Online Tools :
+ [Exiftool](https://exif.tools/)
+ [Pic2Map Photo](https://www.pic2map.com)
+ [GPS Coordinates](https://www.gps-coordinates.net)<br>

Command Line Tools :
> exiftool <br>
```
$ exiftool image.jpg
```
> Steghide <br>
```
$ steghide 
# To Embed file
$ steghide embed -cf image.jpg -ef secret.txt
# To Extract file
$ steghide extract -sf image.jpg
```
> Stegcracker <br>
```
$ stegcracker image.jpg /wordLits
```

## Files Steganography

>  To embedd test in file.txt  <br>
```
$ echo test.txt >> file.txt
```
> Binwalk tool
+ Check if there embedded file
```
$ binwalk file
```
+ To extract file from any file
```
$ binwalk --run-as=root -e file --dd=".*"
```

> Foremost tool

+ To Extract files
```
$ foremost file.txt
$ cd output	
```

## Audio Steganography
+ Audacity
  - Linux && windows
+ Sonic Visualizer	
  - Linux && windows
+ Deep Sound	
  - Add secret file in Audio and if you want password
