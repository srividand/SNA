Social Network Analysis
Social Network Analysis is the study of social structures through the use of graph theory. In SNA, social networks are represented as graphs where nodes represent individuals, organizations, or other entities, and edges represent the relationships or interactions between them. SNA applies mathematical and computational tools to understand and analyze patterns of relationships in complex systems.

Key Concepts in SNA:

Nodes:
The individual entities or actors in the network, such as people, organizations, or events. For example, in a social network, nodes could represent users.

Edges:
The relationships or interactions between the nodes. These can represent a variety of connections such as friendships, communications, or collaborations. Edges can be directed (where the relationship has a direction, like following someone on Twitter) or undirected (where the relationship is mutual, like a friendship).

Degree of a Node:
The number of connections or edges that a node has. A node with a high degree is well-connected, whereas a node with low degree has fewer connections.

Cliques and Communities:
Cliques are subsets of nodes that are all connected to each other. Communities are larger groups of nodes that are more densely connected to each other than to nodes outside the group.

Path and Distance:
A path is a sequence of edges connecting two nodes, and distance is the length (number of edges) of the shortest path between two nodes. Shorter distances generally imply stronger relationships or closer proximity in the network.

Centrality:
Measures the importance of a node within the network. Common centrality measures include:
Degree centrality: The number of edges connected to a node.
Closeness centrality: How close a node is to all other nodes in the network.
Betweenness centrality: The number of times a node acts as a bridge along the shortest path between two other nodes.

PROBLEM STATEMENT: To track how the individuals communicate, how frequent people send emails and who they are sending. And to determine the volume of the communication between the people in a closed relationship and not so close relationship

Dataset used: Email txt data

Libraries imported: network nx, pandas, matplotlib and louvian community from jupyter notebook in anaconda.

The dataset contains text data and firstly after importing the data the main duties are to
Find the nodes, edges, density of network which shows how connected are people within network. Here nodes represent people and edges represent relationship between people.
Finding the node degree which determine how many other nodes are connected with each node. After plotting the histogram which is asymmetric distribution there are 1065 components.
Found out two components which has relationship only between that component and not others. By louvian community detection algorithm I detected 2 communities which are having high modularity.
By finding the 3 types of centrality of the components, we can determine which nodes can pass information more rapdily and which nodes are connected in a very close relationship. This is used to find who are emailing each other very frequently and who are not in a frequent relationship between the community.
