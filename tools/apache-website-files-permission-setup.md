<!-- TITLE: Apache Website Files Permission Setup -->
<!-- SUBTITLE: A quick summary of Apache Website Files Permission Setup -->

Website files served by Apache need to have appropriate permissions. The common practice is to set all directories to 755 and set all files to 644.

To change all the directories to 755 (`drwxr-xr-x`):


```batchfile
find <path_to_document_root> -type d -exec chmod 755 {} \;
```


To change all the files to 644 (`-rw-r--r--`):


```batchfile
find <path_to_document_root> -type f -exec chmod 644 {} \;
```


In the commands above, `chmod 644 {} \;` specifies the command that will be executed by `find` for each file. `{}` is replaced by the file path, and the semicolon denotes the end of the command (escaped, otherwise it would be interpreted by the shell instead of `find`).