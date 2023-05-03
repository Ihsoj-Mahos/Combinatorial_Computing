# Week 1

In this week, we shall be focusing upon Computer Representation of Mathematical Objects. The content to be covered is given below. Though we will eventually focus on the implementation, a lot of math is going to be involved in this SoC. So, it is highly encouraged for you to ask doubts on the whatsapp group :) 

## Reading 

1. Chapter 1, 2 of [Elements of Combinatorial Computing by Wells](../Elements_of_Combinatorial_Computing.pdf) (optional, as this describes the definitions of terms we use in everyday programming. Not really necessary, but you can check it out if interested)
2. Chapter 3 of [Elements of Combinatorial Computing by Wells](../Elements_of_Combinatorial_Computing.pdf). (this is really what we are interested in :))

Further reading and assignments will be updated soon.

## Assignment Problems

### 1. Fun with Ferrer

#### Making a ferrer diagram

In this question, we will explore the concept of Ferrer's diagrams (given in section 3.3.4 of [Elements of Combinatorial Computing](../Elements_of_Combinatorial_Computing.pdf)). These diagrams are extremely useful to show the partitions of a number. Here, you have to write `C++` code which takes in a partition of the form (a, b, c, ...) and prints the corresponding ferrer diagram in the terminal. 

For example, for `7 = 3 + 2 + 1 + 1`, i.e. (3, 2, 1, 1), the ferrer diagram is given by 
```
***
**
*
*
```

For this part, please submit a file named `ferrer_part_a.cpp` or `ferrer_part_a.c`

#### Enumerating number of partitions (with a twist)

In this part, we use computing in order to verify an important result about partitions. Let's introduce some notation.
Let `Q(n,k)` denote the number of partitions in which the largest number is atmost `k`. For `n = 5, k = 3` these are `3+2, 3+1+1, 2+2+1, 2+1+1+1, 1+1+1+1+1` so `Q(5,3) = 5`. 

Let `R(n,k)` denote the number of partitions where the number of numbers is atmost `k`.
For `n = 5, k = 3` it is `5, 4+1, 3+2, 3+1+1, 2+2+1` so `R(5,3) = 5`.
Given inputs `n, k`, return `Q(n, k) R(n, k)`. Input will be two space separated integers, i.e., 

```
Input : 5 3
Output : 5 5
```

For this part, please submit a file named `ferrer_part_b.cpp` or `ferrer_part_b.c`.

Now, for `n = 5, k = 3` we got `Q(n, k) = R(n, k)`. Do you think this was a coincidence? Try running your code for multiple values of `n` and `k` to check whether it is. Well, you might have guessed at this point that it isn't :) 

So here's the next part of the question. Prove that `Q(n, k) = R(n, k)` for all values of `n` and `k`. (Submit this part as `proof_ferrer.pdf`) 


