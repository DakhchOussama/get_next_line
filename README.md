# get_next_line
Calling your function get_next_line in a loop will then allow you to read the text
available on the file descriptor one line at a time until the end of it.
• Your function should return the line that has just been read. If there is nothing
else to read or if an error has occurred it should return NULL.
• Your read must use the BUFFER_SIZE defined during compilation to read from
a file or from stdin. This value will be modified during the evaluation for testing
purposes.
