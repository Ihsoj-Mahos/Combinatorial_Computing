# Week 5

In this week, we shall be focusing upon miscellaneous algorithmic methods. We'll cover some basic methods as well as some stuff related to matchings. The content to be covered is given below.

## Reading 

This section of the project is closely related to design and analysis of algorithms (CS218) offered by the CSE Department. So, we will be using some content directly from this course

1. Read chapter 6 from [Elements of Combinatorial Computing](../Reference_books/Elements_of_Combinatorial_Computing.pdf) by Wells.

2. Some reading about greedy algorithms and dynamic programming from CS218 [slides](https://www.cse.iitb.ac.in/~rgurjar/CS218_2023/slides/GreedyDPSlides.pdf) by Prof. Rohit Gurjar. In order to understand the flavor of these techniques, you can read [this](https://connect2grp.medium.com/dynamic-programming-vs-greedy-approach-c132de5bff44) blog post.

3. Network flow forms the basis of many problems. The basics of that can be found [here](https://www.cse.iitb.ac.in/~rgurjar/CS218_2023/slides/NetworkFlow.pdf) 

## Problems

### Theory

1. Referencing the first coding problem of this week, try to think why the approach given in the link works. That is, give a proof that the conversion of the matching problem to network flow gives the correct maximum matching (using ideas from max-flow min-cut theorem).

### Coding

#### 1. Bipartite Matching

Remember the first problem of last week's problems? This time we will solve the exact same problem but using network flow. In order to get an idea of how to do this, refer [this](https://www.geeksforgeeks.org/maximum-bipartite-matching/) link.  
You are given $n$ workers and $m$ jobs. Each worker is willing to do some jobs between $1$ and $m$. Also, one job can be done by atmost one worker and each worker can do atmost one job. Can you assign a job to each worker? 

```
Input : n m
<n lines with each line containing the number of jobs (k) that a worker is willing to do followed by k space separated integers>

Output : <n lines with each line having two space separated integers which are worker, job if assignment possible, just print -1 if not possible>
```
