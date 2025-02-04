:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the ConvexPolygonShape.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_ConvexPolygonShape:

ConvexPolygonShape
==================

**Inherits:** :ref:`Shape<class_Shape>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

用于3D物理的凸多边形形状。

描述
----

凸多边形形状资源，可以添加到\ :ref:`PhysicsBody<class_PhysicsBody>`\ 或area区域。

教程
----

- `3D Physics Tests Demo <https://godotengine.org/asset-library/asset/675>`__

属性
----

+-------------------------------------------------+---------------------------------------------------------+--------------------------+
| :ref:`PoolVector3Array<class_PoolVector3Array>` | :ref:`points<class_ConvexPolygonShape_property_points>` | ``PoolVector3Array(  )`` |
+-------------------------------------------------+---------------------------------------------------------+--------------------------+

属性说明
--------

.. _class_ConvexPolygonShape_property_points:

- :ref:`PoolVector3Array<class_PoolVector3Array>` **points**

+-----------+--------------------------+
| *Default* | ``PoolVector3Array(  )`` |
+-----------+--------------------------+
| *Setter*  | set_points(value)        |
+-----------+--------------------------+
| *Getter*  | get_points()             |
+-----------+--------------------------+

形成凸多边形的3D点列表。

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
