---
published: true
---
## A New Post
**Additonal Chaper 1 learning**

Stars and bars allows us to count the number of ways to distribute 10 cookies to 3 kids and natural number solutions to x+y+z=11, for example. A relatively easy modification allows us to put a lower bound restriction on these problems: perhaps each kid must get at least two cookies or x,y,z>=2. This was done by first assigning each kid (or variable) 2 cookies (or units) and then distributing the rest using stars and bars.

What if we wanted an upper bound restriction? For example, we might insist that no kid gets more than 4 cookies or that x,y,z<=4. It turns out this is considerably harder, but still possible. The idea is to count all the distributions and then remove those that violate the condition. In other words, we must count the number of ways to distribute 11 cookies to 3 kids in which one or more of the kids gets more than 4 cookies. For any particular kid, this is not a problem; we do this using stars and bars. But how to combine the number of ways for kid A, or B or C? We must use the PIE.

The Principle of Inclusion/Exclusion (PIE) gives a method for finding the cardinality of the union of not necessarily disjoint sets. o find how many things are in one or more of the sets A, B, and C, we should just add up the number of things in each of these sets. However, if there is any overlap among the sets, those elements are counted multiple times. So we subtract the things in each intersection of a pair of sets. 

For four or more sets, we do not write down a formula for PIE. Instead, we just think of the principle: add up all the elements in single sets, then subtract out things you counted twice (elements in the intersection of a pair of sets), then add back in elements you removed too often (elements in the intersection of groups of three sets), then take back out elements you added back in too often (elements in the intersection of groups of four sets), then add back in, take back out, add back in, etc. This would be very difficult if it wasn't for the fact that in these problems, all the cardinalities of the single sets are equal, as are all the cardinalities of the intersections of two sets, and that of three sets, and so on. Thus we can group all of these together and multiply by how many different combinations of 1, 2, 3, … sets there are.

You might worry that to count surjective functions when the codomain is larger than 3 elements would be too tedious. We need to use PIE but with more than 3 sets the formula for PIE is very long. However, we have lucked out. As we saw in the example above, the number of functions which exclude a single element from the range is the same no matter which single element is excluded. Similarly, the number of functions which exclude a pair of elements will be the same for every pair. With larger codomains, we will see the same behavior with groups of 3, 4, and more elements excluded. So instead of adding/subtracting each of these, we can simply add or subtract all of them at once, if you know how many there are. This works just like it did in for the other types of counting questions in this section, only now the size of the various combinations of sets is a number raised to a power, as opposed to a binomial coefficient or factorial. 

We have seen that counting surjective functions is another nice example of the advanced use of the Principle of Inclusion/Exclusion. Also, counting injective functions turns out to be equivalent to permutations, and counting all functions has a solution akin to those counting problems where order matters but repeats are allowed (like counting the number of words you can make from a given set of letters).

**2.1**

A sequence is simply an ordered list of numbers. For example, here is a sequence: 0, 1, 2, 3, 4, 5, …. This is different from the set  because, while the sequence is a complete list of every element in the set of natural numbers, in the sequence we very much care what order the numbers come in. For this reason, when we use variables to represent terms in a sequence they will look like this: a0,a1,a2,a3

A recursive definition (sometimes called an inductive definition) for a sequence  consists of a recurrence relation : an equation relating a term of the sequence to previous terms (terms with smaller index) and an initial condition: a list of a few terms of the sequence (one less than the number of terms in the recurrence relation).

A closed formula for a sequence is a formula for using a fixed finite number of operations on n. This is what you normally think of as a formula in n, just as if you were defining a function in terms of  (because that is exactly what you are doing).

Finding closed formulas, or even recursive definitions, for sequences is not trivial. There is no one method for doing this. Just as in evaluating integrals or solving differential equations, it is useful to have a bag of tricks you can apply, but sometimes there is no easy answer.

One useful method is to relate a given sequence to another sequence for which we already know the closed formula. To do this, we need a few “known sequences” to compare mystery sequences to. Here are a few that are good to know. We will verify the formulas for these in the coming sections.

**Problem 18**

When bees play chess, they use a hexagonal board like the one shown below. The queen bee can move one space at a time either directly to the right or angled up-right or down-right (but can never move leftwards). How many different paths can the queen take from the top left hexagon to the bottom right hexagon? Explain your answer, and this relates to the previous question. (As an example, there are three paths to get to the second hexagon on the bottom row.)

**Answer**

Since we have to reach nth cell of the first row you have to do n-1^k cell of the first roll to the second row

bn=an+bn-1 ... 2

Since we can get to the nth cell of the second row from the nth cell of the first row or the n-1th cell of the second row

bn=an+bn-1
an=bn-bn-1
an=an-1 + bn-2

an=an-1 + bn-1
(bn-1 - bn-2 )+ bn-1

