# interpreter-in-go
Implementing an interpreter for an imaginary language with reference to "Thorsten Ball - Writing An Interpreter In Go"

### Features of the language
- C-like syntax
- variable bindings
- integers and booleans
- arithmetic expressions
- built-in functions
- first-class and higher-order functions
- closures
- a string data structure
- an array data structure
- a hash data structure

### Structure of the Interpreter
**Lexer** - Supports ASCII Characters, identifiers contain only letters, whitespaces are seperators (not a part of syntax)    

**Parser** -  Recursive-Descent Parser, uses an AST (Abstract Syntax Tree), built from ground up, Top-Down Operator Precedence (Pratt Parser), Prefix and Postfix Expression parsing    

**Evaluator** - Tree-walking interpreter, uses Go's inbuilt Garbage Collector, contained scopes (termed Environments), all values are "Objects"
