---

layout: default
---

# Ball-Balancer
The Ball-Balancing system is a SISO system that uses PID to control the ball's position on a plate. 
By adjusting the plate we set the acceleration of the ball and move it towards a reference position. 
The system consists of a ball on an elevated plate. this plate can be tilted about its center of mass, along either its width or length. The controller will be connected to two actuators, controlling the tilt along each axis independently. The feedback will come from a camera mounted directly above the center of the plate. The ball will begin at rest in the center of the plate. Then an external force will be applied to the ball moving it off of the center of the plate. The controller should be able to keep the ball on the plate and return it to the center. The feedback to the controller will be a float in [-1:1], the x and y position of the ball, with the center of the plate as the origin

### Mechanical Design
A major challenge was to design an actuation mechanism for the top plate. In order to run use only one axis we designed a new mechanism which would allow us to uncouple the dynamics of the actuation mechanism and hence allow us to actuate the servo motors independently correspond- ing to its axis without affecting the other. We also simplified the dynamics by this mechanism which would keep the inclination angle of top plate equal to the actuator rotation.The plate has to rotate about its two planar body axes to be able to balance the ball. A special pivot mount was designed which would allow the rotation of top plate in x and y axis

[!][](../Images/Ball_Balancer/cad.png)
