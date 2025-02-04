:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the VisualShaderNodeUniform.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_VisualShaderNodeUniform:

VisualShaderNodeUniform
=======================

**Inherits:** :ref:`VisualShaderNode<class_VisualShaderNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`VisualShaderNodeBooleanUniform<class_VisualShaderNodeBooleanUniform>`, :ref:`VisualShaderNodeColorUniform<class_VisualShaderNodeColorUniform>`, :ref:`VisualShaderNodeScalarUniform<class_VisualShaderNodeScalarUniform>`, :ref:`VisualShaderNodeTextureUniform<class_VisualShaderNodeTextureUniform>`, :ref:`VisualShaderNodeTransformUniform<class_VisualShaderNodeTransformUniform>`, :ref:`VisualShaderNodeVec3Uniform<class_VisualShaderNodeVec3Uniform>`

可视化着色器图中的uniforms的基本类型。

描述
----

uniform表示着色器中的一个变量，它是由外部设置的，即从\ :ref:`ShaderMaterial<class_ShaderMaterial>`\ 中设置。uniform在\ :ref:`ShaderMaterial<class_ShaderMaterial>`\ 中被暴露为属性，可以从检查器或脚本中分配。

属性
----

+-----------------------------+--------------------------------------------------------------------------+--------+
| :ref:`String<class_String>` | :ref:`uniform_name<class_VisualShaderNodeUniform_property_uniform_name>` | ``""`` |
+-----------------------------+--------------------------------------------------------------------------+--------+

属性说明
--------

.. _class_VisualShaderNodeUniform_property_uniform_name:

- :ref:`String<class_String>` **uniform_name**

+-----------+-------------------------+
| *Default* | ``""``                  |
+-----------+-------------------------+
| *Setter*  | set_uniform_name(value) |
+-----------+-------------------------+
| *Getter*  | get_uniform_name()      |
+-----------+-------------------------+

uniform的名称，可以通过\ :ref:`ShaderMaterial<class_ShaderMaterial>`\ 属性访问它。

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
