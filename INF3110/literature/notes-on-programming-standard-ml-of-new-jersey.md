# Notes on the document "Notes on Programming Standard ML of New Jersey"

[link to document](http://www.cs.cornell.edu/riccardo/prog-smlnj/notes-011001.pdf)

**Notes cover Sec. 1.1-1.3, 1.6, and sec. 2**

## Chapter 1
### 1.1 - Standard ML
- Standard ML of New Jersey = SML/NJ
- Started as a meta-language for defining proof tactics in interactive theorem provers
- Mostly functional
- Based on model of evaluating expressions
- Functions = first class values
- Allows imperative constructs such as variables, assignment and sequencing of side-effecting operations
- Strongly and statically typed
- Extends basic notation of types with parametric polymorphism
- Has exceptions! Exceptions that can carry functions! (that's pretty bad ass)
- Module system, based on the notions of structures, signatures and functors
- Garbage collected

### 1.2 - Standard ML of New Jersey
- SMLNJ is an interactive compiler for SML
- compiler has a top level loop which compiles declarations and expressions
	  entered by a user.
- Entries are compiled to machine code and executed.
- Can be exported as an executable
- Not batch-oriented like typical OOP compilers
- Not evaluated piece by piece like an interpreter
- Provides extra libraries (modules) to SML
- Also works as a build tool

### 1.3 - History of the system
- SML/NJ started in 1986 by David McQueen, Andrew Appel
- Original purpose was to be a "language laboratory" for programming language research
- The runtime environment is the only part written in C, rest SML
- At time of writing (2001), last version was 110.

### 1.6 - Getting started
- Negative numbers are prepended with ~ (tilde) instead of - (minus), since - is reserved for the subtraction operation
- Variable assignment: ``- val x = 1;`` (type is inferred to be int)
- When you perform an expression, and you don't save it to a variable, the result of the expression will be saved in the
  variable ``it``. You can therefore always access the last performed calculation.
- Functions: ``fun myFunction (oneVar: int, anotherVar int):int oneVar*anotherVar;``
- Write "libraries" of functions in ``*.sml`` files, then import it using ``use path/to/library.sml``
- ``OS.Process.system "ls"`` will execute the ``ls`` command in the shell.


