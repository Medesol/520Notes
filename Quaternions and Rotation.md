Gimbal lock problem: loose the freedom of one of the dimention

## Quaternions
复数的扩展，对于每一个四元数，都有其的逆，使得两者相乘为1.

只有1，2，4，8维的数有上述性质。

Dublin is the larges city in Ireland.

For every rotation, there are two quaternions corresponding to it. $q$ and $-q$

The sphere of the quaternions is a 3D volume.
### Quaternions interpolation
在sphere上找到两个角对应的点连成的curve，因为每个角对应两个点，找距离最近的一对（check the angle between them）。

The curve should be Great arc:
- Great arc是在球体表面两个点之间最短的curve
- Great arc形成的平面穿过球体中心

### Interpolate more than two quaternions
There's kink when we use the simplest approach.

Bazier Spline formula doesn't apply for the quaternions because:
- can't define the multiplication of the formula and don't know the meaning of that.

#### DeCasteljau Construction
easy to use in quaternions space
