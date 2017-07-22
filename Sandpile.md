Sandpile addition
=================
A sandpile is a square matrix of natural numbers between 0 and 3, representing how many grains of sand there is on each square
To add two sandpiles, just start by adding the two matrices element by element. Except the matrix you generate might not be a sandpile, if one of its element is higher than 3 you must transform this matrix into a sandpile, and this is how it is done :
- If a square has 4 grains of sand or more, it "loses" four and distributes it to its four neighbors (if the square touches an edge, the grain of sand is lost)
- Keep doing that to all the squares with 4 grains or more until all the squares have 3 grains or less

**Example**  
<pre>
000   000   000    010  
020 + 020 = 040 -> 101  
000   000   000    010  
</pre>

Scenarios
=========
**One simple addition**
<pre>
121   020    313  
202 + 202 -> 101  
121   020    313  
</pre>

**A lot of redistribution**
<pre>
121   303    212  
232 + 000 -> 131  
121   303    212 
</pre>

**Bigger**  
<pre>
31003   11111    22112  
13120   12221    23321  
01310 + 12321 -> 13231  
02131   12221    12332  
30013   11111    21122  
</pre>

# Acknowledgement
Adapted from https://www.codingame.com/
 