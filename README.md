# Growing target art

The 2D cellular automata made use of 3 colors, namely black, white, and red. The initial position of the patch is at the center of a white grid with a size of 3 by 3 black pixels. 

The rules are as follows:
If the current color is white: 
- If its black Moore neighbors are more than 1 and its red Von Neumann neighbors are more than 1, then set the "new-color" to black.
- If its red Von Neumann neighbors are more than 1, then set the "new-color" to blue.
- If its blue Moore neighbors are more than 2, then set the "new-color" to black.

If the current color is black:
- If its black Moore neighbors are more than 2, then set the "new-color" to red.

If the current color is red:
- If its red Moore neighbors are more than 2, then set the "new-color" to white.

After determining each patch's "new-color" and saving it in the "new-color" property, apply the "new-color" change to each patch. The rules are then repeated up to 101 times until the pattern is formed. 

Authors:
Caoile, Sean
Yongco, Denzel

Image
<img src="target.png">
