C# version and extension of Godot 3D Lines.

New: draw capsule ray

### Instructions:
- Add DrawLine3D.cs to the Godot [AutoLoad list](http://docs.godotengine.org/en/3.0/getting_started/step_by_step/singletons_autoload.html)  
- Call `DrawLine3D.Instance.DrawLine`, `DrawRay`, `DrawCapsuleRay` or `DrawCube` from any script  

`DrawLine` parameters: start point, end point, color (optional), time (optional)  
`DrawRay` parameters: start point, velocity (direction and magnitude), color (optional), time (optional)  
`DrawCube` parameters: start point, half extents (float), color(optional), time (optional)  
`DrawCapsuleRay` parameters: start point, radius, direction, length, color(optional), time (optional)

#### Examples
- `DrawLine3D.DrawLine(Vector3(0, 0, 0), Vector3(1, 2, 0), Color(0, 0, 1), 1.5)` Draws a line from (0, 0, 0) to (1, 2, 0) colored blue and will last for 1.5 seconds
- `DrawLine3D.DrawCube(Vector3(0, 1, 0), 0.5, Color(1, 0, 0))` Draws a cube at (0, 1, 0) with a half extent size of 0.5 and colored red

![Cube example](/CubeExample.png?raw=true "Cube example")
