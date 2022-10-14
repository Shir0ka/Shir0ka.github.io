---
layout: post
title: Portfolio 1
published: true
---
Discrete math

Math 2720-04

Portfolio 1

**About me**

Hello, everyone. My name is Vincent Lam, and I am currently a second-year Computer Science major at the California State University of San Bernadino. I started to enjoy coding recently and have been self-learning python. Some hobbies I enjoy are cooking, eating, and exercising. My goals in the future are to be an above-average software engineer and hopefully improve the world to be a better place than where I found it.


**Course Summary and problem**


**0.2 Mathematical Statements**

A statement is any declarative sentence that is either true or false. A statement is atomic if it cannot be divided into smaller statements, otherwise, it is called molecular. You can build more complicated (molecular) statements out of simpler (atomic or molecular) ones using logical connectives.

P ^  Q is true when both P and Q are true (conjunction)

P v  Q is true when P or Q or both are true (disjunction)

P -> Q is true when P is false or Q is true of both (implication or conditional)

P<-> Q is true when P and Q are both true or both false (biconditional)

P is read "not P" and called a negation (negation)> We loved with a love that was more than love



**Problem 3**

Suppose P and Q are the statements: P: Jack passed math. Q: Jill passed math.

a. Translate “Jack and Jill both passed math” into symbols.

b. Translate “If Jack passed math, then Jill did not” into symbols.

c. Translate “P V Q” into English.

d. Translate “” into English.

e. Suppose you know that if Jack passed math, then so did Jill. What can you conclude if you know that:

i.  Jill passed math?

ii. Jill did not pass math?

**Solution to problem 3**

a. The answer is "P ^ Q" because both Jack and Jill passed math and this means that this is conjunction since both P and Q are both true statements

b. The answer is "P -> ¬Q" because since it is an if statement meaning that if one of the conditions is met then the outcome becomes true. In the statement If jack passed math, then Jill did not in symbol form it has to be P -> ¬Q meaning If P then Q has to be false.

c. The answer is "either Jack passed the math class or jill passed the math class or both" because P V Q statement means that it is a logical "or" statement which is a disjunction. If a statement is P V Q that means either P or Q or both of them could be true statements.

d. The answer is "If Jack and Jill did not pass then kill did" this is because if jack and jill both passed math classes has been negated that means that only Q can be true.


e i. The answer is "Nothing" since the statement Jill passed math is just a statement and it doesn't question anything.

e ii. The answer is  "Jack did not pass math class" because the original statement stated that Jack passed math and Jill also passed math class. In this one, if Jill didn't pass math that should also mean that Jack did not pass math class as well.



**0.3 Sets**

For us, a set will simply be an unordered collection of objects. We need some notation to make talking about sets easier. This notation is usually called set builder notation. It tells us how to build a set by telling us precisely the condition elements must meet to gain access (the condition is the logical statement after the “:” symbol). Reading and comprehending sets written in this way takes practice. The set Z is the set of integers; positive and negative whole numbers.



The empty set is the set that contains no elements. "Ø"

The universe set is the set of all elements. "U"

The set of natural numbers. That is,N = {0,1,2,3..} . "N"

The set of integers. That is, Z={..,-2,-1,0,1,2,3,...} . "Z"

The set of rational numbers. "Q"

The set of real numbers. "R"

The power set of any set A is the set of all subsets of A "P(A)"

If we want to combine two sets to get the collection of objects that are in either set, then we can take the union of the two sets. The other common operation on sets is an intersection. Venn diagram displays sets as intersecting circles. We can shade the region we are talking about when we carry out an operation.

**Problem 11**

Find an example of sets A and B such that A n B = {3,5} and A u B = {2,3,5,7,8}


**Answer for problem 11**

The answer is A={2,3,5,7,8} and B={3,5}

This is because A U B means the Union of A and B which means that the elements in a set are from A or B or both. The possible elements in the set are {2,3,5,7,8} the only way for A n B = {3,5} to happen is when both 3 and 5 are present in both sets A and B. This means set B has to have the elements 3 and 5 and set A has to have every single number being 2,3,5,7 and 8.





**0.4 Functions**

A function is a rule that assigns each input exactly one output. We call the output the image of the input. The set of all inputs for a function is called the domain. The set of all allowable outputs is called the codomain. We would write f: X -> Y to describe a function with name f, domain X, and codomain Y. This does not tell us which function f is though. To define the function, we must describe the rule. This is often done by giving the formula to compute the output for any input. The set of natural numbers that output is called the range of the function.

For a function f: N -> N, a recursive definition consists of an initial condition together with a recurrence relation. The initial condition is the explicitly given value of f(0). The recurrence relation is a formula in terms of f(n+1)  (and f(_n_) possibly _n_ itself).

A surjection is a function for which every element of the codomain is in the range. How many of the functions?

An injection is a function f that maps distinct elements of its domain to distinct elements.

An injection bijections if a function f: X → Y satisfied the properties of surjective function (onto function) and injective function (one-to-one function).


**Problem 10**

Suppose f:N->N satisfies the recurrence f(n+1)=f(n)+3. Note that this is not enough information to define the function, since we don’t have an initial condition. For each of the initial conditions below, find the value of f(5).

a. f(0)=0
b. f(0)=1
c. f(0)=2
d. f(0)=100


**Answer for problem 10**

a. f(5)=15

This is because when f(0)=0 all you have to do is 3*5 to find f(5)

f(0)= 0

f(1)= f(0+1)=f(1)+3 = 3

f(2)= f(1+1)=f(2)+3 = 6

f(3)= f(2+1)=f(3)+3 = 9

f(4)= f(3+1)=f(4)+3 = 12

f(5)= f(4+1)=f(5)+3 = 15



b. f(5)=16

This is because when f(0)=1 all you have to do is (3*5)+1 to find f(5)

f(0)= 1

f(1)= f(0+1)=f(1)+3 = 4

f(2)= f(1+1)=f(2)+3 = 7

f(3)= f(2+1)=f(3)+3 = 10

f(4)= f(3+1)=f(4)+3 = 13

f(5)= f(4+1)=f(5)+3 = 16

c. f(5)=17

This is because when f(0)=2 all you have to do is (3*5)+2 to find f(5)

f(0)= 2

f(1)= f(0+1)=f(1)+3 = 5

f(2)= f(1+1)=f(2)+3 = 8

f(3)= f(2+1)=f(3)+3 = 11

f(4)= f(3+1)=f(4)+3 = 14

f(5)= f(4+1)=f(5)+3 = 17

d. f(5)=115

This is because when f(0)=100 all you have to do is (3*5)+100 to find f(5)

f(0)= 100

f(1)= f(0+1)=f(1)+3 = 103

f(2)= f(1+1)=f(2)+3 = 106

f(3)= f(2+1)=f(3)+3 = 109

f(4)= f(3+1)=f(4)+3 = 112

f(5)= f(4+1)=f(5)+3 = 115


