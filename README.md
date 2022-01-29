# Brain Network Analysis
I have included details about a research done paper done on the topic "Brain Network Analysis using the Burning number of Graph"

**Team:** 

Shakthi Varsha, Bio Medical Engineering, SSN College of Engineering, Chennai

Vahini Mahesh, Bio Medical Engineering, SSN College of Engineering, Chennai

Yaswanth Udayakumar, Computer Science and Engineering, SSN College of Engineering, Chennai

## Purpose of the research
The human brain is a network where different parts/nodes of the brain are connected to each other. We had researched on the effects of meditation in the brain network.

EEG values were taken from the brain befoe and after meditation and a graph of the network was produced. The the burnning times of each graph was calculated and it was proven that meditation helps information to pass on faster in the brain as the burning number is less. The burning number was calculated using an algorithm which was then implemented into code using Python 3.0 and the results were confirmed using the code.

This research in the end helped us prove that meditation is in fact very helpful for humans as it helps information flow faster in our brain. 

Thank you for spending your valuable time reading about the subject of our paper!

## Introduction
The brain is the biological hardware from which all our thoughts, feelings, and behaviour
emerge. It is therefore unsurprising that understanding the network organisation of the
brain has been a long-standing challenge. The network organization of the brain, as it is
beginning to be revealed by graph theory, is compatible with the hypothesis that the
brain, perhaps in common with other complex networks, has evolved both to maximize
the efficiency of information transfer and to minimize connection cost, at all scales of
space and time.

Graph theory has many real time applications in engineering and technology. It is
particularly useful in the study of the human brain. The human brain is modelled as a
graph in which neurons are taken as nodes or vertices and the physical link between the
neurons are taken as edges. The brain is a more complex network, it consists of a greater
number of neurons, it is not possible to consider all the neurons and their links. So, it can
be clustered into working regions, or lobes, as region of interest to effectively model it.
Meditation plays a vital role in improving brain performance, and helps to improve grey
matter concentration, focus, attention and to reduce work stress.

In this paper, we try to show how fast an information can spread to the entire brain
network before and after meditation by using graph burning model. With the
electroencephalography (EEG) results of the brain (before and after meditation) we can
analyse the speed at which the influence spreads to every vertex. To quantify the speed at
which the influence spreads to every vertex in the brain network, we employ burning
number measurement.

## Burning Number
The concept of graph burning was introduced by Anthony Bonato, Jeannette Janssen, and
Elham Roshanbin in 2015. Graph burning can be used to model how quickly a disease
can spread through a group of people. Burning numbers are discrete time-steps or rounds.
Each node is either burned or unburned; if a node is burned, then it remains in that state
until the end of the process. In every round, we choose one additional unburned node to
burn (if such a node is available). Once a node is burned in round t, in round t + 1, each
of its unburned neighbours becomes burned. The process ends when all nodes are burned.
The burning number of a graph G, written by b(G), is the minimum number of rounds
needed for the process to end. The lower the value of b (G), the easier it is to spread such
contagion in the graph G. Suppose that in the process of burning a graph G, we
eventually burned the whole graph G in k steps, and for each i;1≤i≤ k, we denote the
node that we burn in the i th step by x i . We call such a node simply a source of fire. The
sequence (x1, x2 . . . x k ) is called a burning sequence for G.

The burning process may be highly dependent on the choice of sources. For example, in a
path, burning spreads at a slower rate from a source that is an end-vertex than from a
central vertex. Hence, the choice of sources is critical when minimizing the length of the
process. The burning number corresponds to an optimal choice of sources throughout the
process. The sources that are chosen over time are referred to as a burning sequence; a
shortest such sequence is called optimal. Hence, optimal burning sequences have length,
b (G).

## Example
<p align="center" width="100%">
    <img width="33%" src="https://user-images.githubusercontent.com/68239314/151661481-d693efa7-7910-40cd-ad97-8da3961ad3b5.png">
</p>

<p align="center" width="100%">
    <img width="33%" src="https://user-images.githubusercontent.com/68239314/151661506-0008d91e-5439-4773-81bf-a1f82c9c7929.png">
</p>

<p align="center" width="100%">
    <img width="33%" src="https://user-images.githubusercontent.com/68239314/151661564-faac8626-cb88-4793-9156-a8848779ddc3.png">
</p>

<p align="center" width="100%">
    <img width="33%" src="https://user-images.githubusercontent.com/68239314/151661586-a39ae18b-035e-4fe8-bf18-ecdfb77cbe56.png">
</p>

<p align="center" width="100%">
    <img width="33%" src="https://user-images.githubusercontent.com/68239314/151661601-c51e2165-e043-4aac-a9bf-f2445672af13.png">
</p>

<p align="center" width="100%">
    <img width="33%" src="https://user-images.githubusercontent.com/68239314/151661622-d56b9a4b-a316-4cd8-ad14-fd4a6183089d.png">
</p>

## Properties of Burning Number
- If G is a graph and v is a node of G, then the eccentricity of v is defined as Max
{d (v, u): u V (G)}. The radius of G is the minimum eccentricity over the set of
all nodes in G. The centre of G consists of the nodes in G with minimum
eccentricity. Given a positive integer k, the k-th closed neighbourhood of v is
defined to be the set {u V (G): d (u, v) ≤ k} and is denoted by Nk [v]. N1 [v]
denotes N[v].
- Suppose that (x1, x2 . . . xk), where k ≥ 3, is a burning sequence for a given graph
G. For 1 ≤ i ≤ k, the fire spread from xi will burn only all the nodes within
distance k - i from xi by the end of the k-th step. On the other hand, every node v
V (G) must be either a source of fire, or burned from at least one of the sources of
fire by the end of the k-th step.
- In other words, any node of G that is not a source of fire must be an element of N
k-i [xi], for some 1 ≤ i ≤ k. Therefore, we can see that (x1, x2 . . . xk) forms a
burning sequence for G if and only if the following set equation holds:
Nk-1 [x1] Nk-2 [x2] ∪ . . . ∪ N0 [xk] = V (G)


**Disclaimer:** For privacy reasons, the algorithm of the code cannot be released publicly and so are the other parts of the paper.
