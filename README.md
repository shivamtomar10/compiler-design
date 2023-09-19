 <h1 align="center"> COMPILER-DESIGN </h1>
 
 A **compiler** is a software which converts the ***high-level language*** (source-code) into the ***low-level language*** (object or target program).

<p align="center"><img src="https://static.javatpoint.com/compiler/images/the-phases-of-a-compiler-lexical-analysis.png"</img></p>

<h2>Phases of compiler for which we have to write code for its design</h2>

<p align="center"><img src="https://media.geeksforgeeks.org/wp-content/uploads/compilerDesign.jpg"</img></p>


<h4> Preprocessor </h4> 
When you write code in any language (source-code) its remove all header files and comments from it so that it becomes pure high level language.

<h4> Compiler </h4>
Its get pure HLL from preprocessor and then its phases starts its work to convert the HLL to assembly code.

<h4> Assembler </h4>
When Assembler get assembly code from compiler so it get converted into relocatable machine code.

<h4> Linker/Loader </h4>
Relocatable machine code gets converted into absolute machine code.

<h3>Let's discuss how the phases of compiler converting the HLL into the assembly code : that's the main work/task</h3>

<h4> Lexical Analysis </h4>
This first phase count the number of lexemes/tokens.

**Lexemes** : Lexemes are the character strings assembled from the character stream of a program </br>
**Tokens** : Token represents what component of the program's grammar they constitute.</br>


<p align="center"><img src="https://binaryterms.com/wp-content/uploads/2021/11/Tokens.jpg"</img></p>
