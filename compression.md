# **Types of zip files**

## Compression

There are 3 main types of zip files
- gzip
- bzip2
- xz

These files, zipped end in
- .gz
- .bz2
- .xz


#Example
To compress all '.mp4' files in current directory using gzip
```
gzip *.mp4
```

To compress all files in the 'videos' directory using gzip
```
gzip -r videos/
```


## Decompression

Decompress a compressed file using bzip2 
```
bzip2 -d background.png,bz2
```



## Archiving files

Archiving consolidates multiple files together into one file for easier storage and portability. Linux Bash has two commands for archiving and extracting files: zip and tar.

### zip & tar example
- zip
- zip <archive_name.zip> <file1> <file2>
- Extract unzip <archive_name.zip>

- tar
- tar -cf <archive_name>.tar <files or directory>
- extract tar -xf <archive_name.tar>

In linux environments, tar is preferred as a file extension because a tarball can retain important metadata like file permissions

Archiving the directory `riddles` using `zip`
```
zip riddles.zip -r riddles/
```

Archiving files using `tar`
```
tar -cf languages.tar english.txt french.txt
```


## Compressing Archive Files

The 'zip' bashcommand automatically compresses archives files while 'tar' can be combined with compression utilities like 'gzip', 'bzip2' and 'xz'.
There are specific options for tar that must be used to match compression command

### List of 'tar' options

-c :Creates an archive
-x : Extracts an archive
-f : Creates an archive with given filename
-z : Compresses using gzip. Resulting file extension .tar.gz
-j : Compresses using bzip2. Resulting file extension .tar.bz2
-J : Compresses using xz. Resulting file extension .tar.xz

### example
Archiving a media directory with 'tar' using 'xz' expression
```
tar -cJf media.tar.xz media/
```




## Linux Networking utilities

These are 3 basic commands to manage and communicate with networks

ping <target domain or IP>: Checks connectivity between 2 devices on the same network by sending packets

host <domain or IP>: Performs DNS resolution, which converts domains to IP addresses or vice versa

ifcongif: Shows network interface information 




## Downloading a File in Linux

To access or download a file from the internet, there are 2 main commands 'curl' and 'wget'. These commands establish a connection with the server and download either HTML of a webpage or file stored at the URL to the current working directory

curl -O <URL>
wget <URL>