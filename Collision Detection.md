- Volumetric 方式更不容易出现错误，也更容易施加penalty force
- Structure object: in priory know some micro demormation and can be linear combined.
- B-rep: boundary representation
- OBB: CAN BE tilted
- Convex hull: computation hard, seldom used.
- AABB: often used for self-detection. collide when 2 spans are intersect.
- Sphere:
	- 很多空出来的位置，不精确
	- 计算出最合适的sphere很慢

## Bounding Volume Test Tree
- Collision front
- Temporal Coherance
- 提前算出每个三角形分属的bounding volume

## PCA 算法算出main axis of a box
![[Pasted image 20220509052808.png]]
## Spacial subdivision
tile, Hashtable, 每个tile包含哪些三角形需要经常计算
![[Pasted image 20220509054600.png]]
## Self Collision Detection
- check if the mesh is clean 

Make a test tree copy of itself

speed up when we know how it deforms