---
ID_PAGE: 3329
PG_TITLE: Matrix
PG_VERSION: 1.14
---

Creates a new 4 by 4 matrix

##Members

###m : Float32Array


The matrix, which is an array



##Methods

###isIdentity() &rarr; boolean
Tests if the matrix is an identity matrix


###determinant() &rarr; number
Returns the determinant of the matrix


###toArray() &rarr; Float32Array
Returns the matrix in array form


###asArray() &rarr; Float32Array
Returns the matrix in array form


###invert() &rarr; void
Inverts the matrix


###invertToRef(other) &rarr; void
Inverts the matrix and put it into another matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | other | [Matrix](page.php?p=3329) | Another matrix
---

###setTranslation(vector3) &rarr; void
Sets a translation to the matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | vector3 | [Vector3](page.php?p=3327) | The translation to apply
---

###multiply(other) &rarr; [Matrix](page.php?p=3329)
Multiplies by another matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | other | [Matrix](page.php?p=3329) | Another matrix
---

###copyFrom(other) &rarr; void
Copies another matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | other | [Matrix](page.php?p=3329) | Another matrix
---

###copyToArray(array, offset) &rarr; void
Copies the current matrix into an array

####Parameters
 | Name | Type | Description
---|---|---|---
 | array | Float32Array | The target array
optional | offset | number | The first index of the array to fill in
---

###multiplyToRef(other, result) &rarr; void
Multiplies another matrix into an existing matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | other | [Matrix](page.php?p=3329) | Anoher matrix
 | result | [Matrix](page.php?p=3329) | The matrix to put the result into
---

###multiplyToArray(other, result, offset) &rarr; void
Multiplies another matrix into an existing array at a given index

####Parameters
 | Name | Type | Description
---|---|---|---
 | other | [Matrix](page.php?p=3329) | Another matrix
 | result | Float32Array | The matrix to put the result into
 | offset | number | The first index of the matrix to put the result into
---

###equals(value) &rarr; boolean
Tests if two matrices are equal

####Parameters
 | Name | Type | Description
---|---|---|---
 | value | [Matrix](page.php?p=3329) | The matrix to test against
---

###clone() &rarr; [Matrix](page.php?p=3329)
Clones a martix


###static FromArray(array, offset) &rarr; [Matrix](page.php?p=3329)
Creates a new matrix from an array from a given index

####Parameters
 | Name | Type | Description
---|---|---|---
 | array | number[] | The given array
optional | offset | number | The first index of the array to look in
---

###static FromArrayToRef(array, offset, result) &rarr; void
Fills an existing matrix with an array from a given index

####Parameters
 | Name | Type | Description
---|---|---|---
 | array | number[] | The array to copy
 | offset | number | The first index to copy from
 | result | [Matrix](page.php?p=3329) | The existing matrix
---

###static FromValuesToRef(initialM11, initialM12, initialM13, initialM14, initialM21, initialM22, initialM23, initialM24, initialM31, initialM32, initialM33, initialM34, initialM41, initialM42, initialM43, initialM44, result) &rarr; void
Fills an existsing matrix with a set of values

####Parameters
 | Name | Type | Description
---|---|---|---
 | initialM11 | number | initial MM11 1,1 value
 | initialM12 | number | initial MM12 1,2 value
 | initialM13 | number | initial MM13 1,3 value
 | initialM14 | number | initial MM14 1,4 value
 | initialM21 | number | initial MM21 2,1 value
 | initialM22 | number | initial MM22 2,2 value
 | initialM23 | number | initial MM23 2,3 value
 | initialM24 | number | initial MM24 2,4 value
 | initialM31 | number | initial MM31 3,1 value
 | initialM32 | number | initial MM32 3,2 value
 | initialM33 | number | initial MM33 3,3 value
 | initialM34 | number | initial MM34 3,4 value
 | initialM41 | number | initial MM41 4,1 value
 | initialM42 | number | initial MM42 4,2 value
 | initialM43 | number | initial MM43 4,3 value
 | initialM44 | number | initial MM44 4,4 value
 | result | [Matrix](page.php?p=3329) | The exisiting matrix
---

###static FromValues(initialM11, initialM12, initialM13, initialM14, initialM21, initialM22, initialM23, initialM24, initialM31, initialM32, initialM33, initialM34, initialM41, initialM42, initialM43, initialM44) &rarr; [Matrix](page.php?p=3329)
Creates a matrix from set of values

####Parameters
 | Name | Type | Description
