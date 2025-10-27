## antlr grammar practice
``` python
grammar Datalog;

datalog
  : SCHEMES COLON 
  scheme scheme_list
  FACTS COLON EOF
  ;
  
scheme_list
  : scheme scheme_list
  |
  ;
  
scheme
  : ID LEFT_PAREN ID id_list RIGHT_PAREN
  ;
  
id_list
  : COMMA ID id_list
  |
  ;

COLON
  : ':'
  ;
  
COMMA 
  : ','
  ;
  
FACTS
  : 'Facts'
  ;
  
SCHEMES 
  : 'Schemes'
  ;
  
LEFT_PAREN
  : '('
  ;
  
RIGHT_PAREN 
  : ')'
  ;
  
ID
  : [a-zA-Z][a-zA-Z0-9]*
  ;

WS
  : [ \n\t\r]+ -> skip
  ;
```
![[datalog-tree.png]]
``` python
grammar time;

time
  : HOUR ':' (HOUR | MINUTES) HALF time EOF
  |
  ;
  
HOUR
  : [1-9]
  | [1][0-2]
  ;
  
MINUTES
  : [0-5][0-9]
  ;
  
HALF
  : 'am'
  | 'pm'
  ;
  
WS
  : [ \n\t\r]+ -> skip
  ;
```
![[time-tree.png]]