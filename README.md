# Glutamate-Plasticity-Molecular-Regulatory-Dynamics
Python program “The Glutamate Plasticity Dynamics” works on the dynamics and parameters calculation in 《Connecting the Dots: A Computational Framework linking Molecular Regulation, Synaptic Plasticity, and Brain Disorders》

# Instructions:
1，Please download the “The Glutamate Plasticity Dynamics.ipynb” for the simulation.  
2, Download all the network matrix files(.csv files) in the same file address with “The Glutamate Plasticity Dynamics.ipynb” to make sure the program can read all networks.  
3, Type in the networks' local file address in “The Glutamate Plasticity Dynamics.ipynb” for proper execution of the program.  

# Descriptions:
1, The Boolean dynamics is simulated on the simplified networks in the paper.  
2, In the main Python file, dynamics on the simplified network, dynamics of networks with node-knock-out and betweenness calculation are are executed sequentially to perform simulation operations.  
3, The simplified network and all networks after nodes knock-out in the paper are saved as “.csv” files，the file “nodes_interaction_G_named.xlsx” contains the simplified network with nodes names, the nodes sequence in the knock-out networks are the same as original one.  
4, The Boolean functions between nodes are redefined as linear operations based on the adjacency matrix combined with conditional judgment functions derived from Boolean logic. In the program, these operations are distinguished by the cal_type array:  
cal_type = 1 corresponds to the ​OR operation,  
cal_type = 2 represents the ​AND operation,  
The ​NOT operation is implemented via the ‘-1’ entry in the adjacency matrix.  
5.The results of all dynamics calculation are saved in the form of a four-column matrix, showing the evolution trajectory for each state. From left to the right are “source state”, “sink state”, “degree of source” and “states activation type”.The index is the decimal conversion of Boolean states in the node sequence. “states activation type=0” refers to Endo=0 and SNAREs=0; “states activation type=1” refers to Endo=1 and SNAREs=0; “states activation type=2” refers to Endo=0 and SNAREs=1; “states activation type=100” refers to Endo=1 and SNAREs=1.  
6.Visulization of the networks are using Cytoscape.  
   
# Author:
Ze-Zheng Li  
School of Systems Science, Beijing Normal University, Beijing, 100875, China
