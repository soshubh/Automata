# Automata - Shubhanshu Singh

1.  Proof Techniques
    1. Direct Proof or Proof by Construction
    2. Proof by Contradiction
    3. Proof by Induction
    4. Proof by contrapositive
2. Set Theory
3. Sequence & Tuple
4. Graph Theory
    1. Graph
    2. Sub Graph
    3. Simple Graph
    4. Multiple Graph

## **Proof Techniques**

In computer science, proof techniques are methods and approaches that are used to prove the correctness of algorithms and other logical statements.

### **Direct Proof or Proof by Construction**

Method of proof that involves directly showing that a statement is true, using logic and reasoning.

*Theorem: If a and b are two even positive integers, then a*b is always even.*

***Proof:***

*Let a and b be two even positive integers.*

*By definition, an even number is a number that can be expressed in the form 2k .*

*Therefore, we can write:*

*a = 2x
b = 2y*

*for some integers x and y.*

*Multiplying a and b, we get:*

*ab = (2x)(2y)
= 4xy = 2(2xy)*

*This is an expression for an even number, because the coefficient of the term xy is even.*

*Therefore, a*b is always even.*

*QED*

---

*Theorem: If a is an odd integer and b is an even integer, then a*b is always an even integer.*

***Proof:***

*Let a be an odd integer, and let b be an even integer.*

*By definition, an odd integer is a number that can be expressed in the form 2x + 1 for some integer x. Therefore, we can write:*

*a = 2x + 1*

*for some integer x.*

*By definition, an even integer is a number that can be expressed in the form 2y for some integer y. Therefore, we can write:*

*b = 2y*

*for some integer y.*

*Multiplying a and b, we get:*

*ab = (2x + 1)(2y)
= 4xy + 2y =2(2xy+y)*

*This is an expression for an even integer, because the coefficient of the term 2m is even.*

*Therefore, a*b is always an even integer.*

*QED*

### **Proof by Contradiction or Indirect Proof**

Proof by contradiction is a method of proof that involves assuming that the statement being proved is false, and then showing that this leads to a logical contradiction.

*Theorem: The square root of 2 is an irrational number.

**Proof:**

Suppose, for the sake of contradiction, that the square root of 2 is a rational number. This means that it can be expressed as the ratio of two integers p and q, where q is not equal to 0 and HCF (p, q) =1.*

 *We can write this as:*

*√2 = p/q

Squaring both sides of this equation, we get:

2 = (p/q)² = p²/q²*

2q²=p²——— (i)

 here, p² is even that mean p is even

then p = 2x

put in equation (i)

2q²= 4x

q² = 2x 

q² is even then , q is even

*Since p and q are  even number so there HCF(p, q)!=1.*

*Therefore, our assumption that √2 is a rational number must be false. This means that √2 is an irrational number.

QED*

---

*Theorem: The square root of 3 is an irrational number.*

### Proof by Induction

Proof by induction is a method of proof that is used to establish that a given statement is true for all positive integers n. It involves showing that the statement is true for the base case n = 1, and then using the assumption that the statement is true for some arbitrary positive integer k to show that it is also true for k + 1.

*Theorem: For all positive integers n, 1 + 2 + 3 + ... + n = n(n+1)/2.

**Proof:**

Base case: We will show that the statement is true for*

 *n = 1 —    1 = 1(1+1)/2* 

                  1 = 1
*n = 2 —    1+2 = 2( 2+1)2*

                   3 = 3

then 

n = k 

 1+2+3+4+….+k = k(k+1)/2

n = k+1

  1+2+3+4+….+k+(k+1) = k(k+1)/2 + (k+1) 

         (k+1)(k+1+1)/2= (k+1)((k+1)+1)

*This is the expression for the sum 1 + 2 + 3 + ... + (k+1).

Therefore, we have shown that if the statement is true for some positive integer k, then it is also true for k + 1.

Since the statement is true for the base case n = 1, and we have shown that if it is true for some positive integer k, then it is also true for k + 1, we can conclude by induction that the statement is true for all positive integers n.

QED*

---

*Theorem: For all positive integers n, 5 + 10 + 15 + ... + 5n = 5n(n+1)/2.*

