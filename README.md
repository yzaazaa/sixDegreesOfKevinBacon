# Six Degrees Of Kevin bacon

## Overview
This project, part of the AI50 course at Harvard, focuses on finding the shortest path between two actors/stars based on their shared movie credits.

## Features
- Loads and parses actor/movie data from CSV files
- Allows user to input a source and target actor/star
- Calculates the degrees of separation between the two actors using a Breadth-First Search (BFS) algorithm
- Outputs the sequence of movies/actors in the shortest path

## Usage
1. Clone the Repository:
```bash
git clone https://github.com/yzaazaa/sixDegreesOfKevinBacon
cd sixDegreesOfKevinBacon
```

2. Run the script:
```
python degrees.py  <"small" or "large" (optional: small if no selection)>
```

## Example Output
```
Loading data...
Data Loaded.
Name: Emma Watson
Name: Tom Hanks
1 degrees of separation.
1: Emma Watson and Tom Hanks starred in A Few Good Men

Loading data...
Data Loaded. 
Name: Kevin Bacon
Name: Jack Nicholson
1 degrees of separation.
1: Kevin Bacon and Jack Nicholson starred in A Few Good Men

Loading data...
Data Loaded.
Name: Demi Moore 
Name: Gary Sinise
2 degrees of separation.
1: Demi Moore and Kevin Bacon starred in A Few Good Men
2: Kevin Bacon and Gary Sinise starred in Apollo 13

Loading data...
Data Loaded.
Name: Valeria Golino
Name: Robin Wright
4 degrees of separation.
1: Valeria Golino and Tom Cruise starred in Rain Man
2: Tom Cruise and Kevin Bacon starred in A Few Good Men
3: Kevin Bacon and Tom Hanks starred in Apollo 13
4: Tom Hanks and Robin Wright starred in Forrest Gump
```