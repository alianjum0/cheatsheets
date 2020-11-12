#-# String manipulation

Command                                    Description
-------                                    -----------
${varname:-word}                           If varname exists and isn't null, return its value; otherwise return word
${varname:=word}                           If varname exists and isn't null, return its value; otherwise set it word and then return its value
${varname:?message}                        If varname exists and isn't null, return its value; otherwise print varname, followed by message and abort the current command or script
${varname:+word}                           If varname exists and isn't null, return word; otherwise return null
${varname:offset:length}                   Performs substring expansion. It returns the substring of $varname starting at offset and up to length characters

${variable#pattern}                        If the pattern matches the beginning of the variable's value, delete the shortest part that matches and return the rest
${variable##pattern}                       If the pattern matches the beginning of the variable's value, delete the longest part that matches and return the rest
${variable%pattern}                        If the pattern matches the end of the variable's value, delete the shortest part that matches and return the rest
${variable%%pattern}                       If the pattern matches the end of the variable's value, delete the longest part that matches and return the rest
${variable/pattern/string}                 The longest match to pattern in variable is replaced by string. Only the first match is replaced
${variable//pattern/string}                The longest match to pattern in variable is replaced by string. All matches are replaced

${#varname}                                Return the length of the value of the variable as a character string

*(patternlist)                             Match zero or more occurences of the given patterns
+(patternlist)                             Match one or more occurences of the given patterns
?(patternlist)                             Match zero or one occurence of the given patterns
@(patternlist)                             Match exactly one of the given patterns
!(patternlist)                             Match anything except one of the given patterns
[reference](https://github.com/vrachieru/cheatsheet)
