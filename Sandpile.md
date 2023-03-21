Sandpile & Sandmatrix
========
- A sandpile is a top-down view of a tower of sand grains. 
- When a sandpile is stable, its height ranges between 0 and 3, indicating the number of sand grains in the pile. 
- If a sandpile exceeds a height of 3, it will collapse in four directions: up, down, left, and right. 
- A sandmatrix is a collection of sandpiles, each number represent the heigh of the sandpile at that coordinate.

**Examples**  
In the following 3x3 Sandmatrix, the Sandpile at (1,1) has an height > 3 so it crumbles in the four directions
<pre>
000    010  
040 -> 101  
000    010  
</pre>
In the following 3x3 Sandmatrix, the Sandpile at (1,1) has an height > 3 so it crumbles in the four directions but there will be leftover
<pre>
000    010  
060 -> 121  
000    010  
</pre>
In the following 3x3 Sandmatrix, the Sandpile at (0,0) will crumbles, the grains going outside of the matrix are lost
<pre>
600    210  
000 -> 100  
000    000  
</pre>

Sandmatrix Addition
=================
- To add sandmatrices, add their sandpiles. Align the top left corners
- The result matrix might not be stable. If one of its sandpile is higher than 3 it will cramble.  

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
121   020   141    303    313
202 + 202 = 404 -> 040 -> 101
121   020   141    303    313
</pre>

**A lot of redistribution**
<pre>
121   303    212  
232 + 000 => 131  
121   303    212 
</pre>

**Bigger**  
<pre>
31003   11111    22112  
13120   12221    23321  
01310 + 12321 => 13231  
02131   12221    12332  
30013   11111    21122  
</pre>
 
