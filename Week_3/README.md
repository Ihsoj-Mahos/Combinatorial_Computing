# Week 3

In this week, we shall be focusing upon Satisfiability and SAT Solvers. The content to be covered is given below. Though we will eventually focus on the implementation, a lot of math is going to be involved in this SoC. So, it is highly encouraged for you to ask doubts on the whatsapp group :)

## Reading

In this week, you will require a basic knowledge of computer logic, which will include stuff like boolean expressions, the SAT problem, SAT Solvers. Till now, you have been coding all the logic yourself, which takes an input and gives an output. However, programming with SAT Solvers is different. SAT Solvers are like an engine that is really good at solving the satisfiability problem. Hence, programmers encode the problem as a SAT problem, and "feed" it to a SAT Solver for the answer. This approach is very useful and is a good fall-back option when you don't have an efficient algorithm :)

We will be giving you resources from CS228 (logic in computer science) as well in this week.

1. Lecture slides [1](SAT_encoding_1.pdf), [2](SAT_encoding_2.pdf) covers encoding problems into CNF (the standard form used by SAT Solvers), and covers a few examples related to how the conversion is done.

## Problems

### Sudoku Solver

You might have solved a sudoku using your brain, or a brute force approach before. However, in this problem you have to encode the problem as SAT, and let the SAT Solver do the job. 

```
Input : Space separated 81 digits in row major form (each set of 9 digits is a line from left to right), 0 indicates the absence of a digit. 
Output : Give one possible solution (as a set of 81 digits) if possible, print -1 if not.
```
