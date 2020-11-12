#-#
#-# Input/Output Redirection
#-#

Command                                    Description
-------                                    -----------
cmd1|cmd2                                  Pipe; takes standard output of cmd1 as standard input to cmd2
> file                                     Directs standard output to file
< file                                     Takes standard input from file
>> file                                    Directs standard output to file; append to file if it already exists
>|file                                     Forces standard output to file even if noclobber is set
n>|file                                    Forces output to file from file descriptor n even if noclobber is set
<> file                                    Uses file as both standard input and standard output
n<>file                                    Uses file as both input and output for file descriptor n
<<label                                    Here-document
n>file                                     Directs file descriptor n to file
n<file                                     Takes file descriptor n from file
n>>file                                    Directs file description n to file; append to file if it already exists
n>&                                        Duplicates standard output to file descriptor n
n<&                                        Duplicates standard input from file descriptor n
n>&m                                       File descriptor n is made to be a copy of the output file descriptor
n<&m                                       File descriptor n is made to be a copy of the input file descriptor
&>file                                     Directs standard output and standard error to file
<&-                                        Closes the standard input
>&-                                        Closes the standard output
n>&-                                       Closes the ouput from file descriptor n
n<&-                                       Closes the input from file descripor n
[reference](https://github.com/vrachieru/cheatsheet)