## Basic of Graph Theory

G = ( V, E)

**Loop :** it is a path that begins and ends at the same edge.

 

![photo_2023-01-10_00-20-23.jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-10_00-20-23.jpg)

---

**Parallel edges :** Parallel edges are two or more edges that connect the same two vertices.

![photo_2023-01-10_00-20-28.jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-10_00-20-28.jpg)

---

**Degree of vertex [deg(v)] :** Degree of a vertex is a measure of the number of edges incident to it, or connected to it.

![photo_2023-01-10_00-20-33.jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-10_00-20-33.jpg)

---

**Indegree [deg-(v)] :** Indegree of a vertex is the number of edges pointing towards it.

Indegree of vertex v1 is 2

deg-(v1) = 2

deg-(v2)= 1

![photo_2023-01-10_00-20-38.jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-10_00-20-38.jpg)

---

**Outdegree [deg+(v)] :** Outdegree of a vertex is the number of edges pointing away from it.

Outdegree of vertex v1 is 1

deg+(v1) = 1

deg+(v2)= 1

![photo_2023-01-10_00-20-38.jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-10_00-20-38%201.jpg)

---

**In Undirected graph** :
$Σd(v) = 2 * E$

---

**In Directed graph** :
$Σindegree(v)=Σoutdegree(v) = E$

---

**Isolated Vertex :** If the degree of a vertex is 0, the vertex is an isolated vertex and is not connected to any other vertices.

deg(v)= 0

---

**Pendent Vertex :**  

deg(V) = 1

![photo_2023-01-10_00-20-41.jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-10_00-20-41.jpg)

---

**Simple Graph :** No loop / No multiple edge.

**Multiple Graph :** Which have atleast  one mutli or parallel edge.

---

**Distance b/w two vertices :** Minimum number of edges that must be traversed to go from one vertex to the other.

$d(v1, v4) = 2$ 

![photo_2023-01-09_22-12-14 (1).jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-09_22-12-14_(1).jpg)

---

**Eccentricity of vertex :** The eccentricity of a vertex v, denoted as e(v), is defined as the maximum distance from v to any other vertex in the graph.

$e(v2) :$

$d(v2, v1) = 1$

$d(v2, v3) = 1$

$d(v2, v4) = 2$

$d(v2, v5) = 2$

$d(v2, v6) = 2$

$d(v2, v7) = 1$

$d(v2, v8) = 2$

$`d(v2, v9) = 3`$ **

![photo_2023-01-09_22-12-14 (1).jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-09_22-12-14_(1).jpg)

$e(v2) = 3$

---

**Radius of Graph :** Radius of a graph is a measure of the centrality of the graph. It is defined as the ***minimum eccentricity*** of any vertex in the graph. r(G)

$**r(G) = 1**$

$e(v1) :$

$d(v1, v2) = 1$

$d(v1, v3) = 2$

$d(v1, v4) = 2$

$d(v1, v5) = 1$

$d(v1, v6) = 1$

$d(v1, v7) = 2$

$d(v1, v8) = 3$

$d(v1, v9) = 2$

![photo_2023-01-09_22-12-14 (1).jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-09_22-12-14_(1).jpg)

In this case, the minimum distance is 1, which occurs for the distances from v1 to v2, v5, and v6. Therefore, the radius of the graph is 1. r(G) = 1

> Note : that the radius of a graph is the minimum eccentricity of any vertex in the graph, not just the minimum distance from a particular vertex (v1 in this case). To find the eccentricity of each vertex, you would need to find the maximum distance from that vertex to any other vertex in the graph.
> 

---

`*`**Diameter of Graph :** The diameter of a graph is a measure of the centrality and the spread of the graph. It is defined as the ***maximum eccentricity*** of any vertex in the graph. D(G)

$**D(G) = 5**$

$r(G) = 3$ ——— Radius

 $D(G) = 5$ ——— Diameter

---

**Center Point :** The center of a graph is the set of vertices with the minimum eccentricity. 

or 

 Center Point or $CP ={v2,v7}$

Center of The Graph : ${v2,v7}$

 e(Vi) = r(G)

---

