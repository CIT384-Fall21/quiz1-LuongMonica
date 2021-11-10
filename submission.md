# Quiz #1 : Assessment and Planning 

### Date: November 10, 2021
### In Class/Lab Quiz:
### Due:
* Morning Class:  11:45
* Afternoon Class: 5:45


---
## Name: Monica Luong                                 <!-- answer -->


1. A URL is comprised of a number of components.  Consider the following URL:

  ``one://two:three@four.five.size:seven/eight/nine/ten?eleven=twelve&thirteen=fourteen#fifteen``

  * Provide both the name and value of each component.
    1. scheme: "one"                                    <!-- answer -->
    1. user: "two"                                      <!-- answer -->
    1. password: "three"                                <!-- answer -->
    1. domain: "four.five.size"                         <!-- answer -->
    1. port: "seven"                                    <!-- answer -->
    1. file-path: "/eight/nine/ten"                     <!-- answer -->
    1. query-string: "eleven=twelve&thirteen=fourteen"  <!-- answer -->
    1. URI: "/eight/nine/ten?eleven=twelve&thirteen=fourteen" <!-- answer -->
    1. fragment: "fifteen"                              <!-- answer -->
    <!-- Add more lines as needed -->

1. In the following code block, provide the git instructions necessary to add a new file to the remote repository: git@github.com:org/project.git (You should presume that you don't have a copy of this repository on your local computer.)
   ```
      git clone git@github.com:org/project.git                  <!-- answer -->
      git add file                                              <!-- answer -->
      git commit -m "message"                                   <!-- answer -->
      git push                                                  <!-- answer -->
   ```
   <!-- You many add any number of lines in the above code block that you need. -->

1. Provide the Apache Directive used to perform the requested action
   1. Position the location of root location of the website at:  /var/www/html
     * DocumentRoot /var/www/html                                                 <!-- answer -->
   1. To disable the user "steve" from having a web presence on your server.
     * Disabled "steve" -none                                                 <!-- answer -->
   1. To create an alias between the URI: /marketing and the file: /user/marketing/www
     * Alias /marketing /user/marketing/www                                        <!-- answer -->
   1. To define the location of the error log to be: /var/log/apps/apache/error.log
     * ErrorLog /var/log/apps/apache/error.log                                     <!-- answer -->


1. What is the command used to create the user "steve" within your apache container?
    * useradd -ms /bin/bash steve                                                 <!-- answer -->


1. What does the "AllowOverride" Directive do?
    * lets users override the settings/configurations on that particular directory. For example, users can use an .htaccess file to make changes to that particular directory. AllowOverride also has different options. I think All, None and something else I can't remember.            <!-- answer -->


1. Given the following command, provide the corresponding HTTP Request Header:
    * curl  https://www.csun.edu/~steve/roster/input/value/input/value
    ```
      GET /~steve/roster/input/value/input/value HTTP/1.1                     <!-- answer -->
      ServerName: www.csun.edu                                                <!-- answer -->
    ```                                                      
    <!-- You many add any number of lines in the above code block that you need. -->

1. The CGI standard defines a number of environment variables that are provided to a CGI program.  Identify and explain the purpose of 6 of these environment variables.
   1. QUERY_STRING:  the part of URL after ? character.             <!-- answer -->
   1. REQUEST_FILENAME: the name of the file requested by the user     <!-- answer -->
   1. SERVER_NAME: the name of the (web) server the user is requesting something from      <!-- answer -->
   1. SERVER_PORT: the port (e.g: 80) the server is serving requests on                     <!-- answer -->
   1. REMOTE_PORT: the user's port (e.g: 2049) that they are communicating through         <!-- answer -->
   1. REMOTE_IP: the user's IP addr (e.g: 72.146.12.151) that they are coming from                 <!-- answer -->


 1. Consider the following URL and regular expression used to process this string:
    * URL:   ``http://www.fake.org/marketing/john.smith/code=10325/app/input``
    * regexp: ``"^marketing/([a-z]*.[a-z]*)/(code=[0-9]{4,6})/(.*)$"``

    Define the value of each of the following back references
    1. $1: john.smith                                                <!-- answer -->
    1. $2: code=10325                                                <!-- answer -->
    1. $3: app/input                                                 <!-- answer -->
    1. $4: no value, no more groups ()                               <!-- answer -->

1. There are a number of different types of files.  Each of these file types can be identified by a single character in the output of the command ``ls -l``.  What are these types of files:
   1. -: a regular file
   1. p: process, i know this is wrong, i can't remember what it is right now       <!-- answer -->
   1. l: symbolic link                                            <!-- answer -->
   1. d: directory                                                <!-- answer -->
   1. b: block                                                    <!-- answer -->
   1. c: character                                                <!-- answer -->
   1. s: socket                                                   <!-- answer -->

1. Describe each of the following:
  - process: An entity that does something. All processes have the default 3 file handlers: stdin (0), stdout (1), stderr(2). They each have their own environment where env vars are stored. Processes can be linked together with pipes in order to change where the input/output of one command can come from/go to.                                                     <!-- answer -->
  - environment: The enclosed space/area that commands are executed in. the environment has certain env vars inluding HOME or USER. You can see them by running env. a new environment is created for a command when you: create a subshell () or use a pipe (|). not all variables are passed in to the child env. to have a var be accessible globally, use 'export var' or 'declare -x var'. and put it in one of the profiles like ~/.profile.                                                 <!-- answer -->
  - stdin: the input file, where info is coming in from, file handler is 0, and stdin is usually the keyboard                                                      <!-- answer -->
  - $?: the return value of the command that previously ran. in general: if == 0, then executed successfully, if == 1, some sort of error occurred                                                          <!-- answer -->
 
