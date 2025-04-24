Commands for SMB enumeration:

  --Enumerate shared resources--

      ```bash nxc smb 10.10.10.10. -u "user" -p "password" --shares ```



  --List all readable files--
  
    
 `spider_plus` is a module for recursively listing files and saving JSON share-file metadata to the `OUTPUT_FOLDER`. To see all available modules, use `--list-modules`.

      ```bash nxc smb --list-modules```.        

      ```bash nxc smb 10.10.10.10 -u 'user' -p 'pass' -M spider_plus ```


  --Dumping All Files--

`-o` is the short form of the `MODULE_OPTION`. To list all available options for a module, use the `--options` flag.


      ```bash nxc smb 10.10.10.10 -u 'user' -p 'pass' -M spider_plus -o DOWNLOAD_FLAG=True ```
