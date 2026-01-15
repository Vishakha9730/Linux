## Archiving and Compression-
- Archiving is the process of Bundling and Compression.
- Bundling is the process of combining multiple files and directories (same or different sizes) into one file/place.
- On the other hand, compression is the process of reducing the size of a file or directory.

# tar command-
 - tar is commonly used to bundle files and directories together into a single archive file, which can then be compressed if desired.
### tar <-options> <compress_fileName>.tar <files_to_be_compressed>
#### options-
- -c -> create an archive.
- -f -> file name. (Compulsory option)
- -v -> verbose or view.
- -t -> list the content from archive.
- -x -> execute the content from archive.
- -C -> copy content from an archive to another directory.

# Compression-
- Compression is a reduction in the number of bits needed to represent data.
- Compressing data can save storage capacity, speed up file transfer, and decrease costs for storage hardware and network bandwidth.

## GZIP: 
- GZIP is good option for compressing a lot of data as it is quick.
- Its memory usage is also low.
- GZIP compression can be used by using “-z” option in tar command or by using gzipcommand.
- GZIP compressed file can be extracted using gunzip.
## BZIP2:
- BZIP2 provide better compression ratio compared to GZIP but require more "CPU time" to accomplish it.
- “-j” option in tar or bzip2 command can be used for bzip2 compression.
- Bunzip2 is command to extract bzip2 compressed file.
## XZ:
- XZ provide impressive compression ration but in cost of very high CPU and Memory usage.
- Decompression speed is better but it also consumes a lot of memory.
- XZ compression can be done by “-J” option in tar or xz command.

| No. | Name   | Option | Extension      | Unzip Command |
|-----|--------|--------|----------------|---------------|
| 1   | gzip   | -z     | .tar.gz        | gunzip        |
| 2   | bzip2  | -j     | .tar.bz2       | bunzip2       |
| 3   | xz     | -J     | .tar.xz        | unxz          |


# ZIP Command -
- zip is a command used to compress one or more files/folders into a single .zip archive.
- unzip is a command used to extract files from a .zip archive.

      zip [options] archive_name.zip file1 file2 folder/

-r --> recursive - to zip directory

      unzip [options] archive_name.zip









