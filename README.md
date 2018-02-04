# get_next_line

A programme which reads a text from a file descriptor, returning the next unread line.  A line is defined as a succession of characters ending in either a '\n' or '\0'.  Only read, malloc and functions from my libft were allowed to be used.  Use of lseek was not allowed for the project.  Global variables were forbidden.

# how it works

get_next_line takes 2 parameters: the file descriptor being read from, and the address of a pointer that will be used to store the read line.  The line will be stored without the '\n'.
get_next_line will return 1, 0, or -1 when a line has been read, when the reading has been completed, or when an error has occured respectively.
Calling get_next_line in a loop will then allow you to read the text available on a file descriptor one line at a time until the end of the text, no matter the size of either the text or one of its lines.
get_next_line can also read from multiple file descriptors; the function will store the next line of a file correctly even when other files are read.

