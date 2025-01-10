# Deadlock and Optimizations

Chessformer Puzzle Solver

This project implements a solver for "Chessformer" puzzles.
The solution use an optimized version of a search algorithm to find the shortest path from the initial state to the goal. 
The optimization includes duplication detection using hash tables, which avoids redundant state explorations.

ai.h and ai.c: Handles the AI logic and node management, including applying actions, creating new nodes, and exploring possible moves.
The code is written in C and uses the standard C library.

Input
You can play the game with the keyboard by executing

        ./chessformer <map>
        where map points to the file containing the chessformer problem to solve.

In order to execute your AI solver use the following command:

        ./chessformer -s <map> play_solution
        Where -s calls your algorithm. play_solution is optional, if typed in as an argument, the program will play the solution found by your algorithm once it finishes. All the options can be found if you use option -h:

        $./chessformer -h
        USAGE
                ./chessformer <-s> map <play_solution>

        DESCRIPTION
        Arguments within <> are optional
        -s                 calls the AI solver
        play_solution      animates the solution found by the AI solver

Output
The solver will print into an solution.txt file the following information: 

Solution
        Number of expanded nodes.
        Number of generated nodes.
        Number of duplicated nodes.
        Solutions length
        Number of nodes expanded per second.
        Total search time, in seconds.

Tools used  
- C  

Contributors
- Kerui Huang
- University of Melbourne COMP20003 Teaching Team (Skeleton Code and AI solver concept Provider)
- Sokoban made available by CorrentinB (Base game provider)

This project is for academic purposes under the University of Melbourne's COMP20003 course.

