<img src="assn-imgs/img_1.jpg" width="400">

# Individual Assignment: Six Degrees of Separation

## Overview

The number of relationships that link people together in various domains is often vast. This concept was explored 
in the 1960s by social psychologist Stanley Milgram through his "small world" experiment, illustrating the phenomenon 
known as "six degrees of separation." For more details, see the 
[Small World Experiment on Wikipedia](https://en.wikipedia.org/wiki/Small-world_experiment).

### The Milgram Experiment

Milgram's experiment aimed to map the connections between distant individuals. If someone didn't know the target 
person directly, they were asked to pass a message through someone who might. The results showed that messages 
typically reached their intended recipient within five to six steps, which led to the concept of "six degrees 
of separation."

### The Kevin Bacon Game

Originating as a parlor game, the Kevin Bacon Game illustrates the small-world concept within Hollywood. The game 
challenges players to connect any actor to Kevin Bacon through their film roles in as few steps as possible. Each 
step forms a "Bacon number," which quantifies the separation degree.

### Graph Theory and its Application

In this assignment, we will use graph theory to analyze the "six degrees of separation" within Hollywood. 
You will develop a program that reads actor and movie data, constructs a graph of these relationships, and 
then calculates "actor numbers," which function similarly to Bacon numbers but with the actor of your choice 
as the central figure.

## Getting Started

Begin by downloading the starter files from the 
[GitHub repository](https://github.com/joshbarcher/kevin-bacon-game-assn). Included in the project are several 
files essential for building the graph-based application.

### Constructing the Graph

Your primary task is to build a graph linking actors to the movies in which they've appeared. This structure 
will support the computation of actor numbers.

### Computing Actor Numbers

You will implement a method using breadth-first search (BFS) to determine each actor's degree of separation 
from a chosen central actor.

### Console Application

Create a console application that enables users to:
- Load different datasets.
- Display lists of actors or movies.
- Compute actor numbers for a specified actor.

### Sample Console Interaction

```plaintext
Welcome to my Kevin Bacon Game!
*******************************
Please choose one of the following files:
0: 400_actors.txt
1: 200_actors.txt
2: 100_actors.txt
3: 50_actors.txt
2

Loaded 115 actors and 8859 movies.

Make a choice:
1. List Actors
2. List Movies
3. Calculate Actors Numbers
4. Exit
3

Enter an actor/actress name: jim carrey
Found actor!

jim carrey numbers:
adrian pasdar -> 1
albert finney -> 1
...
Average actor number: 1.2522522522522523

Make a choice:
1. List Actors
2. List Movies
3. Calculate Actors Numbers
4. Exit
4
Process finished with exit code 0