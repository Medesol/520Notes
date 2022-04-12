## 问题

- 衣服（Marvelous Designer）
- 液体
- 头发
- 触觉（haptics）

## Parts

- Modeling
	- neutral, what this creature looks like. Shapes, angels. 整个模型表面的三角形。颜色
		- Mesh
		- Texures
		- Normal Maps
		- Lighting Maps
	- 建模师(Modeler)用3D建模软件做
	- 静止
- Rigging
	- 输出：Animation-Ready Character
	- 生成骨架（skeleton），just some joints，no mesh
		- 树，joint hierarchy
	- Rigger
- Animation
	- bind pose
	- specify joint tranfermations （e.g. $\alpha ,\beta ,\gamma$ for all joints）
	- Depend on the rigger(太少关节会限制移动，太多会让动画师工作复杂很多)
	- Animator