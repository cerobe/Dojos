Sandpile
========
A Sandpile is a tower of sand grain. The tower high is between 0 and 3 and represent how many grains of sand there is in the pile. If a sandpile is higher that 3, it will crumble in the four directions (Up, Down, Left, Right)

**Example**  
<pre>
000    010  
040 -> 101  
000    010  
</pre>
<pre>
000    010  
060 -> 121  
000    010  
</pre>

Sandpile Matrix
==============
A sanpile matrix is a collection of sandpile. Each sandpile matrix is square, so the width is equal to the height.

Sandpile addition
=================
To add two sandpiles, just start by adding the two matrices element by element. Except the matrix you generate might not be a stable sandpile, if one of its element is higher than 3 you must transform this matrix into a sandpile, and this is how it is done :
- If a square has 4 grains of sand or more, it "loses" four and distributes it to its four neighbors (if the square touches an edge, the grain of sand is lost)
- Keep doing that to all the squares with 4 grains or more until all the squares have 3 grains or less

**Example**  
<pre>
000   000   000    010  
020 + 020 = 040 -> 101  
000   000   000    010  
</pre>

Scenarios for the Dojo
=========
The goal is to write a program that will solve the following scenario.
Don't forget to try with the example first for an easy start.

**One simple addition with multiple crumbles**
<pre>
121   020    141    303    313
202 + 202 -> 404 -> 040 -> 101
121   020    141    303    313
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
 
