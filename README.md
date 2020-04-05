# compiler-project
Compiler's project overview:
This project will direct you to design and build an interpreter for Cool. 
The first phase of the interpreter for cool  is lexical analysi.

# Prerequisites
-Install any ide such as Intellij, NetBeans, Eclipse (Intellij is preferred )

-then follow this link : https://github.com/antlr/antlr4/blob/master/doc/java-target.md

-bring your grammar (in this project it is COOL.g4)

-press Ctrl+Shift+G

# 1)Lexical Analysis:

Introduction :

Lexical analysis is the first phase of a compiler. It takes the modified source code from language preprocessors 
that are written in the form of sentences.The lexical analyzer breaks these syntaxes into a series of tokens, 
by removing any whitespace or comments in the source code. If the lexical analyzer finds a token invalid,
it generates an error. The lexical analyzer works closely with the syntax analyzer.It reads character streams
from the source code, checks for legal tokens, and passes the data to the syntax analyzer when it demand

![](https://raw.githubusercontent.com/asmaa122281/compiler-project/master/lexical%20(1).png)

# Regular Expressions:

A good way of specifying and documenting the lexer is transition diagrams.
More concisely, we can use regular expressions:

    Tokens = Space (Token Space)*
    Token  = TInt | TId | TKey | TSpec 
    TInt   = Digit Digit*
    Digit  = '0' | '1' | '2' |'3' | '4' |'5' | '6' |'7' | '8' | '9'
    TId    = Letter IdChar*
    Letter = 'A' | ... | 'Z' | 'a' | ... | 'z'
    IdChar = Letter | Digit
    TKey   = 'i' 'f' | 'e' 'l' 's' 'e' | ...
    TSpec  = '+''+' | '+' | ...For more info, please check For this link: [GitHub]http://www.cse.chalmers.se/edu/year/2009/course/TIN321_Proglang/lectures/proglang-04.html)



 

