<div itemscope itemtype="http://developers.google.com/ReferenceObject">
<meta itemprop="name" content="tfg.geometry.transformation.rotation_matrix_3d.is_valid" />
<meta itemprop="path" content="Stable" />
</div>

# tfg.geometry.transformation.rotation_matrix_3d.is_valid

<table class="tfo-notebook-buttons tfo-api" align="left">
</table>

<a target="_blank" href="https://github.com/tensorflow/graphics/blob/master/tensorflow_graphics/geometry/transformation/rotation_matrix_3d.py">View
source</a>

Determines if a matrix is a valid rotation matrix.

``` python
tfg.geometry.transformation.rotation_matrix_3d.is_valid(
    matrix,
    atol=0.001,
    name=None
)
```

<!-- Placeholder for "Used in" -->

#### Note:

In the following, A1 to An are optional batch dimensions.

#### Args:

* <b>`matrix`</b>: A tensor of shape `[A1, ..., An, 3,3]`, where the last two
  dimensions represent a matrix.
* <b>`atol`</b>: Absolute tolerance parameter.
* <b>`name`</b>: A name for this op that defaults to "rotation_matrix_3d_is_valid".


#### Returns:

A tensor of type `bool` and shape `[A1, ..., An, 1]` where False indicates that
the input is not a valid rotation matrix.
