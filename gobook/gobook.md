# The Go Programming Language

- Package: Go code is organized into packages, which are similar to libraries or modules
in other languages. A package consits of one or more .go source files in a
single directory that define what the package does. Each source file begins with
a package declaration,that states which package the file belongs to, followed by
a list of other packages that it imports, and then the declarations of the
program that are stored in that file.

- Package main is special. It defines a standalone executable program, not a
library. Within package main the function main is also special - it's where
execution of the program begins.

- A function declaration consists of the keyword func, the name of the function,
a parameter list, a result list, and the body of the function - the statements
that define what id does - enclosed in braces.

- Variable can be declared in any of the following forms:
```
s := "" // can only be used within a function
var s string // default initialization to the zero value for strings
var s = ""
var s string = ""
```
In practice, you should generally use one of the first two forms, with explicit
initialization to say that the initial value is important and implicit
initialization to say that the initial value doesn't matter.