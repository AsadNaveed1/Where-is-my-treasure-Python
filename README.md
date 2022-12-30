# Where-is-my-treasure-Python

# Q4: Where is my treasure?
Weight: 40%

Last update: 14 Nov, 10:00pm

In a game there is a map showing the location of various treasures featured in the gameplay. 

Each treasure is depicted by a square black-and-white pictogram represented as a grid of pixel values. 

Each pixel value is either 0 (representing a black pixel), or 1 (representing a white pixel).  

The treasures are of various dimensions. For example, the following 16x16 pixel grid represents a sword in the game: 

```

|1|1|1|1|1|1|1|1|1|1|1|1|1|0|0|0|
|1|1|1|1|1|1|1|1|1|1|1|1|0|0|0|0|
|1|1|1|1|1|1|1|1|1|1|1|0|0|0|0|0|
|1|1|1|1|1|1|1|1|1|1|0|0|0|0|0|1|
|1|1|1|1|1|1|1|1|1|0|0|0|0|0|1|1|
|1|1|1|1|1|1|1|1|0|0|0|0|0|1|1|1|
|1|1|0|0|1|1|1|0|0|0|0|0|1|1|1|1|
|1|1|0|0|0|1|0|0|0|0|0|1|1|1|1|1|
|1|1|1|0|0|0|0|0|0|0|1|1|1|1|1|1|
|1|1|1|0|0|0|0|0|0|1|1|1|1|1|1|1|
|1|1|1|1|0|0|0|0|1|1|1|1|1|1|1|1|
|1|1|1|0|0|0|0|0|0|1|1|1|1|1|1|1|
|1|1|0|0|0|1|0|0|0|0|1|1|1|1|1|1|
|0|0|0|0|1|1|1|1|0|0|1|1|1|1|1|1|
|0|0|0|1|1|1|1|1|1|1|1|1|1|1|1|1|
|0|0|0|1|1|1|1|1|1|1|1|1|1|1|1|1|

```

The map is also represented as a square grid of black-and-white pixels. The cell in the top left corner of the grid has (x,y) coordinates (0,0).

A treasure may appear in one of four possible orientations in the map: rotated clockwise through 0, 90, 180 or 270 degrees from the orientation of its stored representation. 

It is guaranteed that the given treasure appears exactly once in the map, however it may be in any one of the four orientations described above.

Write a program to find the map coordinates of the treasure’s location.  Report the map coordinates of the top left corner cell of the treasure as it appears on the map. (Note that the coordinates of the location are not affected by the orientation of the treasure.)



Assumptions:

Treasures do not overlap with other treasures or with other features in the map.

No treasure appears as part of the representation of any other treasure.

Example: 

You are searching for the sword in a 100x100 pixel map. If you find its pictogram

Rotated through 90 degrees, in the top left corner of the map, output 0 0

Not rotated, in the top left corner of the map, output 0 0

Rotated through 180 degrees, in the bottom left corner of the map, output 0 84

Input specification:

The first M lines contain the representation of the treasure. 

Each line contains M digits (0 or 1 only) representing pixel values. The i-th digit of the j-th line gives the value of the pixel at (x,y) coordinate (i,j) in the representation.

The remaining N lines contain the representation of the map in the same form as described above for the treasure.

In all test cases, 1 <= M < N <= 100.

Output specification:

The (x, y) coordinates of the top left corner cell of the treasure’s location in the map. The coordinates should be separated by a single space.
```
Sample input:

000
101
101
11111
11111
11011
11011
10001

Sample output:

1 2
Explanation: 

For this example, the input represents the following treasure and map.

Treasure:

|0|0|0|
|1|0|1|
|1|0|1|
Map:

|1|1|1|1|1|
|1|1|1|1|1|
|1|1|0|1|1|
|1|1|0|1|1|
|1|0|0|0|1|
The treasure, rotated through 180 degrees, appears in the bottom centre of the map. 

The top-left pixel of the treasure, as it appears in the map, is at map location (1,2).

```
