# Perform actions on CLI
####Create/Read/Update/Delete/Move files and folders from command line
  *create folder
    mkdir dir1
  *create file
    touch file1.txt
  *read file
    cat file1.txt
  *update file
    nano file1.txt
  *delete file
    rm file1.txt
  *move file 
    mv file1.txt dir1
    
####Check disk status
  *df -h
  
####Check the status of processes, able to extract process ids ( hint: use pipe operator to combine ps, xargs and awk)
Getting the most senior parent process
   *ps
   *ps id
   **extract process id**
     *pidof [processname]
     *ps|grep regex

####Change file permissions. Able to explain and manipulate the numerical file permissions. (chmod and chown)
    *chmod WHO[+,-,=]PERMISSIONS FILENAME
      *u	user
       g	group
       o	others
       a	all
    *chmod u=rwx,g=rx,o=
      *chmod 750 ~/example.txt
      000	0	—
      001	1	–x
      010	2	-w-
      011	3	-wx
      100	4	r–
      101	5	r-
      110	6	rw-
      111	7	rwx
     *chown [options] new_owner[:new_group] file(s)
       *How to Change Owner of the File in Linux
         *chown owner_name file_name
           *chown master file1.txt
        *How to Change the Group of the File in Linux
           *chown :group1 file1.txt
        *How to Change Owner and Group of the File in Linux
            *chown master:group1 file1.txt
        *How To Change Group Ownership
            *chown :group1 file1.txt
          
####Able to extract last x lines from files, get word count for a particular word, find a particular word. (basics of sed or awk would do)
Basics of sed and awk.
   *extract last x lines from files
     *tail -n <number of lines> <filepath>
   *get word count for a particular word
     *grep -o Harry drill2.txt | wc -l
   *Basics of sed and awk
     [refer..](https://www.linode.com/docs/guides/differences-between-grep-sed-awk/)
    
  
####learn what is the difference between absolute and relative paths
    *r[refer](https://www.geeksforgeeks.org/absolute-relative-pathnames-unix/)
    
####Practice using absolute and relative paths
     *$pwd
        */home/kt
      *$cd abc                   
      *$pwd
        */home/kt/abc 
####Learn how to use the find command
      *find /path/to/search -options criteria
        *find ~ -name "example.txt"
        *find ./GFG -name *.txt 
        
####Learn ls with the 5 most commonly used flags used such as: -- View hidden files -- Sort by time -- Reverse sort -- Human readable file sizes -- Combining flags to get hidden files, sorted by time in reverse with human readable file sizes.
      *-- View hidden files -- 
        *ls -a
      *-- Sort by time --
        *ls -t
      *-- Reverse sort --
        *ls -r
      *-- Human readable file sizes --
        *ls -lh
      *-- Combining flags to get hidden files, sorted by time in reverse with human readable file sizes --
        *ls -a -lh

####Find out what are terminal control codes such as Ctrl + D, Ctrl + C, Ctrl + Z etc and use them
    *CTRL + D it'll tell the bash session to end
    *CTRL + C and it'll interrupt what it's doing and stop.
    *CTRL + Z pause the compression process and return to the terminal prompt

####Find out the difference between Ctrl + C and Ctrl + Z
    *Control+C aborts the application almost immediately while Control+Z shunts it into the background, suspended.
    
####Find out how to use Ctrl + R to reverse search
    1.  Press `Ctrl+R`. This will start the reverse-i search.
    2.  Type the string you want to search for. As you type, the terminal will show you the most recent command that matches your search string.
    3.  If the command shown is not the one you want, press `Ctrl+R` again to move to the next matching command.
    4.  Once you've found the command you want, press `Enter` to execute it.
    
####Find out how to use tab autocompletion
  *pressing the [TAB] and the active command line options will fill in. If more than one option is available, you can hit [TAB] twice to display all possible choices and continue typing until there is only one matching choice left
  
####Find out how to use the arrow keys to navigate history
  *Linux maintains a history of commands you have entered. Using the up and down arrow keys, you can recall previously-entered commands to the command line, edit them and re-issue them.
