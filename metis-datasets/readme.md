#METIS GRAPH Files

**METIS_GRAPH** is a data directory which contains examples of "graph" files used by the METIS program.

**METIS** can read a graph file, and partition the nodes in a balanced way so that each partition has about the same number of nodes, and the number of cut edges is minimized. This process is designed with the idea that the graph represents a computation that is to be divided up among various processors, with the stipulation that the amount of interprocessor communication must be limited.

##METIS GRAPH File Characteristics:
* ASCII
* a graph of N nodes is stored in a file of N+1 lines;
* the first line lists the number of nodes and the number of edges;
* If the first line contains more than two values, the extra values indicate the weights;
* each subsequent line lists the "neighbors" of a node;
* comment lines begin with a "%" sign;

###Licensing:
The computer code and data files described and made available on this web page are distributed under the GNU LGPL license.

###Reference:
1. George Karypis and Vipin Kumar, METIS, a Software Package for Partitioning Unstructured Graphs and Computing Fill-Reduced Orderings of Sparse Matrices;
2. George Karypis, Vipin Kumar,
A fast and high quality multilevel scheme for partitioning irregular graphs,
SIAM Journal on Scientific Computing,
Volume 20, Number 1, 1998, pages 359-392;
3. <http://www.cs.umn.edu/~metis>, The METIS home page;

###Sample Files:
* 4elt.graph, a "small" graph representing a 2D finite element mesh (15,606 nodes and 45,878 edges);
* test.mgraph, a "very small" graph that includes two vertex weights (766 nodes and 1,314 edges);
* tiny_01.graph, a "tiny" graph that includes no weights (7 nodes and 11 edges);
* tiny_02.graph, a "tiny" graph that includes edge weights (7 nodes and 11 edges);
* tiny_03.graph, a "tiny" graph that includes vertex and edge weights (7 nodes and 11 edges);
* tiny_04.graph, a "tiny" graph that includes three sets of vertex weights (7 nodes and 11 edges);

