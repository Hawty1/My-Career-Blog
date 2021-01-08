## Wednesday 09.12.2020

### Today we are learning Terminal commands.

Terminal is the Linux command shell. We can run commands to perform several effective tasks.

| Command | Parameter                                                                        |        Full Name       |                                                   Usage                                                  |                             Example                             |
|---------|----------------------------------------------------------------------------------|:----------------------:|:--------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------:|
| pwd     |                                                                                  | Print Working Document | shows our current location.                                                                              | pwd                                                             |
| cd      | ../directory <br> ~                                                              |    Change Directory    | Change our current location to the one <br>   in the parameters.                                         |                   cd targetDirectory <br> cd ~                  |
| ls      | ./targetDirectory                                                                |       List Files       | Lists all the files in our <br> targeted directiory. <br> Without a parameter it reads the file          |                        ls targetDiretory                        |
| ll      | ./targetDirectory                                                                |        Long List       | lists a detailed list which files.                                                                       |                        ll targetDirectory                       |
| less    | targetFile                                                                       |          less          | Displays the contents of a file.                                                                         |                          less fileName                          |
| nano    | targetFile                                                                       |          nano          | Small text editor. <br> Without an existing file name as <br> parameter, it will create it as a new one. |               nano fileName <br> nano newFileName               |
| touch   | newFileName                                                                      |          touch         | create a new file                                                                                        | touch newFileName                                               |
| echo    | some text >>fileName <br> some text >>newFileName                                |          echo          | write something into an existing file. <br>  If the file does not, it will create one.                   | echo some text >>fileName <br> echo anotherText >>newFileName |
| cp      | fileName newfileName <br> fileName directory/ <br> -r directory targetDirectory/ |          copy          | we can copy an file                                                                                      | cp file.txt copiedFile.txt <br> cp file.txt targetDirectory/    |
| mv      | fileName newFileName <br> fileName targetDirectory/                              |          move          | can rename files <br>  can move files to another directions                                              | mv blue.txt blue.html <br> mv blue.html ../homepage/            |
| rm      | fileName <br> -r directoryName                                                   |         remove         | the "DANGEROUS" one <br> removes things _"FOREVER"_                                                      | rm fileName <br> rm -r directoryName                            |
#### Command "Flags"
those flag can be added to specify or comands.
| Flag | Usage                               | Example             |
|------|-------------------------------------|---------------------|
| -r   | target whole directory              | rm -r directoryName |
| -v   | check version of the app            | npm -v              |
| -f   | used to force actions like removing | rm -f directoryName |






#### Linux Librarys
there are also some librarys related to linux packages  from where we can install or update packages and apps.  We can just do it from the Terminal without searching on any extra platforms.  
The librarys musst be installed before.

| Command  | Parameter                                      | Full Name                    | Usage                                     | Example                                     |
|----------|------------------------------------------------|------------------------------|-------------------------------------------|---------------------------------------------|
| apt      | -cache search packageName <br> -cache search . | https://packages.ubuntu.com/ | Library for apps that run on Ubuntu       | apt-cache search . apt-cache search AppName |
| npm      | install packageName                            |     node package manager     | Library for node packages we will create  | install react                               |
| sudo     | apt install packageName apt update             |         super user DO        | need for installing or updating a package | sudo apt update                             |