---|---|---|---
 | initialM11 | number | initial MM11 1,1 value
 | initialM12 | number | initial MM12 1,2 value
 | initialM13 | number | initial MM13 1,3 value
 | initialM14 | number | initial MM14 1,4 value
 | initialM21 | number | initial MM21 2,1 value
 | initialM22 | number | initial MM22 2,2 value
 | initialM23 | number | initial MM23 2,3 value
 | initialM24 | number | initial MM24 2,4 value
 | initialM31 | number | initial MM31 3,1 value
 | initialM32 | number | initial MM32 3,2 value
 | initialM33 | number | initial MM33 3,3 value
 | initialM34 | number | initial MM34 3,4 value
 | initialM41 | number | initial MM41 4,1 value
 | initialM42 | number | initial MM42 4,2 value
 | initialM43 | number | initial MM43 4,3 value
 | initialM44 | number | initial MM44 4,4 value
---

###static Identity() &rarr; [Matrix](page.php?p=3329)
Returns the identity matrix


###static IdentityToRef(result) &rarr; void
Fills an existing matrix with the identity matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | result | [Matrix](page.php?p=3329) | The existing matrix
---

###static Zero() &rarr; [Matrix](page.php?p=3329)
Returns a null matrix


###static RotationX(angle) &rarr; [Matrix](page.php?p=3329)
Rotates a matrix around X axis

####Parameters
 | Name | Type | Description
---|---|---|---
 | angle | number | The X angle of rotation
---

###static RotationXToRef(angle, result) &rarr; void
Rotates a matrix around X axis into an existing matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | angle | number | The X angle of rotation
 | result | [Matrix](page.php?p=3329) | The existing matrix
---

###static RotationY(angle) &rarr; [Matrix](page.php?p=3329)
Rotates a matrix around Y axis

####Parameters
 | Name | Type | Description
---|---|---|---
 | angle | number | The Y angle of rotation
---

###static RotationYToRef(angle, result) &rarr; void
Rotates a matrix around Y axis into an existing axis

####Parameters
 | Name | Type | Description
---|---|---|---
 | angle | number | The Y angle of rotation
 | result | [Matrix](page.php?p=3329) | The existing matrix
---

###static RotationZ(angle) &rarr; [Matrix](page.php?p=3329)
Rotates a matrix around Z axis

####Parameters
 | Name | Type | Description
---|---|---|---
 | angle | number | The Z angle of rotation
---

###static RotationZToRef(angle, result) &rarr; void
Rotates a matrix around Z axis into an existing axis

####Parameters
 | Name | Type | Description
---|---|---|---
 | angle | number | The Z angle of rotation
 | result | [Matrix](page.php?p=3329) | The existing matrix
---

###static RotationAxis(axis, angle) &rarr; [Matrix](page.php?p=3329)
Rotates a matrix using a [Vector3](page.php?p=3327)

####Parameters
 | Name | Type | Description
---|---|---|---
 | axis | [Vector3](page.php?p=3327) | [Vector3](page.php?p=3327) axis of the rotation
 | angle | number | angle of the rotation
---

###static RotationYawPitchRoll(yaw, pitch, roll) &rarr; [Matrix](page.php?p=3329)
Rotates a matrix using yaw, pitch and roll values

####Parameters
 | Name | Type | Description
---|---|---|---
 | yaw | number | The yaw rotation value
 | pitch | number | The pitch rotation value
 | roll | number | The roll rotation value
---

###static RotationYawPitchRollToRef(yaw, pitch, roll, result) &rarr; void
Rotates a matrix using yaw, pitch and roll values and put it into a target matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | yaw | number | The yaw rotation value
 | pitch | number | The pitch rotation value
 | roll | number | The roll rotation value
 | result | [Matrix](page.php?p=3329) | The target matrix
---

###static Scaling(x, y, z) &rarr; [Matrix](page.php?p=3329)
Creates a scaling matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | x | number | The X scaling factor
 | y | number | The Y scaling factor
 | z | number | The Z scaling factor
---

###static ScalingToRef(x, y, z, result) &rarr; void
Creates a scaling matrix and put it into a target matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | x | number | The X scaling factor
 | y | number | The Y scaling factor
 | z | number | The Z scaling factor
 | result | [Matrix](page.php?p=3329) | The matrix target
---

###static Translation(x, y, z) &rarr; [Matrix](page.php?p=3329)
Creates a matrix with a translation pitch defined by x, y, z

####Parameters
 | Name | Type | Description
---|---|---|---
 | x | number | The X translation value
 | y | number | The Y translation value
 | z | number | The Z translation value
---

###static TranslationToRef(x, y, z, result) &rarr; void
Creates a matrix with a translation pitch defined by x, y, z and put it into a target matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | x | number | The X translation value
 | y | number | The Y translation value
 | z | number | The Z translation value
 | result | [Matrix](page.php?p=3329) | The matrix target
---

###static LookAtLH(eye, target, up) &rarr; [Matrix](page.php?p=3329)
Builds a left-handed look-at [Matrix](page.php?p=3329)

####Parameters
 | Name | Type | Description
---|---|---|---
 | eye | [Vector3](page.php?p=3327) | The [Vector3](page.php?p=3327) that defines the camera point
 | target | [Vector3](page.php?p=3327) | The [Vector3](page.php?p=3327) that defines the camera look-at target
 | up | [Vector3](page.php?p=3327) | The [Vector3](page.php?p=3327) that defines the up direction
