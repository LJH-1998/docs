page_type: reference
<style>{% include "site-assets/css/style.css" %}</style>

<!-- DO NOT EDIT! Automatically generated file. -->

# tf.keras.constraints.UnitNorm


<table class="tfo-notebook-buttons tfo-api" align="left">

<td>
  <a target="_blank" href="/api_docs/python/tf/keras/constraints/UnitNorm">
  <img src="https://www.tensorflow.org/images/tf_logo_32px.png" />
  TensorFlow 2 version</a>
</td>

<td>
  <a target="_blank" href="https://github.com/tensorflow/tensorflow/blob/r1.15/tensorflow/python/keras/constraints.py#L91-L118">
    <img src="https://www.tensorflow.org/images/GitHub-Mark-32px.png" />
    View source on GitHub
  </a>
</td></table>



## Class `UnitNorm`

Constrains the weights incident to each hidden unit to have unit norm.

Inherits From: [`Constraint`](../../../tf/keras/constraints/Constraint)

### Aliases:

* Class <a href="/api_docs/python/tf/keras/constraints/UnitNorm"><code>tf.compat.v1.keras.constraints.UnitNorm</code></a>
* Class <a href="/api_docs/python/tf/keras/constraints/UnitNorm"><code>tf.compat.v1.keras.constraints.unit_norm</code></a>
* Class <a href="/api_docs/python/tf/keras/constraints/UnitNorm"><code>tf.compat.v2.keras.constraints.UnitNorm</code></a>
* Class <a href="/api_docs/python/tf/keras/constraints/UnitNorm"><code>tf.compat.v2.keras.constraints.unit_norm</code></a>
* Class <a href="/api_docs/python/tf/keras/constraints/UnitNorm"><code>tf.keras.constraints.unit_norm</code></a>


<!-- Placeholder for "Used in" -->


#### Arguments:


* <b>`axis`</b>: integer, axis along which to calculate weight norms.
    For instance, in a `Dense` layer the weight matrix
    has shape `(input_dim, output_dim)`,
    set `axis` to `0` to constrain each weight vector
    of length `(input_dim,)`.
    In a `Conv2D` layer with `data_format="channels_last"`,
    the weight tensor has shape
    `(rows, cols, input_depth, output_depth)`,
    set `axis` to `[0, 1, 2]`
    to constrain the weights of each filter tensor of size
    `(rows, cols, input_depth)`.

<h2 id="__init__"><code>__init__</code></h2>

<a target="_blank" href="https://github.com/tensorflow/tensorflow/blob/r1.15/tensorflow/python/keras/constraints.py#L108-L109">View source</a>

``` python
__init__(axis=0)
```

Initialize self.  See help(type(self)) for accurate signature.




## Methods

<h3 id="__call__"><code>__call__</code></h3>

<a target="_blank" href="https://github.com/tensorflow/tensorflow/blob/r1.15/tensorflow/python/keras/constraints.py#L111-L115">View source</a>

``` python
__call__(w)
```

Call self as a function.


<h3 id="get_config"><code>get_config</code></h3>

<a target="_blank" href="https://github.com/tensorflow/tensorflow/blob/r1.15/tensorflow/python/keras/constraints.py#L117-L118">View source</a>

``` python
get_config()
```