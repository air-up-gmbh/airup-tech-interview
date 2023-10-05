ƒ# Mars Rover Kata
A squad of robotic rovers are to be landed by NASA on a plateau on Mars. The rovers must navigate this plateau so that their onboard cameras can get a complete view of the surrounding terrain to send back to Earth.

A rover’s position and location are represented by a combination of x and y coordinates and a letter representing one of the four cardinal compass points. The plateau is divided up into a grid to simplify navigation. An example position might be 0, 0, N, which means the rover is in the bottom left corner and facing North.

In order to control a rover, NASA sends a simple string of letters. The possible letters are `L`, `R` and `M`. 

`L` and `R` makes the rover spin 90 degrees left or right respectively, without moving from its current spot. `M` means move forward one grid point, and maintain the same heading.

Assume that a rover that moves forward facing North changes its position from (x, y) to (x, y + 1).

## Input
The first line of input is the upper-right coordinates of the plateau, the lower-left coordinates are assumed to be 0, 0.

The rest of the input is information related to the rovers that have been deployed. The second line gives the rover’s position, and the third line is a series of instructions telling the rover how to explore the plateau. The position is made up of two integers and a letter separated by spaces, corresponding to the x and y coordinates and the rover’s orientation.

## Output
The output should be the rover's final coordinates and heading.

## Examples
Test Input (1 rover): 
```
5 5
1 2 N
LMLMLMLMM
```

Expected Output:
```
1 3 N
```

Test Input (2 rovers):
```
5 5
1 2 N
LMLMLMLMM
3 3 E
MMRMMRMRRM
```

Expected Output:
```
1 3 N
5 1 E
```

There is no need to support multiple rovers from the start.

## Notes

We would like to see your TDD and Code Design, don't worry about completing the kata.

We have set up a TypeScript environment with tests, run `npm run install` and `npm run test` to execute the tests.

No libraries are expected to be involved with the implementation of the rover.

No CLI, API or UI is expected to be created.
