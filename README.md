# Graph Coloring: Sudoku Solver and Time Table Scheduling

       Su Doku is usually played on a 9 by 9 board, divided into 3 by 3 cells. You can generalize this into playing
on an M × M square board broken into non-overlapping rectangular cells, each containing M squares. The
solution of the puzzle is to place M symbols on the board such that each row, column or cell contains each
symbol exactly once, without moving the initial clues. Puzzles with M < 9 are called Sub Dokus, those for M
> 9 are called Super Dokus.

#History of Shi Doku
The name Shi Doku comes from Japanese and means ”four singles”. Shi Doku was invented on Wednesday
by someone who wanted a puzzle which could be solved while waiting for the lights to turn green. The puzzle
is set on a four by four board divided into non-overlapping two by two cells. The object is to place the symbols
”B” ”O” ”R” ”E” on the board so that each row, column or cell contains each symbol exactly once. The puzzle
starts with a set of symbols, called ”clues”, already placed on the board, which may not be moved.

#The Graph Coloring Problem
       A graph coloring is an assignment of labels, called colors, to the vertices of a graph such that no two adjacent
vertices share the same color. The chromatic number χ(G) of a graph G is the minimal number of colors for
which such an assignment is possible. Other types of colorings on graphs also exist, most notably edge colorings
that may be subject to various constraints.

       A graph G is called k-colorable if there exists a graph coloring on G with k colors. If a graph is k-
colorable, then it is n-colorable for any n > k. A graph has a chromatic number that is at least as large as the
chromatic number of any of its subgraphs. A graph has a chromatic number that is at most one larger than
the chromatic number of a subgraph containing only one less vertex. Graph Coloring is NP-Complete. We can
obtain approximate solutions and it has a lot of applications.

    • Mobile Radio Frequency Assignment When frequencies are assigned to towers, frequencies assigned
to all towers at the same location must be different. How to assign frequencies with this constraint? What
is the minimum number of frequencies needed?
    • Register Allocation In compiler optimization, register allocation is the process of assigning a large
number of target program variables onto a small number of CPU registers.
    • Map Coloring Geographical maps of countries or states where no two adjacent cities cannot be assigned
same color. Four colors are sufficient to color any map.

#Part A
we will write the pseudo-code for a basic greedy graph vertex coloring algorithm. Give its time complexity.

#Part B
NetworkX is a Python package for the creation, manipulation, and study of the structure, dynamics, and
functions of complex networks. With NetworkX you can load and store networks in standard and nonstandard
data formats, generate many types of random and classic networks, analyze network structure, build network
models, design new network algorithms, draw networks, and much more. We will use NetworkX for solving the greedy graph coloring problem. 

• Using NetworkX, we will make a graph for a Su Doku puzzle with no entries, and visualize it.
• I wrote a function greedy_graph_coloring(graph, colors) that takes two arguments - graph and
colors and returns . Given a graph G and k colors, we have to assign a color to each node in G such
that the adjacent nodes get different colors.
• We will go to Sudoku Puzzle Archive and choose the puzzle corresponding to your birthday in 2008. Formulate
the graph for difficulty of Easy, T ough and 16x16, assign colors and visualize all the three graphs. Now,
solve all the three puzzles using the function you have written.

#Part C
The greedy solution to solve the Duko problems can be transferred to find an optimal solution for schedul-
ing exams! We’ll provide you with a synthetic data set in csv format with students and the courses in which
they have enrolled. You have to prepare a schedule that prevents students from having colliding exam time slots.