bn = an+bn-1
(2bn-1 - bn-2) +bn-1
3bn-1 - bn-2

bn=3bn-1 - bn-2 , n>=2
b0=0
b1=1

3b1 -b0
3(1)-0 =3

b3 = 3b2-b1
=3(3)-1 =8

b4 =33b3 -b2
=3(8)-3=21

b5 = 3b4 - b3 = 
3(21)-8=55

b6 = 3b5 -b4 
3(55) - 21=144

144 paths

**2.2 Arithmetic and Geometric Sequences**

Arithmetic Sequences.
If the terms of a sequence differ by a constant, we say the sequence is arithmetic. If the initial term (a0) of the sequence is a and the common difference is d, then we have,

Recursive definition: an=an-1+d  with .a0=a

Closed formula: an =a+dn

What about sequences like 2,6,18,54? This is not arithmetic because the difference between terms is not constant. However, the ratio between successive terms is constant. We call such sequences geometric.

Geometric Sequences.
A sequence is called geometric if the ratio between successive terms is constant. Suppose the initial term a0 is a and the common ratio is r. Then we have,

Recursive definition: an=ra_n-1  with a0=a.

Closed formula: an =a * r^n

Look at the sequence which starts 1,3,6,10,15. These are called the triangular numbers since they represent the number of dots in an equilateral triangle (think of how you arrange 10 bowling pins: a row of 4 plus a row of 3 plus a row of 2 and a row of 1).

Notice that the differences between terms do form an arithmetic sequence:2,3,4,5,6 . This means that the nth term of the sequence (Tn) is the sum of the first n terms in the sequence 1,2,3,4,5 . We say that (Tn) is the sequence of partial sums of the sequence 1,2,3 (partial sums because we are not taking the sum of all infinitely many terms).

**Problem 10**

 If you have enough toothpicks, you can make a large triangular grid. Below, are the triangular grids of size 1 and of size 2. The size 1 grid requires 3 toothpicks, the size 2 grid requires 9 toothpicks.
 
 A.Let tn be the number of toothpicks required to make a size n triangular grid. Write out the first 5 terms of the sequence t1,t2....
 
 B.Find a recursive definition for the sequence. Explain why you are correct.
 
 C.Is the sequence arithmetic or geometric? If not, is it the sequence of partial sums of an arithmetic or geometric sequence? Explain why your answer is correct.

 D.Use your results from part (c) to find a closed formula for the sequence. Show your work.


**Answer**

A. t1=3 , t2=9(3+6) , t3=18(3+6+9), t4= 30= (3+6+9+12), t5= 45 (3+6+9+12+15)


B. an = an01 +3b
a2=1+b
3+6=9
a3=a2+3*3
9+9=18
a4 = a3 + 3*4
18+12=30
the definition is correct

C.

3=3
9=3+6
18=3+6+9
30=3+6+9+12
45=3+6+9+12+15
=3+6+9+12+45+ 3n


3,9,18,30,45... is the sum of the arithmetic sequence.

D.

3=3
9=3+6
18=3+6+9
30=3+6+9+12
45=3+6+9+12+15
=3+6+9+12+45+ 3n

(3n(n+1))/2 is the closed formula

**2.3 Polynomial Fitting**

So far we have seen methods for finding the closed formulas for arithmetic and geometric sequences. Since we know how to compute the sum of the first  terms of arithmetic and geometric sequences, we can compute the closed formulas for sequences which have an arithmetic (or geometric) sequence of differences between terms. But what if we consider a sequence which is the sum of the first n terms of a sequence which is itself the sum of an arithmetic sequence?

Before we get too carried away, let's consider an example: How many squares (of all sizes) are there on a chessboard? A chessboard consists of 64 squares, but we also want to consider squares of longer side length. Even though we are only considering an 8x8 board, there is already a lot to count. So instead, let us build a sequence: the first term will be the number of squares on a 1c1 board, the second term will be the number of squares on a 2x2 board, and so on. After a little thought, we arrive at the sequence 1,5,14,30,55

This sequence is not arithmetic (or geometric for that matter), but perhaps it's sequence of differences is. For differences we get 4,9,16,25


Not a huge surprise: one way to count the number of squares in a 4x4 chessboard is to notice that there are 16 squares with side length 1, 9 with side length 2, 4 with side length 3 and 1 with side length 4. So the original sequence is just the sum of squares. Now this sequence of differences is not arithmetic since it's sequence of differences (the differences of the differences of the original sequence) is not constant. In fact, this sequence of second differences is 5,7,9


The closed formula for a sequence will be a degree k polynomial if and only if the sequence is k-constant (i.e., the kth sequence of differences is constant).This tells us that the sequence of numbers of squares on a chessboard,1,5,14,30,55, which we saw to be 3-constant, will have a cubic (degree 3 polynomial) for its closed formula.Now once we know what format the closed formula for a sequence will take, it is much easier to actually find the closed formula. In the case that the closed formula is a degree k polynomial, we just need k+1 data points to “fit” the polynomial to the data.

