Commands for SMB enumeration:

  --Enumerate shared resources--

      nxc smb 10.10.10.10. -u "user" -p "password" --shares



  --List all readable files--
  
    
 `spider_plus` is a module for recursively listing files and saving JSON share-file metadata to the `OUTPUT_FOLDER`. To see all available modules, use `--list-modules`.

      nxc smb --list-modules        

The output of this command will give us the path where the JSON file is saved.
      
      nxc smb 10.10.10.10 -u 'user' -p 'pass' -M spider_plus



  --Dumping All Files--

`-o` is the short form of the `MODULE_OPTION`. To list all available options for a module, use the `--options` flag.


    nxc smb 10.10.10.10 -u 'user' -p 'pass' -M spider_plus -o DOWNLOAD_FLAG=True

