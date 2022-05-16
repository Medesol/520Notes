# Cloth Simulation
电影中可以当作physical object模拟，游戏中不能，因为游戏中是实时的。

No springs any more, instead, there are3 kind of engergy:
- stretch
- Bend: change normal of two triangles, equals to $\theta$, which is the angle of the two normals
	- much harder and still being better
- Shear, dot product. mearsuring the angle between them.
	- also affected by stretching
	- correct it need more computation so don't

By differentiate them, the forces can be calculated.

Implemented by Vega

Without self collision
 
![[Pasted image 20220506220110.png]]