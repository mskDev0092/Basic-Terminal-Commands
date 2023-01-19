# Basic Terminal Commands

# grep command

> The grep command is a powerful command line tool used for searching for patterns in text files or streams. It can be used to search for specific strings or regular expressions, and can be used to filter out unwanted lines from output. 

> If you want to practice the grep command, you can use the command line to do so. You can search through a file for a specific string pattern, or search multiple files for a string pattern. For example, to search for the word "example" in a file named "example.txt", you would use the following command:

grep example example.txt

> If you wanted to search multiple files, you could use the following command:

grep example *.txt

> You can also use regular expressions to search for patterns of characters, or use additional flags to modify the behavior of the grep command. 

# awk command

> The awk command is a powerful command line tool used for processing text files and manipulating the data within them. It can be used to search for specific patterns in a file, perform calculations on data, and modify the format of the output

> To practice using the awk command, you can use the command line to do so. The awk command is used to process text files and manipulate the data within them. To use the awk command you will need to specify a pattern, which can be a regular expression, and then specify an action to take with the data that matches the pattern.

> For example, to search for the word "example" in a file named "example.txt" and print out the line containing the word, you would use the following command:

awk '/example/ {print}' example.txt

> If you wanted to search multiple files, you could use the following command:

awk '/example/ {print}' *.txt

> You can also use awk to perform calculations on data, such as summing up a column of numbers. To do this, you would need to specify the field separator, which is usually a comma or space, and then specify the action to take with the data. For example, to sum up the values in the third column of a file named "data.txt", you would use the following command:

`awk -F, '{sum += $3} END

# sed command

> The sed command is a powerful command line tool used for processing text files and manipulating the data within them. It can be used to search for specific patterns in a file, perform calculations on data, and modify the format of the output.

> To practice using the sed command, you can use the command line to do so. The sed command is used to process text files and manipulate the data within them. To use the sed command you will need to specify a pattern, which can be a regular expression, and then specify an action to take with the data that matches the pattern.

> For example, to search for the word "example" in a file named "example.txt" and replace it with the word "example2", you would use the following command:

sed 's/example/example2/g' example.txt

> You can also use sed to perform calculations on data, such as summing up a column of numbers. To do this, you would need to specify the field separator, which is usually a comma or space, and then specify the action to take with the data. For example, to sum up the values in the third column of a file named "data.txt", you would use the following command:

sed -e 's/[, ]/\n/g' data.txt | awk '{sum += $3} END {print sum}'

# curl command

> The curl command is a powerful command line utility used for transferring data over the web. It can be used to make requests to web servers and download data, as well as upload data to web servers.

> To practice using the curl command, you can use the command line to do so. To make a GET request to a URL, you would use the following command:

curl -X GET https://www.example.com/data.json

> You can also use additional flags to modify the behavior of the curl command. For example, you can use the -d flag to send data in the request body, or the -H flag to set HTTP headers. You can also use the -u flag to include authentication credentials in the request.

> To practice downloading data from a web server, you can use the -O flag to save the data to a file. For example, to download a file named "data.json" from the URL "https://www.example.com/data.json", you would use the following command:

curl -O https://www.example.com/data.json

> You can also use the -o flag to specify a different output file name. For example, to download the same file and save it as "data2.json", you would use the following command:

`curl -

# wget command

> The wget command is a powerful command line utility used for downloading files from the internet. It can be used to download webpages, images, and other types of files from a web server. 

> To practice using the wget command, you can use the command line to do so. To download a file named "data.json" from the URL "https://www.example.com/data.json", you would use the following command:

wget https://www.example.com/data.json

> You can also use additional flags to modify the behavior of the wget command. For example, you can use the -O flag to specify a different output file name, or the -c flag to resume an interrupted download. You can also use the -P flag to specify the directory where the file should be downloaded.

> To practice uploading data to a web server, you can use the --post-file flag to include data in the request body. For example, to upload a file named "data.json" to the URL "https://www.example.com/upload.php", you would use the following command:

wget --post-file data.json https://www.example.com/upload.php

> You can also use the -T flag to specify the timeout for the request.

# tail command

> The tail command is a UNIX utility used to view the end of a file or stream. By default, it will display the last 10 lines of a file, but it can be used to display any number of lines.

> To practice using the tail command, you can use the command line to do so. To view the last 5 lines of a file named "data.txt", you would use the following command:

tail -n 5 data.txt

> The tail command can also be used to monitor files as they are written to, by using the -f flag. This allows you to view the output of log files in real-time, or monitor files for changes. For example, to monitor a file named "data.txt" for changes, you would use the following command:

