# Circuit Solver

This is a web-based circuit simulator which imports a netlist as a text file (<a href="netlist.txt">netlist.txt</a> is a sample), solves the circuit, and displays a schematic diagram for the circuit.  
The nodes as mentioned in the netlist are shown as red circles. The voltage at a particular node is displayed when that node is clicked.

The circuit is solved using <a href="https://www.swarthmore.edu/NatSci/echeeve1/Ref/mna/MNA3.html">modified nodal analysis</a>. The circuit may only contain ideal, independent, constant current and voltage sources, and resistors. I hope to include more features soon. 

To run this circuit solver, download or copy-paste the contents of <a href="ckt_solver.html">ckt_solver.html</a>, save it with a .html extension, and open it in a web browser. You should see something like this-<br>
<center>
<img src="readme_imgs/on_opening.png" alt="drawing" width="320"/>
</center>

Click on Browse and import the text file containing the netlist. The contents of the file are displayed and a circuit diagram is displayed-<br>
<center>
<img src="readme_imgs/after_importing.png" alt="drawing" width="650"/>
</center>

Now simply click on the nodes and the voltages at those particular nodes will be displayed like so-
<center>
<img src="readme_imgs/after_clicking.png" alt="drawing" width="200"/>
</center>

___

The arrangements of nodes is done in a circular manner, clockwise. This was chosen so that the number of crossing-overs would be minimized. However, this does not work satisfactorily when the number of nodes are large. Any other general configuration of nodes, on the other hand, would lead to a mess in the centre. Some smart way of arranging the nodes which takes into account the number of components attached to each node would be an improvement. 