**Girth of a Graph :** The girth of a graph is the ***length of the shortest cycle*** (a path that starts and ends at the same vertex) in the graph. The girth of a graph, denoted as g(G), is defined as the minimum length of any cycle in the graph.

$v6,v7,v8,v9,v6 = 4$

![photo_2023-01-09_23-17-35.jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-09_23-17-35.jpg)

---

`*`**Circumference of Graph :** The circumference of a graph is the ***length of the longest cycle*** (a path that starts and ends at the same vertex) in the graph. The circumference of a graph, denoted as C(G), is defined as the maximum length of any cycle in the graph.

$v1,v2,v7,v6,v9,v8,v4,v5,v1 = 8$

![photo_2023-01-09_23-17-35.jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-09_23-17-35.jpg)

### Type of Graph

1. **Finite Graph** 
    
     $e,v - Finite$ 
    
    ---
    
2. **Infinite Graph**
    
     $e,v - Infinite$ 
    
    ---
    
3. **Trivial Graph**
    
     Only one vertex
    
    ---
    
4. **Simple Graph** 
    
    No loop
    
    No multiple edges
    
    ---
    
5. **Multi Graph**
    
    Which have atleast  one multi or parallel edges 
    
    ---
    
6. **Null Graph**
    
    A null graph is **a graph in which there are no edges between its vertices.** A null graph is also called empty graph. 
    
    ---
    
7. **Complete Graph**
    
    a complete graph is a graph in which every pair of distinct vertices is connected by an edge. A complete graph with n vertices is denoted as Kn.
    
    ![photo_2023-01-09_23-46-56.jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-09_23-46-56.jpg)
    
    ---
    
8. **Regular Graph**
    
    Regular graph is a graph in which all the vertices have the same degree (i.e., the same number of edges).
    
    K - regular graph
    
    deg(vi) = K
    
    ![photo_2023-01-09_23-46-51.jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-09_23-46-51.jpg)
    
    This graph is **2-regular graph**
    
    ---
    
9. **Bipartite Graph**
    
    Bipartite graph is a graph whose vertices can be divided into two disjoint sets such that every edge in the graph connects a vertex in one set to a vertex in the other set.
    
    ![photo_2023-01-10_00-03-40.jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-10_00-03-40.jpg)
    
    ---
    
10. **Complete Bipartite Graph**
    
    A complete bipartite graph is a bipartite graph in which every vertex in one set is connected to every vertex in the other set.
    
    ![photo_2023-01-10_00-03-36.jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-10_00-03-36.jpg)
    
    ---
    
11. **Star Graph**

![photo_2023-01-10_00-03-31.jpg](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/photo_2023-01-10_00-03-31.jpg)

---

### **Question**

**Case I :** Distance between two vertexes(Vi) is same

Q :  We have 11 villages and have to place 3 shops in between them. Find the locations of the villages where you can place the shops.

![graph.png](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/graph.png)

Eccentricity e(Vi)

e(1) = 4  D(1 to 9)

e(2) = 3  D(2 to 9)

e(3) = 3  D(3 to 7)

e(4) = 3  

e(5) = 3  

e(6) = 4  

e(7) = 4 

e(8) = 4  

e(9) = 4  

e(10) = 4  

e(11) = 3 

For 3 shops we can choose any 3 from 

**`{2,3,4,5,11}`**

---

**Case II :** Distance between two vertexes(Vi) is not same

Q :  We have 11 villages and have to place 3 shops in between them. Find the locations of the villages where you can place the shops.

![graph (1).png](./Automata%20-%20Shubhanshu%20Singh%2035bd5948ace841edaaa43970a0a9843c/graph_(1).png)

$e(1) = 10$

d(1, 2) = 2

d(1, 3) = 5

d(1, 4) = 7

d(1, 5) = 3

d(1, 6) = 2

d(1, 7) = 1

d(1, 8) = 7

d(1, 9) = 8

`d(1,10)=10`

d(1, 11) = 2

$e(2) = 8$

d(2, 1) = 2

d(2, 3) = 3

d(2, 4) = 5

d(2, 5) = 4

d(2, 6) = 4

d(2, 7) = 3

