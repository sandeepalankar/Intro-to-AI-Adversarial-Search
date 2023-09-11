# Intro-to-AI-Adversarial-Search

For this project, I developed an AI agent for a turn-based adversarial game based on the Wumpus world. The game will be played on a d by d grid, where d is a multiple of 3 (e.g. 3x3, 6x6, 9x9 ect.). Each cell is either empty or
contains a pit. To place the pits you should select d/3-1 cells in each row except for the
top and bottom row and mark them as pits.

Both players will have a set of d pieces which consist of d/3 Wumpuses, d/3 heroes and
d/3 mages. The agent's pieces will start in the top row of the grid and the adversary's
pieces will start in the bottom row of the grid. The pieces will start in alternating order from
left to right starting with a Wumpus, a hero and a made (so if you have a 6/6 grid there will
be Wumpus in cell 1,1 a hero in cell 1,2 a mage in cell 1,3, a Wumpus in cell 1,4 a hero in
cell 1,5 and a mage in cell 1,6.

The game proceeds in a turn based manner starting with the adversary player. During
each turn a player must select exactly one piece and move it one square horizontally,
vertically or diagonally. If a piece is move into a square containing one of the opponent's
pieces then they do battle. If a hero battles a wumpus then the her shoots the wumpus
and kills it. If a mage does battle with a hero then it uses its fire magic to destroy the hero.
If a wumpus does battle with a mage then the wumpus will eat the mage. If two pieces of
the same type do battle then both pieces are destroyed. If a piece moves into a cell
containing a pit then it is destroyed and a player cannot move a piece into a cell that
contains one of their own pieces. If the game reaches a state where one of the player's
pieces are all destroyed then the other player wins. If both players ave no pieces left ten
the game is a draw.
