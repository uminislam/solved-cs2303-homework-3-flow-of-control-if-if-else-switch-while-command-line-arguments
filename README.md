Download Link: https://assignmentchef.com/product/solved-cs2303-homework-3-flow-of-control-if-if-else-switch-while-command-line-arguments
<br>
<span class="kksr-muted">Rate this product</span>




flow of control: if, if-else, switch, while, command line arguments

Abstract

The objective is to give you practice with the statements by which we control the flow of execution, and allow data to modify the flow of execution. We will also navigate through a graph data structure. User input will be collected and used.

The context of this problem is carrying out a hunt for treasure in a “house” that is represented by a graph. The program will accumulate treasure, and keep track of how much is found in what place. The program will accept user input to customize the search process.

Be sure to construct test cases for each function you build. Put thought into the test cases. The goal is to know that a function works, when it passes all of its test cases. One test case per function is usually not enough.

<ul>

 <li>Construct a sequence diagram for your project. You can draw it by hand and include a phone/photo, or draw it with a software tool.</li>

 <li>Use the test-driven development style for developing your code. Docu- ment this by taking a new screen shot of your test code every time you make a new test (See Figure 1.), and of your production code every time you extend your production code. It could be a large number of screen shots. Be sure to run your code every time you add a few lines of test or production code. (See Figures 2 and 3.) Do not allow the number of errors to get large.</li>

 <li>An explanation of a representation of a graph will be given here, because a graph data structure will be used to represent the layout of the house. The program must use this data structure to present to the user the choices of next rooms to search. The representation is called an adjacency matrix. It is a two dimensional matrix. The number of rows and the number of columns are both set to be the number of nodes in the graph. In our case, it is the number of rooms in the treasure house. The values in the matrix come from whether the room number that is the row number is directly connected to the room number that is the column number. Because these direct connections are bidirectional, the adjacency matrix is symmetric about its main diagonal. Moreover, the values in the main diagonal are1</li>

</ul>

Figure 1: In the process of creating a new test.

Figure 2: Starting some production code.

Figure 3: Adding more production code.

2

Figure 4: The matrix on the left represents the floor plan on the right. The front door opens into room 1. Room 1 connects to rooms 2 and to 3, but room three does not connect with room 2.

all ones, because every room is directly reachable from itself. If the value in the matrix is not one, it is zero. You can use boolean or integer for the datatype of the array representing the adjacency matrix. We can add one more row and column to the graph to represent the front door, or, equivalently, the outside world if you prefer. Make functions for working with this data representation. For example, if the searcher is in room x, the searcher might wish to know which are the adjacent rooms.

<ul>

 <li>The searcher looks for treasure, and accumulates it. The goal is to max- imize the treasure found. Functions supporting this include finding out how much treasure has been accumulated, and adding the amount of a newly found treasure.</li>

 <li>Whether a room has been searched yet, or not, is a useful idea. Make a data structure to record this information. Don’t forget to initialize this so that no room has been searched. If you include the outside world as a room, it has already been searched.</li>

 <li>Print the rooms that have been searched, and the treasure subtotals, as they are accumulated.</li>

 <li>The program must enable the user to specify two limits: an amount of treasure and a number of rooms. If the subtotal of treasure is greater than or equal to the limit, the searcher must exit the house without picking up any more treasure. If the number of rooms searched equals the limit, the searcher must exit the house without picking up any more treasure. One or both of these two values can be entered on the command line. If fewer than two entries appear on the command line, the program must query the user for these values.Things to do: 1. Either:(a) Make a C project from the Hello,World project.(b) Populate that project with tests.c, tests.h, production.c and produc- tion .h.</li>

</ul>

or use the starter code.

3

<ol start="2">

 <li>Create the sequence diagram and include the electronic file (diagram, screenshot or photo). Make sure your name appears within the sequence diagram.</li>

 <li>Place function prototypes for all of your functions from the sequence dia- gram into one or more .h files.</li>

 <li>As you work on the assignment, collect a sequence of screen shots showing how your test code, and your production code are growing.</li>

 <li>Be sure to build and run often; do not allow errors to build up.</li>

 <li>Show the sequence of moves from room to room by listing them, and also show the subtotal of treasure through the house.</li>

 <li>Receive the values entered on the command line. Ask for values not pro- vided in the command line. In either case, check for reasonable values. Negative treasure or rooms implies no search should be conducted. Use these limit values in execution.</li>

</ol>