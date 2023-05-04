Download Link: https://assignmentchef.com/product/solved-csci-2270-homework9-implement-graph-traversal-for-cities
<br>
<strong><u>Overview</u></strong>

In this assignment, you will apply DF traversal for finding connected cities in a graph and find the shortest path using Dijkstra’s algorithm.

<strong><u>Graph Class</u></strong>

Your code should implement graph traversal for cities. A header file that lays out this graph can be found in ​<strong>Graph.hpp</strong>​ on Moodle. ​<em>As usual, do not modify the header file. You may implement helper functions in your .cpp file if you want as long as you don’t add those functions to the Graph class. </em>

Your graph will utilize the following struct:

<table width="640">

 <tbody>

  <tr>

   <td width="640"><strong>struct</strong>​ ​<strong>vertex</strong>​; <strong>struct</strong>​ ​<strong>adjVertex</strong>​{     vertex *v;};<strong>struct</strong>​ ​<strong>vertex</strong>​{     vertex() {this-&gt;visited = false;         this-&gt;distance = 0;         this-&gt;pred = NULL;}string name;     bool visited;     int distance;     vertex *pred;vector&lt;adjVertex&gt; adj; };</td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong>void addVertex(string name); </strong>

<ul>

 <li>Use from the previous assignment.</li>

</ul>

<strong> </strong>

<strong>void addEdge(string v1, string v2, </strong><strong>int num</strong>​ ​<strong>); </strong>

<ul>

 <li>Make a connection between v1 and v2 (same as last assignment). <u>​</u><strong><u>Important</u></strong><u>​</u> point here is to ​<strong>add weights to the edges</strong>​. Each edge will have a corresponding weight attached to it. E.g. addEdge(“Aurora”, “Bloomington”,5);</li>

</ul>




<strong>void depthFirstTraversal(string sourceVertex): </strong>

<ul>

 <li>Use Depth first traversal (recursive) from sourceVertex to traverse the graph. Print the city name and corresponding distance from the sourceVertex. Format for printing:</li>

</ul>

<strong>// for printing the path found through DF Traversal (each node) </strong><strong>cout&lt;&lt; n-&gt;name &lt;&lt; </strong>​” –&gt; “​<strong>; </strong>

<strong>// print “Done” at the end when all the cities have been visited.</strong><strong> cout &lt;&lt; “</strong>​Done​<strong>“; </strong>

<strong>vertex* DijkstraAlgorithm(string start, string end): </strong>

<ul>

 <li>Use Dijkstra’s algorithm to find the shortest path in the graph from the start city to the end city.</li>

</ul>

<strong> </strong>

<strong>For example: </strong><u>​</u><a href="https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm"><strong>Dijkstra’s</strong></a><u>​</u> <strong>Shortest distance from Boulder (Bo) to Denver (De): 15</strong>

<strong>  </strong>

<strong>void shortestpath(string s1, string s2): </strong>

<ul>

 <li>You should print the shortest path found though the Dijkstra’s algorithm.</li>

</ul>

<strong>// for printing the shortest path </strong><strong>cout &lt;&lt; </strong>​<strong>path[i]-&gt;name </strong>​<strong>&lt;&lt; ” “; </strong>

<strong> </strong>

<strong> </strong>

<strong><u>Other cout statements:</u></strong>

cout&lt;&lt;“Depth First Traversal ” &lt;&lt;endl; cout&lt;&lt;endl;

cout&lt;&lt;“Dikstra’s Shortest distance from Aurora to Fruita: “&lt;&lt;vertex-&gt;distance&lt;&lt;endl; cout&lt;&lt;“Dikstra’s Shortest path from Aurora to Fruita: “&lt;&lt;endl;


