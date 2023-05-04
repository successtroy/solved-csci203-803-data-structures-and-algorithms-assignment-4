Download Link: https://assignmentchef.com/product/solved-csci203-803-data-structures-and-algorithms-assignment-4
<br>
<h1>Objectives</h1>

 Design and implement a program to solve the Travelling Salesman Problem using a greedy algorithm based on nearest neighbours and a branch-and-bound algorithm;  Use appropriate data structures for different algorithms;  Analyse the results of different algorithms.




<h1>Task</h1>

You should write a single program which implements the greedy algorithm based on nearest neighbours and a branch-and-bound algorithm to find approximate and optimal solutions for the Travelling Salesman Problem, respectively.

<h1>Program</h1>

Your program should read a symmetric matrix from a text file that describes weighted edges of an undirected, complete graph and find the Hamiltonian cycles using the greedy and branch-and-bound algorithms. Your program should also read a list of city names corresponding to the vertices of the graph represented by the adjacency matrix. The program will display the tour and related information.

Since this assignment focuses on the algorithmic solution of the problem, STL or Java Collection or other collection framework of the programming language of your choice can be used. Library functions can also be used.

Your program should be readable and well commented.

<h1>Data Structures and Algorithms</h1>

<ul>

 <li>Greedy algorithm</li>

</ul>

Strategy: Nearest neighbour




<ul>

 <li>Branch-and-bound algorithm</li>

</ul>

Upper bound: weight by nearest neighbours Lower bound: minimal weight without constraints Strategies:

<ol>

 <li>Breadth-first;</li>

 <li>Depth-first.</li>

</ol>

Choose suitable data structures for the algorithms and strategies, to be described in your report.

<h1>Requirements</h1>

<strong> </strong>

<strong><u>CSCI203 students</u> (10 marks or 8, 6 or 4 marks) </strong>

<strong> </strong>

<ol>

 <li>Program</li>

</ol>

You have two choices on how to write your code.

<ul>

 <li>Implement the greedy algorithm and Branch-and-bound algorithm with a strategy of your choice; (3 and 5 marks, respectively)</li>

</ul>

or

<ul>

 <li>Integrate the greedy algorithm and/or Branch-and-bound algorithm with a strategy of your choice. In this case, you may use or adapt the code available in public domains.</li>

</ul>

Properly cite the sources of your code in your report and program.       (1 mark for each)




<ol start="2">

 <li>Report

  <ol>

   <li>Cover page</li>

  </ol></li>

</ol>

Student name

Subject code

Student number Email ID

(0 mark; your assignment will not be marked if there is not this section)




<ol>

 <li>Methods and result analysis (no more than 300 words)</li>

</ol>

Describe the algorithms, data structures and structure of your code. Analyse and discuss your results from two algorithms. State a conclusion about the algorithms and strategies.

(2 marks)




<strong><u>CSCI803 students</u> (10 marks) </strong>

<strong> </strong>

<ol>

 <li>Program</li>

</ol>

Implement the greedy algorithm and Branch-and-bound algorithm with two strategies.

(2, 3 and 3 marks, respectively)

<ol start="2">

 <li>Report</li>

 <li>Cover page</li>

</ol>

Student name

Subject code

Student number Email ID

(0 mark; your assignment will not be marked if there is not this section)




<ol>

 <li>Methods and result analysis (no more than 400 words)</li>

</ol>

Describe the algorithms, data structures and structure of your code. Analyse and discuss your results from the greedy algorithm and branch-and-bound algorithm and the number of nodes generated with two strategies. State a conclusion about the algorithms and strategies.

(2 marks)

<h1>Other requirements</h1>

<ul>

 <li>All your programs excluding a4compile and a4run scripts will have the following header:</li>

</ul>

/*

<ul>

 <li>CSCI203 or 803 Assignment 4</li>

</ul>

*

<ul>

 <li>Student name:</li>

 <li>Subject code:</li>

 <li>Student number:</li>

 <li>Email ID:</li>

</ul>

*

<ul>

 <li>(The following heading goes all places where appropriate if</li>

 <li>all or part of code in your program is not written by you.)</li>

 <li>Author:</li>

 <li>Sources: (citation of the sources)</li>

</ul>

*/

<ul>

 <li>Your programs can be compiled and executed with bash scripts called <strong>a4compile</strong> and <strong>a4run</strong>, respectively, on Ubuntu setup in the lab.

  <ul>

   <li>The script <strong>a4run</strong> should be configured to run for both input files (Australia_roads.txt and Australia_flights.txt) to produce all results.</li>

   <li>Failure to compile and run your program to produce all results from your scripts will receive 0 mark.</li>

  </ul></li>

 <li>Report, named <strong>pdf</strong>, is created in the PDF format.</li>

 <li>Failure to meet any requirements above may result in loss of marks.</li>

</ul>




<h1>Input</h1>

Your program will work with selected Australian cities and find tours to visit each and all of them once <em>starting from and returning to Wollongong</em> using the greedy and branch-and-bound algorithms

Your program should read <strong>two input file names</strong> from the <strong>command line</strong>. The first file contains the adjacency matrix and the second file the city names in the order of the vertex indices. The adjacency matrix in the input file has a format as follows.

<ul>

 <li>The integer number of vertices in the graph.</li>

 <li>The positive real number weights of one vertex per line, delimited by a tab. The value 0 or 0.0 is used for no connection.</li>

</ul>

The city names in the input file has a format as follows.

<ul>

 <li>Each city name in one line</li>

</ul>

The number of cities is the same as the number of vertices in the adjacency matrix.

Input files of two adjacency matrices are provided.

<ul>

 <li>txt: driving distances between cities</li>

 <li>txt: flight time between cities</li>

</ul>

Apparently some flight time in Australia_flights.txt is a fake.

And the input file of the city names corresponding to the adjacency matrices is also provided as Australia_cities.txt.

Your program should work with any input files of the same format. It may be tested with an adjacency matrix of a different size and different city names.

<h1>Output</h1>

Your program should display the results to the standard output. An example of the program output format for an adjacency matrix is shown as follows.

<table width="601">

 <tbody>

  <tr>

   <td width="601">1.  Greedy algorithm:Number of cities:  11Tour:1  2 6 … 9Wollongong -&gt; Sydney -&gt; Canberra -&gt; … -&gt; Perth -&gt; Wollongong    Total cost: 17637.0 2.  Branch-and-bound algorithm (Breadth-first):Number of cities:  11Upper bound:  17637.0    Lower bound:  9338.0Optimal tour:1  2 11 … 6Wollongong -&gt; Sydney -&gt; Gold Coast -&gt; … -&gt; Canberra -&gt; Wollongong    Total cost: 14988.0</td>

  </tr>

 </tbody>

</table>




In the result of the tour, the first line displays the vertex numbers (without the returning vertex) and the second line the city names (with returning city).

You should run your program for both adjacency matrices to produce tours for travelling by road and flight.

For CSCI203 students, your program should display one result of the branch-and-bound algorithm with a strategy of your choice.

For CSCI803 students, your program should display one more result of the branch-and-bound algorithm with another strategy, and the total number of nodes generated with each strategy.