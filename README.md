# Barabasi-Albert algorithm

##  About
The **Barabási–Albert (BA) model** is an algorithm for generating random scale-free networks using a preferential attachment mechanism. Several natural and human-made systems, including the Internet , the world wide web, citation networks, and some social networks are thought to be approximately scale-free and certainly contain few nodes (called hubs) with unusually high degree as compared to the other nodes of the network. (Wikipedia)
##  Algorithm
The network begins with an initial connected network of  $m_0$ nodes.

New nodes are added to the network one at a time. Each new node is connected to  ${\displaystyle m\leq m_{0}}$  existing nodes with a probability that is proportional to the number of links that the existing nodes already have. Formally, the probability  ${\displaystyle p_{i}}$  that the new node is connected to node  ${\displaystyle i}$  is

${\displaystyle p_{i}={\frac {k_{i}}{\sum _{j}k_{j}}},}$

where ${\displaystyle k_{i}}$ is the degree of node ${\displaystyle i}$ and the sum is made over all pre-existing nodes ${\displaystyle j}$ (i.e. the denominator results in twice the current number of edges in the network). (Wikipedia)