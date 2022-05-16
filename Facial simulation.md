- Live stage capture: invented in USC and very precise with geometry
- Faces are very complicated so it's very hard to simulate

## Facial rig
used to generate facial animation. Can get sliders which change the expression

#### 肌肉类型
- sphincter: 括约肌
- linear muscle
- Sheet muscle: composed of several linear muscle

There is no opposing muscle on faces.

### Facial Action Coding System(FACS)
- action units 
- intensity
- can be added
### MPEG 4 standard
- displacement of 68 landmarks on face.
- can't tansfered to other people. 

## Facial animation and rigging
no joint angles.

- WRAP3: use ICP(iterative closest point) 解决两次扫描之后的mesh不同问题
	- bring the two meshes into correspondance

- Scanning 
- Cleanup
- Then tweak parameters to create animation 

alphas are Extra parameters/Sliders

Combination Shape: because muscles are non-linearly. Just scan important ones.
![[Pasted image 20220508032922.png]]
## Physics based