d(2, 8) = 5

d(2, 9) = 6

`d(2,10)=8`

d(2, 11) = 3

$e(3) = 7$

d(3, 1) = 5

d(3, 2) = 3

d(3, 4) = 2

`d(3,5)=7`

`d(3,6)=7`

d(3, 7) = 6

d(3, 8) = 2

d(3, 9) = 3

d(3, 10) = 5

d(3, 11) = 6

$e(4) = 9$

$e(5) = 8$

$e(6) = 11$

$e(7) = 10$

$e(8) = 9$

$e(9) = 10$

$e(10) = 11$

$e(11) = 9$

For 3 shops we can choose 

**`{2,3,5}`**

Q : Put a village (v=12) in case I and case II 

## Formal language theory

**Symbol :** A symbol is a basic unit of a language.

**Alphabet :** Finite set of symbols. Ex : Σ= {0,1} 

**String :** Sequences of symbols drown from alphabet (finite length).

- **Language :** Collection of string drown from alphabet.
    
    ***Finite :** A finite language is a language that contains a finite number of strings.*
    
     *For example, the set of all strings that are made up of the letters 'a' and 'b' and have a length of less than 5 is a finite language.*
    
    ***Infinite :** A infinite language is a language that contains an infinite number of strings.*
    
    *For example, the set of all strings that are made up of the letters 'a' and 'b' is an infinite language. The set of all strings that starts with 'a' and ends with 'b' is also an infinite language.*
    
    ---
    
    Σ = {0,1} 
    
    L = { aⁿ bⁿ | n>0 and n≤2 }
    
    L = { ab,a²b² }
    
     a² = a.a = aa
    
    ---
    
    a* = Repetition of a, 0 or more time.
    
     ex : { a⁰ , a¹ , a² , a³ , a⁴ , ……….. }
    
      a⁰  = **λ (Empty String)**
    
    a⁺ = Repetition of a, 1 or more time.
    
     ex : { a¹ , a² , a³ , a⁴ , ……….. }
    
    ---
    
- **Prefix :**
    
    Prefix is any string that will obtain after removing *0 and more character from end* of string.
    
    S  = abcabca
    
    Prefix  :
    
    abcabca  -  0 char remove
    
    λ  -   7 char remove
    
    abcabc - 1 char remove 
    
    abcab - 2 char remove 
    
    abca - 3 char remove
    
    abc - 4 char remove 
    
      
    
- **Suffix  :**
    
    Suffix is the string that will be obtain after removing *0 or more character from front* of the string
    
    S  = abcabca
    
    Suffix :
    
    abcabca  -  0 char remove
    
    λ  -   7 char remove
    
    bcabca - 1 char remove 
    
    cabca - 2 char remove 
    
    abca - 3 char remove
    
    bca - 4 char remove 
    
      
    

**Proper Prefix or Suffix :** All the prefix and suffix excluding { abcabca, λ }

**Substring :**  Removing 0 or more character form beginning or from end.

- **Question :**
    
    Σ = {a, b}
    
    **Q - 1 : Define a long which that container exactly 2 a’s.**
    
    L = { bⁿ a bⁿ a bⁿ }
    
    **Q - 2 : Prefix will be aba always.**
    
    L = { aba (a + b)ⁿ | n≥0 }
    
    **Q - 3 : Start with ‘a’ an with ‘b’.**
    
    L = { a (a + b)ⁿ b | n≥0 }
    
- **Example :**
    
    w = 1010001
    
    wᴿ = 1000101
    
    Σ = {0, 1}
    
    Σ* = { λ, 0 , 1, 00, 01, 10, 11, ……}
    
    Σ⁺ = Σ* - λ
    
    ---
    
    L = { 0ⁿ 1ⁿ | n≥0 }
    
    L = { λ, 01, 0011, 000111, 00001111, ……..}
    
    L’ = Σ* - L
    
    Lᴿ = { 1ⁿ 0ⁿ | n≥0 }
    
    L* = { λ, 0ⁿ1ⁿ, 0ⁿ1ⁿ0ⁿ1ⁿ, 0ⁿ1ⁿ0ⁿ1ⁿ0ⁿ1ⁿ, ……..}
    
    ---
    
    Σ = { a, b }
    
    L₁ = { aⁿ bⁿ cⁿ | n≥1 }
    
    L₂ = { aᵐ bᵐ | m>0 }
    
    L₁ U L₂ = { aⁿ bⁿ cⁿ U aᵐ bᵐ | n≥0 & m>0 }
    
    L₁ U L₂ = { λ, abc, aabbcc, .…., ab, aabb, aaabbb, .…..}
    
    L₁ **∩** L₂ = λ
    
    L₁ . L₂ = { aⁿ bⁿ cⁿ aᵐ bᵐ | n≥1 & m≥0 }
    
    ---
    

