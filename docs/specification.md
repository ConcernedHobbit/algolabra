# Project specification

My degree programme is bachelor's in computer science (tkt). This document will be the baseline specification for the Algorithms & AI lab course in period 3 of the 2023-2024 academic year.

## Working language, programming language

The working language of this project is English. There are no Finnish elements.  
The work can be reviewed in Finnish, as I am a native speaker. I can also review English projects.  

The programming language used is **TypeScript**, a superset of **JavaScript**.  
This project should be easy enough to understand with only JS knowledge, but TS syntax is used in some cases to self-document and ensure type safety.

I also understand Java, Python, PHP and Ruby enough to review projects done in these languages. These are just the common languages that might be used, and I can be asked about others.

## Algorithm

The algorithm this project implements is the [Wave Function Collapse](https://github.com/mxgmn/WaveFunctionCollapse) ([Wikipedia](https://en.wikipedia.org/wiki/Wave_function_collapse)) simulation algorithm, referred to as WFC in the rest of the project.

Wave function collapse bases on quantum mechanics, but the core idea has been adopted to a computer simulation of a simpler version of the phenomenom. The GitHub repo linked as the base contains quite a lot more than the base WFC, but the core ideas I am aiming to implement can be summed up in [this description](https://github.com/mxgmn/WaveFunctionCollapse#algorithm) of the algorithm.

Although this may seem like a simple algorithm, backtracking and efficient consideration of the Shannon entropy of all tiles are important to have the algorithm fully complete a tile for any starting point and random seed value, as well as doing it in an efficient way that can be scaled up.

## Data structures

A memory-efficient WFC implementation requires its own data structure, to which I will get to given there is enough time in the project. Describing multiple "connectiont points" (sockets) per face of a tile and allowing tiles to be sorted by Shannon entropy are unique aspects of the data structure. The exact implementation is not clear to me yet.

## Why?

WFC seems simple, but has a lot of devious tricks in optimisation and backtracking. Implementing a working version of the algorithm is quite a challenge in itself, and then improving efficiency is a challenge in itself. If these are both done fast, WFC can be expanded with ideas from the base WaveFunctionCollapse project or with novel applications of the algorithm.

It is also visually interesting, and efficiency can be tested easily by scaling up the tilemap and size of the output.

## Program

The program is given a set of tiles and an area to fill. Optionally a starting point with a specific tile can be specified. A simplification can be a set of letters (tiles) that have rules for connecting each side of the letter (tile). The program then tries to create a solution, an NxN matrix, that follows the rules. This requires algorithmic backtracking in some situations, as the rules associated with tiles cannot be bruteforced easily.

## Sources

https://en.wikipedia.org/wiki/Wave_function_collapse

https://github.com/mxgmn/WaveFunctionCollapse