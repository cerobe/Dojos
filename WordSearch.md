# Word Search Solver

Write a program to find all the words (entered in plain text) in a grid.

# Puzzle

Input:

    U E W R T R B H C D
    C X G Z U W R Y E R
    R O C K S B A U C U
    S F K F M T Y S G E
    Y S O O U N M Z I M
    T C G P R T I D A N
    H Z G H Q G W T U V
    H Q M N D X Z B S T
    N T C L A T N B C E
    Y B U R P Z U X M S

    Contains: RUBY, DAN, ROCKS, MATZ

Expected output:

    + + + R + + + + + +
    + + + + U + + + + +
    R O C K S B + + + +
    + + + + + + Y + + +
    + + + + + + + + + M
    + + + + + + + D A N
    + + + + + + + T + +
    + + + + + + Z + + +
    + + + + + + + + + +
    Y B U R + + + + + +


# To go further

Too easy? How about generating a puzzle.

Input: 

    Words: THIS, PUZZLE, ROCKS, SOCKS

OUTPUT:

    A correct puzzle in the above form.

Accept:

- Words must be placed forwards
- Words must be placed in reverse
- Words must be placed in forwards diagonals
- Words must be placed in backwards diagonals
- Words may overlap


# Acknowledgement
Adapted from http://rubyquiz.com/quiz107.html by Daniel Finnie