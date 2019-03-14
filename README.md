# Fault-Diagnosis
A Neural Network based inter turn Fault diagnosis of a Synchronous generator

Inter turn fault is the most commonly occurring fault in the synchronous machines used all over the world. It is basically a chain reaction where, adjacent turns in a coil in the machine could get shorted for various reasons like insulation wear off over time, excessive heat causing insulation failure.

Once a few turns get shorted, then like an avalanche the other turns in the machine would also get shorted resulting total break-down. And this down time in industries could lead to huge financial losses.

We can identify the fault using non linear kalman filters but to avoid the complex mathematical derivations, i decided to develop a neural network to identify the fault(classification-0/1). The data is obtained from the Ansys maxwell simulation software which is very similar to CAD or AutoDesk but solves magnetic fields using FEM(finite element method).Using that software we can get both healthy and faulty data.

The added csv file has data in the following format:

<p>first column of the csv represents the each time step of the total time the simulation was run</p>
<p>column 2 to 4 represents the 3 phase stator currents</p>
<p>column 5 to 6 represents the state of the generator(healthy/faulty) and if faulty, then the percentage of fault is represented by 6th column</p>

<p>columns 2 to 4 are the input while columns 5 and 6 represent the target labels</p>
<p>in column 5,</p><ul><li> 0 represents healthy state</li>
  <li>1 represents fault in phase A</li>
  <li>2 represents fault in phase B</li>
  <li>3 represents fault in phase C</li></ul>
  <p>in column 6,</p><ul><li> 4 represents 1.6% fault</li>
  <li>5 represents 3.33% fault</li>
  <li>6 represents 4% fault</li></ul>
<p>for the column 6th column as of now only 1.6% fault data has been added</p>