**Problem**
Give two different recursive definitions for the sequence with closed formula an=3+2n . Prove you are correct. At least one of the recursive definitions should makes use of two previous terms and no constants.

**Answer**
First you do
an-1 = 3+2(n-1)
=3+2n-2
an-1 = an-2 (an=3+2n)
This makes it equal to 
an=an-1+2 where a1 would equal 5
in the end you get a1=5 and an=an-1+2 which equals to an=3+2n

**2.4 Solving Recurrence Relations**

We have seen that it is often easier to find recursive definitions than closed formulas. Lucky for us, there are a few techniques for converting recursive definitions to closed formulas. Doing so is called solving a recurrence relation. Recall that the recurrence relation is a recursive definition without the initial conditions. For example, the recurrence relation for the Fibonacci sequence is Fn=Fn-1+Fn-2. (This, together with the initial conditions F0=0 and F1=1 give the entire recursive definition for the sequence.)

We are going to try to solve these recurrence relations. By this we mean something very similar to solving differential equations: we want to find a function of n (a closed formula) which satisfies the recurrence relation, as well as the initial condition. Just like for differential equations, finding a solution might be tricky, but checking that the solution is correct is easy.

Sometimes we can be clever and solve a recurrence relation by inspection. We generate the sequence using the recurrence relation and keep track of what we are doing so that we can see how to jump to finding just the an term. Here are two examples of how you might do that.

Telescoping refers to the phenomenon when many terms in a large sum cancel out—so the sum “telescopes.” For example:
(2-1)+(3-2)+(4-3)+...+(100-99)+(101-100)=-1+101 

because every third term looks like: 2+-1=0, and then 3+-3=0 and so on. We can use this behavior to solve recurrence relations. 

**Problem***

Solve the recurrence relation an=2an-1 - an-2.
a.What is the solution if the initial terms are a0=1 and a=2 ?
b.What do the initial terms need to be in order for a9=30 ?
c.For which  are there initial terms which make a9?

**Answer**
a. We have characteristic polynomial x^2-2x+1, which has x-1 as the only repeated root.  THe recucurence relation would have to be an = 1+n

b. For a9=30 Wen using the equation aboive a9=1+9=10. This means that the difference is 30-10 which equals to 20 the term should be a0 = 1+20 =21 and a1= 2+20=22

c. For the intial termwhich makes a9 you have to to be 
a0= 1+(x-10)=x=9 
a1=2+(x-10)= x-8

**3.1 Propositional Logic**

A proposition is simply a statement. Propositional logic studies the ways statements can interact with each other. It is important to remember that propositional logic does not really care about the content of the statements. For example, in terms of propositional logic, the claims, “if the moon is made of cheese then basketballs are round,” and “if spiders have eight legs then Sam walks with a limp” are exactly the same. They are both implications: statements of the form, P -> Q.

We need to decide when the statement (P -> Q)V(Q -> P) is true. Using the definitions of the connectives in Section 0.2, we see that for this to be true, either P -> Q must be true or Q -> P must be true (or both). Those are true if either P is false or Q is true (in the first case) and Q is false or R is true (in the second case). So—yeah, it gets kind of messy. Luckily, we can make a chart to keep track of all the possibilities. Enter truth tables. The idea is this: on each row, we list a possible combination of T's and F's (for true and false) for each of the sentential variables, and then mark down whether the statement in question is true or false in that case. We do this for every possible combination of T's and F's. Then we can clearly see in which cases the statement is true or false. For complicated statements, we will first fill in values for each part of the statement, as a way of breaking up our task into smaller, more manageable pieces.

Since the truth value of a statement is completely determined by the truth values of its parts and how they are connected, all you really need to know is the truth tables for each of the logical connectives. 

Logical Equivalence aretwo (molecular) statements P and Q are logically equivalent provided P is true precisely when Q is true. That is, P and Q have the same truth value under any assignment of truth values to their atomic parts.

To verify that two statements are logically equivalent, you can make a truth table for each and check whether the columns for the two statements are identical.

**Problem**

12. Determine if the following deduction rule is valid:
P V Q
 ¬P
 -----
 ∴Q
 
 **Answer**
 
 To check it is valid or not you can make a truth table
 
 P | Q |¬P | P V Q | (P V Q) ^ ¬P | ((P V Q) ^ ¬P )¬Q
--------------------------------------------------------
 T | T | F |   T   |       F      |        T         
 T | F | F |   T   |       F      |        T   
 F | T | T |   T   |       t      |        T         
 F | F | T |   F   |       F      |        T         
 
 This shows that the truth value of Q in the rows that have  P V Q and  ¬P are true.