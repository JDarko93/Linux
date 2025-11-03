#### **Types of zip files**

### Compression

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



### Archiving files

Archiving consolidates multiple files together into one file for easier storage and portability. Linux Bash has two commands for archiving and extracting files: zip and tar.

# zip & tar example
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