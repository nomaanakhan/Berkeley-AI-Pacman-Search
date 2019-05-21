# AI-Pacman-Search
Implementing Depth First Search, Breadth First Search, Uniform Cost Search, and A* Search for a pacman.

For full documentation refer http://ai.berkeley.edu/search.html

## To Run

### Breadth First Search

python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs

python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5

If Pacman moves too slowly for you, try the option --frameTime 0.

### Depth First Search

python pacman.py -l tinyMaze -p SearchAgent

python pacman.py -l mediumMaze -p SearchAgent

python pacman.py -l bigMaze -z .5 -p SearchAgent

### Uniform Cost Search

python pacman.py -l mediumMaze -p SearchAgent -a fn=ucs

python pacman.py -l mediumDottedMaze -p StayEastSearchAgent

python pacman.py -l mediumScaryMaze -p StayWestSearchAgent

### A* Search

python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic

### Finding All the Corners

python pacman.py -l tinyCorners -p SearchAgent -a fn=bfs,prob=CornersProblem

python pacman.py -l mediumCorners -p SearchAgent -a fn=bfs,prob=CornersProblem

### Corners Problem: Heuristic

python pacman.py -l mediumCorners -p AStarCornersAgent -z 0.5

-p SearchAgent -a fn=aStarSearch,prob=CornersProblem,heuristic=cornersHeuristic

### Eating All The Dots

python pacman.py -l testSearch -p AStarFoodSearchAgent

python pacman.py -l trickySearch -p AStarFoodSearchAgent

### Suboptimal Search

python pacman.py -l bigSearch -p ClosestDotSearchAgent -z .5 
