![[Logical Equivalences.png]]
![[Conditional Logical Equivalences.png]]
![[Rules of Inference.png]]
s: George is a spider
e: George has 8 legs
If George does not have 8 legs, he is not a spider

0. ~e -> ~s
1. s
2. e by modus tollens on 0 and 1
---
0. ~e -> ~s
1. s
2. e | ~s   equivalent to 0
3. s | F      equivalent to 1
4. e | F     res 2 and 3
5. e          simplify
# Proof by Contradiction
0. ~e -> ~s
1. s
2. ~e      proof by contradiction
3. ~s      Modus ponens on 2 and 0
4. F        by 1 and 3
---
Assumptions
- Logic is difficult and not many students like logic
- If mathematics is easy then logic is not difficult
Propositions
- d: logic is difficult
- s: students like logic
- m: math is easy

prove s -> ~m
1. d & ~s
2. m -> ~d
3. ~(s -> ~m) proof by contradiction 
4. ~m | ~d equiv to 2
5. ~(~s | ~m) equiv to 3
6. s & m equiv to 5
7. d 
8. ~s
9. False


prove: Not many students like logic if mathematics is not easy
~m -> ~s
1. d & ~s
2. m -> ~d
3. ~(~m -> ~s) proof by contradiction
4. ~m | ~d equiv to 2
5. ~(m | ~s) equiv to 3
6. ~m & s equiv to 5
7. s