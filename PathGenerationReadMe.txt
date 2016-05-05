This program runs on Microsoft Visual Studio 2015 and it uses OpenGL, so you'll need to include the required libraries to run the program.

******************************
Some instructions:
1) left mouse click -> creates a new control point
2) right mouse click -> stop adding control points
3) 's' key -> engage in autonomous path generation mode
4) 'e' key -> user interactive mode, which allows manual knot insertions
5) 'p' key -> enable control point adjustment, place cursor within the displayed circle around the current control point to be adjusted
6) '+' key -> adjust next control point
7) '-' key -> adjust previous control point


******************************
For the autonomous path generation to work, place the control points at each corner. 

********************************
The following are the functions that govern the autonomous behavior:

In PathGeneration.cpp
 1) FindNormalAndTangent
 2) CheckCorridorConstraint
 3) AdjustControlPointForLine
 4) find_rotation_direction
 5) AdjustControlPointForArc
 6) AddControlPoint
 7) CheckSegmentConstraint
 8) FindAverageFailedKnots
 9) ReadjustControlPoint

In main.cpp
 10) some autonomous codes from line 415 to 600 within the display function in main.cpp