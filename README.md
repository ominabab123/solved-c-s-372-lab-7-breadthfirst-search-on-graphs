Download Link: https://assignmentchef.com/product/solved-c-s-372-lab-7-breadthfirst-search-on-graphs
<br>









In this lab, you will implement the breadth­first search (BFS) algorithm using an iterative strategy and make sure it runs in linear time to the size of the input graph.

<h1>1        Requirement for the BFS algorithm</h1>

Design a linear­time BFS algorithm with the following function prototype void BFS( Graph &amp; G, Node &amp; s )

{

/ /     Input :      graph G,      which    can   be  e i t h e r     undirected      or       directed

/ /    Output :     the   e f f e c t   of   BFS  i s    that    a l l   nodes

/ /                       1.    are    marked    with    a    distance      label

/ /      perform BFS on      the    graph    from    a    given    node   s

}

The effect of the BFS on the graph <em>G </em>are distance labels indicating the distance from source node <em>s </em>to every node in the graph. In C++, you can generate a double type positive infinity by the function

std : : numeric_limits &lt;double &gt; : : i n f i n i t y ( )

The distances will be stored within the Graph data structure. You can enhance the graph class from previous labs in more than one way. You are free to design your strategy and describe it in your lab report. The distance values cannot be saved as global variables.

<h1>2        Iterative solution</h1>

You can use the std::queue class in C++ to hold the discovered but not yet processed nodes. The useful member functions of the class are push() to inject an object into the end of the queue, pop() to eject an element from the front of the queue, front(), and empty().

<h1>3        Test the classes</h1>

Generate five example graphs to test your code. The graphs do not have to be very large but must represent a variety: cyclic/acyclic, directed/undirected, having one or more connected components. You test your code against the precomputed distance values as the truth.

Your C++ program must include a main() function that calls the testall() function. When the program is compiled by a C++ compiler it generates a binary executable file that will run when invoked from the command line.

<h1>4        Plot the runtime as a function of number of nodes and edges</h1>

After testing the correctness of the the program, you will study how the runtime scales with the size of graph for your BFS implementation. Use the random graph generation function you developed in Lab 4 to produce large graphs in increasing sizes.

You will produce by R two curves of BFS runtime as a function of

<ol>

 <li>the number of nodes, given the number of edges</li>

 <li>the number of edges, given the number of nodes in the input graphs.</li>

</ol>

Your algorithm must be able to handle graphs with 10,000 or more nodes and 1,000,000 or more edges in the order of a few seconds.