---

###static LookAtLHToRef(eye, target, up, result) &rarr; void
Builds a left-handed look-at [Matrix](page.php?p=3329) and put it in a target matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | eye | [Vector3](page.php?p=3327) | The [Vector3](page.php?p=3327) that defines the camera point
 | target | [Vector3](page.php?p=3327) | The [Vector3](page.php?p=3327) that defines the camera look-at target
 | up | [Vector3](page.php?p=3327) | The [Vector3](page.php?p=3327) that defines the up direction
 | result | [Matrix](page.php?p=3329) | The matrix target
---

###static OrthoLH(width, height, znear, zfar) &rarr; [Matrix](page.php?p=3329)
Creates a left-handed orthogonal projection matrix.

####Parameters
 | Name | Type | Description
---|---|---|---
 | width | number | The width of the view volume
 | height | number | The height of the view volume
 | znear | number | The minimum z value of the view volume
 | zfar | number | The maximum z value of the view volume
---

###static OrthoOffCenterLH(left, right, bottom, top, znear, zfar) &rarr; [Matrix](page.php?p=3329)
Creates a custom left-handed orthogonal projection matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | left | number | The minimum x value of the view volume
 | right | number | The maximum x value of the view volume
 | bottom | number | The minimum y value of the view volume
 | top | number | The maximum y value of the view volume
 | znear | number | The minimum z value of the view volume
 | zfar | number | The maximum z value of the view volume
---

###static OrthoOffCenterLHToRef(left, right, bottom, top, znear, zfar, result) &rarr; void
Creates a custom left-handed orthogonal projection matrix and put it into the target matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | left | number | The minimum x value of the view volume
 | right | any | The maximum x value of the view volume
 | bottom | number | The minimum y value of the view volume
 | top | number | The maximum y value of the view volume
 | znear | number | The minimum z value of the view volume
 | zfar | number | The maximum z value of the view volume
 | result | [Matrix](page.php?p=3329) | The target matrix
---

###static PerspectiveLH(width, height, znear, zfar) &rarr; [Matrix](page.php?p=3329)
Creates a left-handed perspective projection matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | width | number | The width of the view volume at the near view plane
 | height | number | The height of the view volume at the near view plane
 | znear | number | The z value of the near view plane
 | zfar | number | The z value of the far view place
---

###static PerspectiveFovLH(fov, aspect, znear, zfar) &rarr; [Matrix](page.php?p=3329)
Creates a left-handed perspective projection matrix based on the field of view

####Parameters
 | Name | Type | Description
---|---|---|---
 | fov | number | Field of view in the y direction, in radians.
 | aspect | number | Aspect ratio, defined as the view space width divided by height.
 | znear | number | Z-value of the near view plane.
 | zfar | number | Z-value of the far view plane.
---

###static PerspectiveFovLHToRef(fov, aspect, znear, zfar, result) &rarr; void
Creates a left-handed perspective projection matrix based on the field of view and put it into the target matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | fov | number | Field of view in the y direction, in radians.
 | aspect | number | Aspect ratio, defined as the view space width divided by height.
 | znear | number | Z-value of the near view plane.
 | zfar | number | Z-value of the far view plane.
 | result | [Matrix](page.php?p=3329) | The target matrix
---

###static GetFinalMatrix(viewport, world, view, projection, zmin, zmax) &rarr; [Matrix](page.php?p=3329)
??

####Parameters
 | Name | Type | Description
---|---|---|---
 | viewport | [Viewport](page.php?p=3331) | The [Viewport](page.php?p=3331) structure representing the viewport
 | world | [Matrix](page.php?p=3329) | The [Matrix](page.php?p=3329) structure representing the world
 | view | [Matrix](page.php?p=3329) | The [Matrix](page.php?p=3329) structure representing the view
 | projection | [Matrix](page.php?p=3329) | The [Matrix](page.php?p=3329) structure representing the projection
 | zmin | number | The minumum z value of the viewport
 | zmax | number | The maximum z value of the viewport
---

###static Transpose(matrix) &rarr; [Matrix](page.php?p=3329)
Transposes the rows and the columns of the given matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | matrix | [Matrix](page.php?p=3329) | The matrix to transpose
---

###static Reflection(plane) &rarr; [Matrix](page.php?p=3329)
Creates the reflection matrix of a given [Plane](page.php?p=3330)

####Parameters
 | Name | Type | Description
---|---|---|---
 | plane | [Plane](page.php?p=3330) | The given plane
---

###static ReflectionToRef(plane, result) &rarr; void
Creates the reflection matrix of a given [Plane](page.php?p=3330) and put it into a target matrix

####Parameters
 | Name | Type | Description
---|---|---|---
 | plane | [Plane](page.php?p=3330) | The given plane
 | result | [Matrix](page.php?p=3329) | the target matrix
---