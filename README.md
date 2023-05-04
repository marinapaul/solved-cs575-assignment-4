Download Link: https://assignmentchef.com/product/solved-cs575-assignment-4
<br>
Topics: Graph theory; Depth-first search, Breadth-first search, topological sorting, and linear programming.

<strong><u>[Part A] Theory : </u></strong>

<ol>

 <li>Explain how to determine whether or not an undirected graph is connected? And whether or not it is a tree? Using the following graph as an example to justify your answer.</li>

 <li> Does an undirected graph with 5 vertices, each of degree 3 exist? If yes draw the graph, otherwise explain why there is no such graph.</li>

 <li>Apply depth first search to the following graph. Show the graph after a new edge has been identified as a tree, forward, backward, or cross edge and indicate its type. Show also the current color of all the nodes. (NOTE: assume starting from node 1, and go to node 2 first).</li>

 <li> Apply topological sort to the graph below. Show the sequence of the nodes found by your application. Include also the discovery and finishing time of each node.  (Assume the starting node is 1, the second node to go is 7.  Also node 2 will be selected before node 4.)</li>

 <li>(11%) The <strong><em>square</em></strong> of a directed graph G(V, E) is the graph G<sup>2</sup> = (V, E<sup>2</sup>) such that (u, w) Î E<sup>2</sup> if and only if for some v Î V, both (u, v) Î E and (v, w) Î That is, G<sup>2</sup> contains an edge between u and w whenever G contains a path with exactly two edges between u and w. Describe an efficient algorithm for computing G<sup>2</sup> from G for the adjacency-matrix representation of G. Give the running time of your algorithm.</li>

</ol>




Hint:

Adjacency matrix in In G<sup>2:</sup>

A<sup>2</sup>[i, j] = 1 if (A[i, 1] =1 &amp;&amp; A[1, j] = 1) or (A[i, 2] =1 &amp;&amp; A[2, j] = 1) or… or (A[i, n] =1 &amp;&amp; A[n, j]=1)




Algorithm is defined in function CreateGsquare(A, n)

Input: Adjacency matrix A for graph G  (n = |V|)

Output: Adjacency matrix Asquare for graph G<sup>2</sup>










<ol>

 <li>[12%] A graph is said to be bipartite if all its vertices can be partitioned into two disjoint subsets X and Y so that every edge connects a vertex in X with a vertex in Y. (We can also say that a graph is bipartite if its vertices can be colored in two colors so that every edge has its vertices colored in different colors; such graphs are also called 2-colorable).</li>

</ol>




<ul>

 <li>(4%) Indicate whether graph (i) and (ii) are bipartite</li>

</ul>










<ol>

 <li>(4%) Design a DFS-based algorithm for checking whether a graph is bipartite.</li>

 <li>(4%) Design a BFS-based algorithm for checking whether a graph is bipartite.</li>

</ol>













<ol start="7">

 <li>[10%]</li>

</ol>




One can model a maze by having a vertex for a starting point, a finishing point, dead ends, and all the points in the maze where more than one path can be taken, and then connecting the vertices according to the paths in the maze.

<ol>

 <li>Construct such a graph for the following maze.</li>

 <li>Which traversal–DFS or BFS–would you use if you found yourself in a maze and why?</li>

</ol>










<ol start="8">

 <li>[10%] A merchant plans to manufacture two models of home computers at costs of $250 and $400, respectively. To sell the computers, the $250 model yields a profit of $45 and the $400 model yields a profit of $50. The merchant estimates that the total monthly demand will not exceed 250 units. Find the number of units of each model that should be stocked in order to maximize profit. Assume that the merchant does not want to invest more than $70,000 in computer inventory.</li>

</ol>







<ol start="9">

 <li>[10%] Using the Simplex Algorithm to solve the three variables linear programming problem</li>

</ol>

