---
published: true
---
##

Course summary 

Class math 2720 also known as Discrete Math at CSUSB is a class about combinatorics, sequences, symbolic logic, and graph theory. 


(1)
A statement is any declarative sentence that is either true or false. A statement is atomic if it cannot be divided into smaller statements, otherwise, it is called molecular. You can build more complicated (molecular) statements out of simpler (atomic or molecular) ones using logical connectives.

P ^ Q is true when both P and Q are true (conjunction)

P v Q is true when P or Q or both are true (disjunction)

P -> Q is true when P is false or Q is true of both (implication or conditional)

P<-> Q is true when P and Q are both true or both false (biconditional)

P is read “not P” and called a negation (negation)> We loved with a love that was more than love



(2)
A set is a unordered collection of objects. These objects are sometimes called elements or members of the set. Representing sets are like Listing enumerating the members of the set or the definition by property, using the set builder notation A set A is said to be a subset of B if and only if every element of A is also an element of B.

The empty set is the set that contains no elements. “Ø”

The universe set is the set of all elements. “U”

The set of natural numbers. That is,N = {0,1,2,3..} . “N”

The set of integers. That is, Z={..,-2,-1,0,1,2,3,…} . “Z”

The set of rational numbers. “Q”

The set of real numbers. “R”

The power set of any set A is the set of all subsets of A “P(A)”

(3)
A function is a rule that assigns each input exactly one output. We call the output the image of the input. The set of all inputs for a function is called the domain. The set of all allowable outputs is called the codomain. We would write f: X -> Y to describe a function with name f, domain X, and codomain Y. This does not tell us which function f is though. To define the function, we must describe the rule. This is often done by giving the formula to compute the output for any input. The set of natural numbers that output is called the range of the function.

For a function f: N -> N, a recursive definition consists of an initial condition together with a recurrence relation. The initial condition is the explicitly given value of f(0). The recurrence relation is a formula in terms of f(n+1) (and f(n) possibly n itself).

A surjection is a function for which every element of the codomain is in the range. How many of the functions?

An injection is a function f that maps distinct elements of its domain to distinct elements.

An injection bijections if a function f: X → Y satisfied the properties of surjective function (onto function) and injective function (one-to-one function).

(4)
Additive Principle (with sets). Given two sets A and B, if An B = Ø (that is if there is no element in common to both A and B), then |AUB| = |A| + |B|

Cartesian Product. Given sets A and B, we can form the set A x B = ((x,y) : x ∈ A ^ y ∈ B] to be the set of all ordered pairs (x, y) where a is an element of A and y is an element of B. We call A x B the Cartesian product of A and B.

Multiplicative Principle. The multiplicative principle states that if event A can occur in m ways, and each possibility for A allows for exactly n ways for event B, then the event “ A and B” can occur in m - n ways.

(5)
Bit Strings “Bit” is short for “binary digit,” so a bit string is a string of binary digits. The binary digits are simply the numbers 0 and 1. All of the following are bit strings:1001, 0, 1111,

Bit Strings. An n-bit string is a bit string of length n. That is, it is a string containing n symbols, each of which is a bit, either 0 or 1.

Binomial coefficients are the coefficients in the expanded version of a binomial, such as (x+y)^5. What happens when we multiply such a binomial out? We will expand (x=y)^n for various values of n


(6)
In general, we can ask how many permutations exist of k objects choosing those objects from a larger collection of n objects.  We write this number P(n,k) and sometimes call it a k-permutation of n elements. From the example above, we see that to compute P(n,k), we must apply the multiplicative principle to k numbers, starting with n and counting backwards.

k-permutations of n elements. P(n,k) is the number of k-permutations of n elements, the number of ways to arrange k objects chosen from n distinct objects.

(7)
Stars and bars allows us to count the number of ways to distribute 10 cookies to 3 kids and natural number solutions to x+y+z=11, for example. A relatively easy modification allows us to put a lower bound restriction on these problems: perhaps each kid must get at least two cookies or x,y,z>=2. This was done by first assigning each kid (or variable) 2 cookies (or units) and then distributing the rest using stars and bars.