tail -f data.txt

> You can also use the -n flag to specify the number of lines to display, and the -s flag to specify the delay between updates. For example, to view the last 10 lines of a file named "data.txt" with a 1-second delay between updates, you would use the following command:

tail -n 10 -s 1 data.txt

# head command

> The head command is a UNIX utility used to view the beginning of a file or stream. By default, it will display the first 10 lines of a file, but it can be used to display any number of lines. 

> To practice using the head command, you can use the command line to do so. To view the first 5 lines of a file named "data.txt", you would use the following command:

head -n 5 data.txt

> You can also use additional flags to modify the behavior of the head command. For example, you can use the -q flag to suppress the output of headers, or the -n flag to specify the number of lines to display.

> You can also combine the head and tail commands to view a specific range of lines. For example, to view lines 5-10 of a file named "data.txt", you would use the following command:

head -n 10 data.txt | tail -n +5

> You can find more information about the head command and examples of its usage by searching online.

# less command

> The less command is a UNIX utility used to view the content of a file or stream. It can be used to view the entire content of a file, or to scroll through the file one page at a time.

> To practice using the less command, you can use the command line to do so. To view the contents of a file named "data.txt", you would use the following command:

less data.txt

> The less command can also be used to search for text within the file. For example, to search for the term "example" within the file, you would use the following command:

less data.txt /example

> You can also use additional flags to modify the behavior of the less command. For example, you can use the -e flag to exit the less command when the end of the file is reached, or the -N flag to display line numbers.

> You can find more information about the less command and examples of its usage by searching online.

# find command

> The find command is a UNIX utility used to search for files and directories in a given directory and its subdirectories. It can be used to search for files with certain characteristics, such as files of a certain size or age.

> To practice using the find command, you can use the command line to do so. To find all files in the current directory that are larger than 1GB, you would use the following command:

find . -type f -size +1G

> The find command can also be used to search for files with specific names, or with specific permissions. For example, to find all files in the current directory with the name "data.txt", you would use the following command:

find . -name data.txt

> You can also use additional flags to modify the behavior of the find command. For example, you can use the -mmin flag to search for files modified within a certain time range, or the -perm flag to search for files with a certain permissions mode.

> You can find more information about the find command and examples of its usage by searching online.

# ssh command

> The ssh command is a UNIX utility used to securely access a remote computer over an unsecured network. It is used to securely connect to a remote computer, execute commands on that computer, and transfer files between the two computers.

> To practice using the ssh command, you can use the command line to do so. To connect to a remote computer, you would use the following command:

ssh username@hostname

> Once connected, you can use the command line to execute commands on the remote computer, or to transfer files between the two computers. For example, to copy a file from the local computer to the remote computer, you would use the following command:

scp filename username@hostname:path/to/destination

> You can also use additional flags to modify the behavior of the ssh command. For example, you can use the -i flag to specify a private key file for authentication, or the -p flag to specify a port number to connect to.

> You can find more information about the ssh command and examples of its usage by searching online.

# kill command

> The kill command is a UNIX utility used to terminate a process by sending a signal to it. It can be used to terminate a process that is stuck or unresponsive, or to terminate a process that is using up too much system resources.

> To use the kill command, you need to know the process ID of the process you want to terminate. To find the process ID of a process, you can use the ps command.

> To practice using the kill command, you can use the command line to do so. To find the process ID of a process, you can use the ps command. For example, to list all processes running on the system, you would use the following command:

ps -A

> Once you have the process ID, you can use the kill command to terminate the process. For example, to terminate process with ID 1234, you would use the following command:

kill 1234

> You can also use additional flags to modify the behavior of the kill command. For example, you can use the -9 flag to send the SIGKILL signal, which will force the process to terminate immediately.

> You can find more information about the kill command and examples of its usage by searching online.

> To kill an application that is using multiple process IDs, you can use the killall command. This command will terminate all processes with the specified name. For example, to kill an application named "myapp", you would use the following command:

killall myapp

> Note that the name of the application may not always be the same as the name of the executable file. If you are not sure what the name of the application is, you can use the ps command to list all of the processes running on the system and find the name of the application you want to terminate.

# dig command

> The dig command is a UNIX utility used to query DNS name servers. It is used to query DNS servers for information about host addresses, mail exchanges, and other information related to domain names.

> To use the dig command, you need to specify the domain name you want to query and the type of query you want to perform.

> To practice using the dig command, you can use the command line to do so. To query the DNS server for the address of the host example.com, you would use the following command:

dig example.com A

> You can also use the -t flag to specify the type of query you want to perform, such as MX to query for mail exchanges or NS to query for name servers