<table>

 <tbody>

  <tr>

   <td><strong>Maximize</strong></td>

   <td>P</td>

   <td>=</td>

   <td>20x<sub>1</sub></td>

   <td>+</td>

   <td>10x<sub>2</sub></td>

   <td>+</td>

   <td>15x<sub>3</sub></td>

   <td> </td>

   <td> </td>

  </tr>

  <tr>

   <td><strong>Subject to: </strong></td>

   <td> </td>

   <td> </td>

   <td>3x<sub>1</sub></td>

   <td>+</td>

   <td>2x<sub>2</sub></td>

   <td>+</td>

   <td>5x<sub>3</sub></td>

   <td>≤</td>

   <td>55</td>

  </tr>

  <tr>

   <td> </td>

   <td> </td>

   <td> </td>

   <td>2x<sub>1</sub></td>

   <td>+</td>

   <td>x<sub>2</sub></td>

   <td>+</td>

   <td>x<sub>3</sub></td>

   <td>≤</td>

   <td>26</td>

  </tr>

  <tr>

   <td> </td>

   <td> </td>

   <td> </td>

   <td>x<sub>1</sub></td>

   <td>+</td>

   <td>x<sub>2</sub></td>

   <td>+</td>

   <td>3x<sub>3</sub></td>

   <td>≤</td>

   <td>30</td>

  </tr>

  <tr>

   <td> </td>

   <td> </td>

   <td> </td>

   <td>5x<sub>1</sub></td>

   <td>+</td>

   <td>2x<sub>2</sub></td>

   <td>+</td>

   <td>4x<sub>3</sub></td>

   <td>≤</td>

   <td>57</td>

  </tr>

  <tr>

   <td> </td>

   <td> </td>

   <td> </td>

   <td>x<sub>1</sub></td>

   <td>,</td>

   <td>x<sub>2</sub></td>

   <td>,</td>

   <td>x<sub>3</sub></td>

   <td>≥</td>

   <td>0</td>

  </tr>

 </tbody>

</table>







Show the results through the pivot operations and linear program (show the table step by step by hand).







<strong><u>[Part B]: Graph Algorithm (20%)</u></strong>




<strong>B.1.</strong> (10%)

Suppose a CS curriculum consists of n courses, all of them mandatory. The prerequisite graph G has a node for each course, and an edge from course v to course w if and only if v is a prerequisite for w. Find and algorithm that works directly with this graph representation, and computes the minimum number of semesters necessary to complete the curriculum (Assume that a student can take any number of courses in one semester). The running time of your algorithm should be linear.




Using following example to justify your answer:

The CS Department requires fifteen one-semester courses with the prerequisites shown below:




cs1

cs2

cs3

cs4 requires cs2

cs5 requires cs4

cs6 requires cs1 and cs3

cs7 requires cs4

cs8 requires cs5 and cs6

cs9 requires cs7

cs10 requires cs9

cs11 requires cs8

cs12 requires cs3

cs13 requires cs6

cs14 requires cs4 and cs6

cs15 requires cs14




<em><u>Your task is to determine the minimum number of semesters needed to finish the degree. </u></em>







(Hint: Represent the courses and their prerequisites as a DAG. Finding the minimum number of semesters translates to a simple graph problem, e.g., Using adjacency-matrix representation in BFS).




<strong><u>Please provide: </u></strong>

<ol>

 <li>Manually plot the DAG (1%)</li>

 <li>Explain the algorithm that you are going to implement by the Pseudo-code, and indicate the minimum number of semesters necessary to finish the degree. (1%)</li>

 <li>Write and run your program to print out the result for verification (i.e., minimum number of semesters) (8%)</li>

</ol>




B.2. (10%)

In order to find the <em>connected components</em> or find out <em>whether there is a cycle</em> in graph (i) and (ii), you need to choose and use correct data structure of the graph representation for time and space efficiency.




<ul>

 <li>(2%) Indicate what data structure to represent (i) and (ii), respectively.</li>

</ul>




<ul>

 <li>(8%) Implement your algorithm of finding the connected components for (i) and (ii), and print out the connect components of (i) and (ii).</li>

 <li>(8%) Implement your algorithm of determining whether there is a cycle in (i) and (ii), and print out your finding by “yes” or “no”. (Extra 5 points: print out the cycle nodes in a correct order).</li>

</ul>

(Note: For (b) and (c), you can do one of them).







B.3. [Optional Extra point 10%]




To answer the Question #9 (Part A), implement the Simplex Algorithm and display the results by your program.


