==Conway's Game of Life (or simply Life)==

It's an interesting game/simulation/Turing-complete game developed by Conway in 1970
The rules are simple:
- 2 type of cell: live (L) and dead (D)
- a cell is surrounded by 8 possible neighbours (N)
- L && N < 2| N > 3 => D
- D && N == 3 => L

Logical arithmetic can be simulated with patterns in Life => it's a Turing-complete machine
