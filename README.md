# Get Next Line Project

Welcome to the Get Next Line project! 📜 This project involves creating a function named `get_next_line` that reads a line from a file descriptor.

## Function Prototype
```c
char *get_next_line(int fd);
```

## Files to Submit
Turn in the following files:

- `get_next_line.c`
- `get_next_line_utils.c`
- `get_next_line.h`

## Parameters
- 📄 `fd`: The file descriptor to read from

## Return Value
- 📜 Read line: Correct behavior
- `NULL`: There is nothing else to read, or an error occurred

## External Functions
- 📚 `read`
- 🧠 `malloc`
- 🗑️ `free`

## Description
Write a function that returns a line read from a file descriptor.
- Repeated calls to `get_next_line()` should let you read the text file pointed to by the file descriptor, one line at a time.
- The function should return the line that was read. If there is nothing else to read or if an error occurred, it should return `NULL`.
- Ensure that the function works as expected both when reading a file and when reading from the standard input.
- The returned line should include the terminating `\n` character, except if the end of the file was reached and does not end with a `\n` character.
- The header file `get_next_line.h` must at least contain the prototype of the `get_next_line()` function.
- Add all the helper functions you need in the `get_next_line_utils.c` file.

## Compiler Option
Because you will have to read files in `get_next_line()`, add this option to your compiler call:
```bash
$ cc -Wall -Wextra -Werror -D BUFFER_SIZE=n <files>.c
```
Happy coding! 🚀
