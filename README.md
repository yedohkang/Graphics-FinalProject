# theEnd
Final Graphics Project with Alex Lu, Period 4

What we have done: 
- Created 5 new primitive shapes: Tetrahedron, Cone, Cylinder, Ellipsoid, and Triangular Prism
- Create options to vary knobs in exponential fashion

New MDL commands:
- tetrahedron: takes in 12 doubles (x0, y0, z0, x1, y1, z1, x2, y2, z2, x3, y3, z3), corresponding to the 4 points of a tetrahedron
- cone: takes in 5 doubles (cx, cy, cz, r, h), corresponding to the center of the base of the cone, the radius of the base, and the height of the cone
- cylinder: takes in 5 doubles (cx, cy, cz, r, h), corresponding to the center of the base of the cylinder, the radius of the base, and the height of the cylinder
- ellipsoid: takes in 6 doubles (cx, cy, cz, a, b, c), corresponding to the center of the ellipsoid, and the three principal semi-axis of the ellipsoid
- triprism: takes in 10 doubles (x0, y0, z0, x1, y1, z1, x2, y2, z2, h), corresponding to the three verticies of the triangular base, and the height of the triangular prism

Modifications to existing MDL commands:
- Vary may now take a 5th argument. The 5th argument is a double, and will correspond to the exponent of the rate the knobs will vary.

INPUT | EFFECT 
:---: | --- 
```vary spinny 0 99 0 1``` | the same old vary we already know
```vary spinny 0 99 0 1 2``` | the spinny knob will vary as a square, so the variation will start slowly, then speed up

Instructions:
Feel free to create any mdl of your liking. Running the following:
```
mkdir anim
make
animate simple.gif
```
will create a gif with a falling (in this order) ellipsoid, tetrahedron, cylinder, cone, and triangular prism, each rotating, and each falling in a linear, quadratic, cubic, quartic, and quintic rate, respectively.