(8)
Arithmetic Sequences. If the terms of a sequence differ by a constant, we say the sequence is arithmetic.  For instance, the sequence 5, 7, 9, 11, 13, 15 is an arithmetic progression with a common difference of 2.
Geometric Sequences. A sequence is called geometric if the ratio between successive terms is constant.
For example, the sequence 2, 6, 18, 54 is a geometric progression with common ratio 3.

(9)
A proposition is simply a statement. Propositional logic studies the ways statements can interact with each other. It is important to remember that propositional logic does not really care about the content of the statements. For example, in terms of propositional logic, the claims, “if the moon is made of cheese then basketballs are round,” and “if spiders have eight legs then Sam walks with a limp” are exactly the same. They are both implications: statements of the form, P -> Q.




------------------------------------------------------------------------------------------------------------
**4.1**

**summary**

Graph Definition is a graph is an ordered pair G=(V,E) consisting of a nonempty set V (called the vertices) and a set E (called the edges) of two-element subsets of V.

Isomorphic Graphs.
An isomorphism between two graphs G1 and G2 is a bijection f: V1 ->V2 between the vertices of the graphs such that (a,b) is an edge in G1 if and only if (f(a), f(b)) is an edge in G2.

Two graphs are isomorphic if there is an isomorphism between them. In this case we write . G1=G2

An isomorphism is simply a function which renames the vertices. It must be a bijection so every vertex gets a new name. These newly named vertices must be connected by edges precisely when they were connected by edges with their old names.

Sometimes we will talk about a graph with a special name (like Kn or the Petersen graph) or perhaps draw a graph without any labels. In this case we are really referring to all graphs isomorphic to any copy of that particular graph. A collection of isomorphic graphs is often called an isomorphism class. There are other relationships between graphs that we care about, other than equality and being isomorphic

**question**

8. for which n >= 3 is the grpah cn bipartite


**answer**

For n>=3, graph Cn is bipartite if n is even and is not bipartite if n is odd.

If you can color the graph so that the vertices are colored by the same colar it is possible for the graph to be bipartite. 
Cn is bipartite if n is even 
if n is odd it will not be bipartite


------------------------------------------------------------------------------------------------------------
**4.2**

**summary**
Definition of a Tree.
A tree is a connected graph containing no cycles.
A forest is a graph containing no cycles. Note that this means that a connected forest is a tree.

In general, there is no reason for a tree to have this added structure, although we can impose such a structure by considering rooted trees, where we simply designate one vertex as the root.

A tree is a connected graph with no cycles. Is there anything else we can say? It would be nice to have other equivalent conditions for a graph to be a tree. That is, we would like to know whether there are any graph theoretic properties that all trees have, and perhaps even that only trees have.

As soon as one vertex of a tree is designated as the root, then every other vertex on the tree can be characterized by its position relative to the root. This works because there is a unique path between any two vertices in a tree. So from any vertex, we can travel back to the root in exactly one way. This also allows us to describe how distinct vertices in a rooted tree are related.

If two vertices are adjacent, then we say one of them is the parent of the other, which is called the child of the parent. Of the two, the parent is the vertex that is closer to the root. Thus the root of a tree is a parent, but is not the child of any vertex (and is unique in this respect: all non-root vertices have exactly one parent).

**question**
For each degree sequence below, decide whether it must always, must never, or could possibly be a degree sequence for a tree. Justify your answers.
A(3,3,2,2,2,)
B(3,2,2,1,1,1)
C(3,3,3,1,1,1,)
D(4,4,1,1,1,1,1,1,)

**answer**
a. sum 3+3+2+2+2=12 number of edges is 12/2 = 6 
n-1
6-1=5
n is the number of vertices
n=5
n-1=4 does not equal to 6  

not a tree

b. sum 3+2+2+1+1+1 =10 even
10/2 = 5
vertices = 6
n-1=5 number of edges 
IT can form a tree

