
# Introduction to Graph Theory 

## Introduction

Graph theory is the study of mathematical structures used to model pairwise relations between objects, otherwise known as graphs. Such a structure is made up of vertices, nodes, or points which are connected by edges, arcs, or lines. Network theory is a part of graph theory: a network can be defined as a graph in which nodes and/or edges have attributes (e.g. names). In this lesson we shall have a quick look at what this theory encompasses, what a graph looks like and also look at some real examples. 

## Objectives
* Understand and explain fundamental concepts and terminology used in graph theory
* Describe a graph with its constituent components including nodes and edges
* Understand different types of networks with respect to their formations

### So what is a graph 

Right let's quickly see some basic definitions ..

A "**Graph**" in mathematical and computer science terms consists of "**Nodes**" or "**Vertices**". Nodes/Vertices may or may not be connected with one another. The connecting line between two nodes is called an "**edge**". This is shown in the example below:


### Parts of Graphs

<img src="http://i.imgur.com/upMNKXf.png" width="400">

__Node / Vertex__: The entity of analysis which has a relationship. Node is used in the network context, vertex is used in the graph theory context, but both terms are often used interchangeably.

__Link / Edge / Relationship__: The connections between the nodes. Link is used in the network context, edge is used in the graph theory context, and all words are used interchangably with *relationship*.

__Attributes__: Both nodes and edges can store attributes, which contain additional data about that object.

__Weight__: A common *attribute* of edges, used to indicate *strength* or *value* of a relationship.

__Degree__: Number of edges a node has.

### Types of Graphs

Graphs are typically classified based on the presence of weights and direction attached to the edges in a graph. The table below covers what we call each type of graph:

|                | Absent     | Present  |
|----------------|------------|----------|
| __Weights__ | Unweighted | Weighted |
| __Directionality__ | Undirected | Directed |


Nodes in a graph are usually labeled to help identify them.  If the edges between the nodes are undirected, the graph is called an **Undirected Graph**. If an edge is directed from one vertex (node) to another, a graph is called a **Directed Graph**. An directed edge is called an **Arc**, as is represented with a arrow head.

<img src="g2.gif" width=500>

Weighted graphs may be shown with a weight value explicitly written, or visually it may be sown as strengths of the edges. 

<img src="weight.jpg" width=500>


In some cases, weights may be associated with nodes themselves instead of graphs , these options are shown below:
<img src="edge.gif" width=500>


### This is good , But why do I need to know about this ?

Think of an example of booking an Uber taxi using Uber's intelligent system relation drivers to clients. Think of Uber connecting a client to number of possible drivers , which can be shown as the graph below:

<img src="uber.png" width=400>


So the 6 possible rides (Ride 1 … Ride 6) are shown in this in graph, connected rider to the rides. The links between rider and rides are shown to reflect the distance between them. This makes it easier to visualize and match the closest ride to the user. We can clearly visualize that Ride 3 is the closest option.

Remember, here we are using a single metric (distance) for our decision. In a real life scenario, there are multiple metrics through which the allotment of a ride is decided, such as rating of the rider and driver, traffic between different routes, time for which the rider is idle, etc.


One the key benefits of using graphs in the data science domain is that its a great visualization and analysis technique. Graphs are incredibly useful in helping businesses make data-driven decisions.

Graphs allow us to visualize and process data in more detail, while using visual cues and other elements highlighting the relationships between different objects . For example, in the Twitter network graph below, (built using Python NetworkX, which we shall see shortly). This graph is based on the use of mention @Walmart.  We can see a strong tweet connection with Huggies. Network graphs like the one above can be used to study interactions in social media which may lead to insights that can be useful in the real world. 

<img src="walmart.JPG" width=700>

Let's have a look at another graph below. The points in the visual represent the characters of Game of Thrones, while the lines joining these points represent the connection between them. Jon Snow has connections with multiple characters, and the same goes for Tyrion, Cersei, Jamie, etc.

<img src="got.png" width=700>

## Summary 

In this lesson, we looked at basics of graph theory and what comprises a graph. We looked at how nodes and edges can form different formations within a graph. We also looked at some example of real world graphs. NExt we shall start digging a bit deeper into this topics and start building our graphs using the popular python library called `NetworkX`.
