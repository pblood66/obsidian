# Balancing Braces
Give a regular expression or FSA that gives $\{^{n} \}^{n}$ . 
	- *cannot do with regex or FSA*
	- Can't count to an arbitrary number 

L(regex) === L(FSA)
- regex generates a language (Generator)
- fsa recognizes membership in a language (Recognizer)

{Regex & FSAs} -> good to recognize patterns but can't count
### Context Free Grammars
Push down Automaton (PDA) - FSA but  you have a stack 
**Recursive Top-Down Parsing** 
Grammars are inherently recursive
Grammars have derivation
- 

*Terminal* - Recursion ends (upper case)
*Non-Terminal* - some rule that invokes Recursion (lower case)

``` python
grammar Braces; 
start
  : braces EOF
  ;

braces 
  : LBRACE braces RBRACE  # BRACES -> lbrace BRACES rbrace
  |                       # or empty string
  ;

LBRACE 
  : {
  ;

RBRACE
  : } 
  ;

WS
  : [ \n\t\r]+ -> skip
  ;
```

Derivation 
start => braces EOF
    => LBRACE braces RBRACE
    => LBRACE $\lambda$ RBRACE

``` python
datalog
  : SCHEMES COLON predicate_list FACTS COLON EOF

predicate_list
  : ID LEFT_PAREN id_list RIGHT_PAREN predicate_list
  | 
  ;


  
```