c.sum 3+3+3+1+1+1=2
edges 12/2=6 does not equal n-1=5

not a tree

d. sum 4+4+1+1+1+1+1+1 =14
edges 14/2 = 7 = n-1
it does form a tree since there are two vertices meaning the graph can be connected. 

------------------------------------------------------------------------------------------------------------
**4.3**

**summary**
Euler's Formula for Planar Graphs.
For any connected planar graph with v vertices, e edges and f faces, we have
v-e+f=2

A polyhedron is a geometric solid made up of flat polygonal faces joined at edges and vertices. We are especially interested in convex polyhedra, which means that any line segment connecting two points on the interior of the polyhedron must be entirely contained inside the polyhedron.

The cube is a regular polyhedron (also known as a Platonic solid) because each face is an identical regular polygon and each vertex joins an equal number of faces.



**question**
3.Is it possible for a connected graph with 7 vertices and 10 edges to be drawn so that no edges cross and create 4 faces? Explain.

**answer**

given v=7 e=10 f=4
v-e+f = 7-10+4
=1 not 2

therefore it is not possible to draw a connected graph.

------------------------------------------------------------------------------------------------------------
**4.4**

**summary**
In general, given any graph G, a coloring of the vertices is called (not surprisingly) a vertex coloring. If the vertex coloring has the property that adjacent vertices are colored differently, then the coloring is called proper. Every graph has a proper vertex coloring. For example, you could color every vertex with a different color. But often you can do better. The smallest number of colors needed to get a proper vertex coloring is called the chromatic number of the graph, written  x(G).

The Four Color Theorem.
If G is a planar graph, then the chromatic number of G is less than or equal to 4. Thus any map can be properly colored with 4 or fewer colors.

A clique in a graph is a set of vertices all of which are pairwise adjacent. In other words, a clique of size n is just a copy of the complete graph Kn. We define the clique number of a graph to be the largest n for which the graph contains a clique of size n. Any clique of size n cannot be colored with fewer than n colors, so we have a nice lower bound.

The chromatic number of a graph G is at least the clique number of G.
**question**
10.Find the chromatic number of the graph below and prove you are correct.
**answer**

the chromatic number of a grph is the smallest amount of color needed to color the vertext. And two adjection points cant be the same color 

after coloring the graph the smallest amount of colors you need is 4 making the comatic number 4.

------------------------------------------------------------------------------------------------------------
**4.5**

**summary**

An Euler path, in a graph or multigraph, is a walk through the graph which uses every edge exactly once. An Euler circuit is an Euler path which starts and stops at the same vertex. Our goal is to find a quick way to check whether a graph (or multigraph) has an Euler path or circuit.

A walk in a graph is a sequence of vertices such that every vertex in the sequence is adjacent to the vertices before and after it in the sequence. If the walk travels along every edge exactly once, then the walk is called an Euler path (or Euler walk).

If, in addition, the starting and ending vertices are the same (so you trace along every edge exactly once and end up where you started), then the walk is called an Euler circuit (or Euler tour).

A graph has an Euler circuit if and only if the degree of every vertex is even.

A graph has an Euler path if and only if there are at most two vertices with odd degree.

In graph theory terms, we are asking whether there is a path which visits every vertex exactly once. Such a path is called a Hamilton path (or Hamiltonian path).
 
We could also consider Hamilton cycles, which are Hamilton paths which start and stop at the same vertex.

**question**
1.  You and your friends want to tour the southwest by car. You will visit the nine states below, with the following rather odd rule: you must cross each border between neighboring states exactly once (so, for example, you must cross the Colorado-Utah border exactly once). Can you do it? If so, does it matter where you start your road trip? What fact about graph theory solves this problem?

**answer**

A= California
B=Nevada
C=Utah
D=Arizona
E=Colorado 
F=New Mexico
G=Kansas
H=Oklahoma
I=Texas

there are two vertices of odd degres being B=Nevada and C=Arizona. The two certices will have an odd degree. You will have to start or end with one of those two states to make the trip.
