# Game of Life simulator

## Summary and rules

This is a c implementation of John Conway's famous 'Game of Life'. The rules of the
'game' are simple. The universe of the game is a torus-connected two dimensional grid
filled with 'live' cells (denoted by 'X' in my implementation) and 'dead' cells (denoted
by ' '). At the beginning of the game, the grid is randomly populated with a some
distribution of live and dead cells, and cells are either born or destroyed based on
their interactions with their eight neighbors:

1. Any live cell with fewer than 2 living neighbors dies of loneliness.
2. Any live cell with more than 3 living neighbors dies of overcrowding.
3. A live cell with 2 or 3 neighbors continues on to the next generation
4. A dead cell surrounded by exactly 3 neighbors will be made live

