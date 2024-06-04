
[Back](http://marochang.github.io/)

## Table of Contents

#Links to the documentation
- [1. How to run](https://marochang.github.io/bash/1.How_to_run)
- [2. Basic script](https://marochang.github.io/bash/2.Basic_script)
- [3. Bash script ideas](https://marochang.github.io/bash/3.Bash_script_ideas)

Bash is a command processor. It's widely used Unix shell and command language that is the default shell on many Linux distributions and macOs.

### Key features
1. Command execution
2. Scripting / Automation of tasks
3. Environment Customization
4. Pipelines & Redirection: Bash supports piping (`|`) to pass the output of one command as input to another, and redirection (`>`, `>>`, `<`) to manage input and output streams.

### Basic Commands

#### Navigation
```sh
cd /path/to/directory  #change directory
cd ..                  #back 
cd ~                   #back to root

pwd                    #print working directory

ls                     #list directory content
ls -a
ls -l
```
#### File Management
```sh 
mkdir directory       #make new directory
touch fileName        #create an empty file
rm fileName           #remove file
rmdir directort       #remove directory
cp source dest        #Copy a file or directory
mv source dest        #Move or rename a file or directory
```

#### Viewing files
```sh
cat fileName         #Concatenate & display file content
head fileName        #Display the 1st line
tail fileName        #Display the last line
```

#### Search files
```sh
#Searching for file with filter
find /path -name "filename"
find . -name "*.txt" -print

#Find files by name
locate fileName

#GREP (Globally serach a Regular Expression and print)
#search for patterns within file
grep theText thefile.txt
```

#### Useful Commands

```sh
echo "Hello world!"  #Display text
history              #command history
date                 #Friday, 31 May 2024 3:12:25PM
location             #current file path
whoami               #Current logged-in user
man ls               #manual for a command  
exit                 #exit the terminal or script
```

#### Compression and Archiving
```sh
tar -cvf achive_name.tar directory_name
tar -xvf archive_name.tar

gzip file_name
gunzip file_name.gz

zip archive_name.zip file_name
unzip archive_name.zip
```
#### Network
```sh
ping www.example.com
ifconfig

ip addr show           
ip link show

wget http://example.com/file
curl http://example.com
```
### Arguments
App 
Sub Command = action
Flags/Option = modify behavior. Extension of a command
Arguments = Noun

```sh
cp -f [args 1] [args 2]

remove --force [file]
#short form
remove -f [file]
```

![[Pasted image 20240601010410.png]]