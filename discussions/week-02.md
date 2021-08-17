# Part II: Programming Paradigms 

Pages 19 to 67 (48 pages)

## Chapter 03 - Paradigm Overview

- **Structured Programming**: prevents the programmer from using a GOTO statement
- **Object-Oriented Programming**: prevents the programmer from "indirect control" (calling private functions, accessing private variables)
- **Functional Programming**: Prevents the programmer from assigning variables (without strict controls)

**Summary** - in each instance a programming paradigm is centered around REMOVING the ability to do something.

### Conclusion 

The three main concers with architecture
- Function
- Separation of components
- Data management

Discussion points: 
- GOLANG and RUST are also languages which impose strict controls on the programmer which prevents the user from inadvertently creating memory leaks
- TypeScript prevents a user from doing all sorts of stuff, making javascript "safer" to work with

## Chapter 04 - Structured Programming

### Proof

- Dijkstra decided to apply mathematical proofs to algorithms. 
- discovered you can't prove something in code with GOTO statements
- created `if/then/else` and `do/while` control structures

- GOTO Statement Considered Harmful 
- **Functional Decomposition** by breaking down code into smaller functions we can mathematically PROVE that it works.
- Formal proofs are possible, but way too much work.
- Testing shows the presence, not the absence, of bugs
- We show that code is correct by *failing to prove it is incorrect* despite our best efforts

### Functional Decomposition:

Architectural best pactice #1 - break large amounts of code into smaller chunks until it is small enough to PROVE.

- This is why we say smaller functions, fewer lines of code per file.
