# Regular Expression Compiler

An implementation of a regular expression parser, compiler and matcher. Consists of two main programs, `REcompile` and `REsearch` that
can be used together to search through files for instances of the given regular expression. Under the hood a finite state machine is built
and shared between the two programs.

Blank lines will result in no matches as there is no content, even if the pattern matches with nothing.

## Usage

To compile a regex expression:

- `java REcompile [expression]`

To search through a file for pattern instances (FSM is read from standard input)

- `java REsearch [filename]`

See [here](https://github.com/luke-finlayson/regex/wiki/Operations-&-Expressions) for valid regex syntax and full documentation.
