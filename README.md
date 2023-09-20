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
<p></p>

**Lexemes** : Lexemes are the character strings assembled from the character stream of a program. </br>
**Tokens** : Token represents what component of the program's grammar they constitute.

<p align="center"><img src="https://binaryterms.com/wp-content/uploads/2021/11/Tokens.jpg"</img></p>

<h4>Now Let's see how compiler make the Lexemes and Tokens table by going through the pure HLL.</h4>
<p>If you consider a code in which one line is "x=a+b*c" then lexemes and tokens are define like the below table.</p>
<p align="center"><img src="https://github.com/shivamtomar10/compiler-design/blob/master/lexemes.png"</img></p>

When this lexemes and token table get built for the whole source code like for the one line we have shown above, this passes to the synatx analysis phase.

<h4> Syntax Analysis </h4>

In this phase , on the basis of some production rule **PARSE TREE** form and then yielding of this tree accord to *top/bottom* and *left/right* approach.

<p align="center"><img src="https://github.com/shivamtomar10/compiler-design/blob/master/parse.png"</img></p>

If yielding of this tree result out the same of that lexemes and token table then there is no syntax error in the source code .

Now you can see in the above image that yielding of parse tree result out **id=id+id*id** which is similar to the lexemes and token table values as **x=a+b*c**.
So, this line **x=a+b*c** has no syntax error.
<p></p>

 <h4 align="center"> PARSER CLASSIFICATION </h4>
 <p align="center"><img src="https://github.com/shivamtomar10/compiler-design/blob/master/parseclassification.png"</img></p>