## Grammar

$G = < T, V, S, P >$

- T is a finite set of terminals, which are the basic symbols of the language.
- V is a finite set of non-terminals, which represent the variables or syntactic categories of the language.
- S is the start symbol, which is a non-terminal that represents the beginning of the derivation process.
- P is a finite set of production rules, which specify how strings in the language can be constructed by replacing non-terminals with strings of terminals and non-terminals.

---

Capital Symbols = V (non-terminals)

Σ (Small Symbols)  = T (terminals)

Start Symbol = S

A → aAb / λ

V = { A }

T = { a, b }

S = { A }

- **Types of Grammars :**
    
    There are different types of grammars, each with their own set of rules and capabilities:
    
    1. Regular Grammar
    2. Context-Free Grammar
    3. Context-Sensitive Grammar
    4. Unrestricted Grammar
- **Example :**
    
    
    L = { a }
    
    Σ = { a }
    
    S → a
    
    S = S 
    
     T = { a }
    
     V = { S  } 
    
    L = { aa }
    
    S → aa
    
    S = S
    
    T = { a }
    
    V = { S }
    
    or 
    
    S → aB
    
    B → a
    
    tS= { S }
    
    T = { a }
    
    V = { S, B }
    
    ---
    
    **1 :** 
    
    L = { aⁿ | n>0 }
    
    L = { a, aa, aaa, aaaa, .... }
    
    S → aS / a
    
    T = { a }
    
    V = { S }
    
    S = { S }
    
    ---
    
    **4 :**
    
    L = { aⁿ bᵐ  | n,m≥0 }
    
    S → AB
    
    A → aA /  a
    
    B → bB / b
    
    T= { a, b }
    
    V = { S, A, B}
    
    S = { S }
    
    ---
    
    **2 :**
    
    L = { aⁿ | n≥0 }
    
    L = { λ, a, aa, aaa, aaaa,...}
    
    S → aS / Φ
    
    T = { a}
    
    V = { S }
    
    S = { S }
    
    ---
    
    **5 :**
    
    L = { aⁿ bᵐ  | n≥2, m>3 }
    
    S → AB
    
    A → aA / aa
    
    B → bB / bbb
    
    T = { a, b }
    
    V = { S, A, B}
    
    S= { S }
    
    ---
    
    **3 :**
    
    L = { aⁿ | n≥k }
    
    let k = 3
    
    S → Sa / aaa
    
    T = { a }
    
    V = { S }
    
    S = { S }
    
    ---
    
    **6 :**
    
    L = { aⁿ bⁿ  | n>0 }
    
     S → aSb / ab
    
    T = { a, b }
    
    V = { S }
    
    S = { S }
    
    **7 :** L = { aⁿ bⁿ  | n≥0 }
    
     S → aSb / Φ
    
- **Question :**
    
    **Q : Write a language that contains all the strings over the alphabet {a,b} such that the strings have exactly 2 b’s.**
    
    Σ = { a, b }
    
    L = { aⁿ b aⁿ b aⁿ | n≥0 }
    
    S → AbAbA
    
    A → aA / Φ
    
    S = { S }
    
    T = { a, b }
    
    V = { S, A }
    
    ---
    
    **Q : It starting start with a and end with b or start with b and end with a.**
    
    L = { a(a+b)b U b(a+b)a}
    
    S → aAb/bAa
    
    A → aA | bA | ε
    
    S = { S }
    
    T = { a, b }
    
    V = { S, A }
    
    ---
