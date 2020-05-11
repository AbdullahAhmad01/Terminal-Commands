1 : flmod:
      The program is used for two main purposes:
      1- Creating files of given mode
      2- Creating script files
  
      Examples
      ========
            I- flmod 644 details.txt
               [ equivilant to 'touch details.txt ; chmod 644 details.txt' ]
      
           II- flmod -o 644 details.txt
               [ same as first example but delete file if exists ]
      
          III- flmod -s myscript
               [ create 'myscript' file in current working directory, write following content in 'myscript' and finally run it]
               ______________________________________________________________
               | 1 | #!/bin/bash                                             |
               | 2 |                                                         |
               | 3 | # myscript : describe your program in one line          |
               | 4 |                                                         |
               | 5 | echo "Script file is ready"                             |
               |_6_|_________________________________________________________|
      
           IV- flmod -s -e myscript
              [ same as III but also open script using 'nano myscript' command ]

2 : grabber
      Grab files for copy/move
      
      Syntax
      ======
            grabber cp|mv FROM TO SEARCH_STRING
      
      Example
      =======
      following command will copy all '.jpg' files from /dev/sdb1 to Pictures of user directory
            grabber cp /dev/sdb1 /home/user/Pictures .jpg
