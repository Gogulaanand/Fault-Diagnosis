# Fault-Diagnosis
A Neural Network based inter turn Fault diagnosis of a Synchronous generator

Inter turn fault is the most commonly occurring fault in the synchronous machines used all over the world. It is basically a chain reaction where, adjacent turns in a coil in the machine could get shorted for various reasons like insulation wear off over time, excessive heat causing insulation failure.

Once a few turns get shorted, then like an avalanche the other turns in the machine would also get shorted resulting total break-down. And this down time in industries could lead to huge financial losses.

We can identify the fault using non linear kalman filters but to avoid the complex mathematical derivations, i decided to develop a neural network to identify the fault(classification-0/1). The data is obtained from the Ansys maxwell simulation software which is very similar to CAD or AutoDesk but solves magnetic fields using FEM(finite element method).Using that software we can get both healthy and faulty data.
