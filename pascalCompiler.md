A Basic pascal Compiler using lex and yacc

# Introduction #

Every programming language needs a compiler. It is just a basic compiler
for pascal which use lex and yacc to implement code. Codes are basically written
in C++. Some knowledge about Regular Expression and a good knowledge of context
free grammar is needed. I implemented a basic pascal compiler upto intermediate code
generation.For this, some knowledge of assembly language is also needed.


# Details #

To write a compiler using lex and yacc, I used fedora 8. Other linux can also be used.
Then you have to install packages necessary to install lex and yacc.

After you have successfully done this, you have to go for writing the lex file.
It is where you need regular expression. It is needed for your compiler to recognize some pattern or keywords. For example, in C we can write a single line or multi-line comment which have some patterns. We can use regexp to find this pattern. So, lex is intended to do that pattern matching things.

We will also need a symbol table for storing identifiers, numbers for calculation etc. It can be efficiently implemented using hash table. The efficiency of it depends on the efficiency of hash function.

Now, we have to do the big job. Writing a perfect grammar is very important to create a compiler. Knowledge of context free grammar is needed here. This is the work for yacc part.
After implementing the grammar the first work will be to check whether we can work with it perfectly.

Then using lexfile, grammar, symbol table and some additional coding , we have to give our output as a assembly file.

So, given a pascal source file we can output a assembly file now.