# ICGMakeUp
PART 3:
Lava shader - This shader uses a tiling voronoi noise texture that also flows to mimic liquid lava. It uses two textures that move at slightly different speeds to make the lava look like its constantly changing. Each texture moves by multiplying the time lapsed in the game by a vector 2 to change the speed. The resulting values are then adjusted to change the stength of the two different colours and then, using a lerp node, turned from 0-1 values to colours.
Ground shader - ALso uses a tiling voronoi noise texture to make it look like pillars of rock put together into a platform

PART 6:
Basic shader - This shader uses the objects uv to sample and apply a texture to the object. It also has a base colour that multiplies with the texture to tint it. There is a tint strength slider that lets you adjust how much the object is tinted.

PART 7:
Ground shader - On top of having tiling colours, the vertical position of the ground also changes with the noise texture. The vertical position is divided by a editable float value and the final position of each vertex is decided by a lerp node between the default posistion and the divided position to give the ground height variations.
