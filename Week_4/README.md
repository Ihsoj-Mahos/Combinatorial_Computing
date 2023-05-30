# Week 4

In this week, we shall be focusing upon Generation of elementary configurations. The content to be covered is given below. Though we will eventually focus on the implementation, a lot of math is going to be involved in this SoC. So, it is highly encouraged for you to ask doubts on the whatsapp group :)

## Some interesting stuff

At this point you're probably wondering what [this](../delaunay.png) thing is. This is a type of triangulation called the "delaunay triangulation". Basically, given a set of discrete points, can you triangulate them so that no point lies inside the circumcircles of resulting triangles. This has polynomial time algorithms and the history of this is quite interesting, can be found [here](https://en.wikipedia.org/wiki/Delaunay_triangulation). [This](https://www.sciencedirect.com/science/article/pii/S0010448597000821) is a very good paper about the delaunay triangulation.

## Reading

In this week, we will cover generation of elementary configurations, partitions, sets, permutations and some random discrete math stuff. 

1. Posets and lattices are interesting mathematical objects, since they occur quite frequently in computer science and have interesting properties. [This](Posets.pdf) handout covers the basic properties of posets, defines lattices. Moreover, whenever posets arise, dilworth's theorem and mirsky's theorem seem to be useful. [This](https://math.ucdenver.edu/~wcherowi/courses/m7409/acln10.pdf) handout covers them along with hall's matching theorem and many others. Often you have many theorems that are equivalent or one derives others. The handout covers the relationship between various such theorems as well.

2. Equivalence relations also occur quite frequently in problems, and are also interesting to study. [This](EquivalenceRelations.pdf) handout defines them and gives some examples. [This](https://www.cs.sfu.ca/~ggbaker/zju/math/equiv-rel.html) is another source which relates equivalence relations and partitions.

3. Read chapter 5 from [Elements of Combinatorial Computing](../Reference_books/Elements_of_Combinatorial_Computing.pdf) by Wells.

## Problems

### Theory

1. [This](equivalence_exercise.pdf) is an exercise sheet based upon equivalence relations, and [this](posets_exercise.pdf) exercise covers posets. They may require other theorems such as induction, recurrences, etc. If any terms feel unfamiliar, feel free to ask. (p.s. the problems were a part of the course "discrete structures" by Prof. Diwan, so don't be surprised if they're challenging :p)

### Coding

#### 1. Bipartite Maching

This is a classic bipartite matching problem which needs to be solved using the algorithmic proof of hall's theorem. You are given $n$ workers and $m$ jobs. Each worker is willing to do some jobs between $1$ and $m$. Also, one job can be done by atmost one worker and each worker can do atmost one job. Can you assign a job to each worker? 

```
Input : n m
<n lines with each line containing the number of jobs (k) that a worker is willing to do followed by k space separated integers>

Output : <n lines with each line having two space separated integers which are worker, job if assignment possible, just print -1 if not possible>
```
