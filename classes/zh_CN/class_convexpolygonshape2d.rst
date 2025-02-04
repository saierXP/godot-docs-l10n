:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the ConvexPolygonShape2D.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_ConvexPolygonShape2D:

ConvexPolygonShape2D
====================

**Inherits:** :ref:`Shape2D<class_Shape2D>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

用于2D物理的凸多边形形状。

描述
----

用于2D物理的凸多边形形状。凸多边形，无论其形状如何，都可以在内部分解为所需数量的凸多边形，以确保始终对凸多边形执行所有针对它的碰撞检查（检查速度更快）。

\ ``ConvexPolygonShape2D``\ 和\ :ref:`ConcavePolygonShape2D<class_ConcavePolygonShape2D>`\ 之间的主要区别在于，凹面多边形假定其为凹面，并使用更复杂的碰撞检测方法，而凸面多边形则将自身强制变为凸面，以加快碰撞检测的速度。

属性
----

+-------------------------------------------------+-----------------------------------------------------------+--------------------------+
| :ref:`PoolVector2Array<class_PoolVector2Array>` | :ref:`points<class_ConvexPolygonShape2D_property_points>` | ``PoolVector2Array(  )`` |
+-------------------------------------------------+-----------------------------------------------------------+--------------------------+

方法
----

+------+---------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`set_point_cloud<class_ConvexPolygonShape2D_method_set_point_cloud>` **(** :ref:`PoolVector2Array<class_PoolVector2Array>` point_cloud **)** |
+------+---------------------------------------------------------------------------------------------------------------------------------------------------+

属性说明
--------

.. _class_ConvexPolygonShape2D_property_points:

- :ref:`PoolVector2Array<class_PoolVector2Array>` **points**

+-----------+--------------------------+
| *Default* | ``PoolVector2Array(  )`` |
+-----------+--------------------------+
| *Setter*  | set_points(value)        |
+-----------+--------------------------+
| *Getter*  | get_points()             |
+-----------+--------------------------+

多边形的顶点列表。可以按顺时针或逆时针顺序。

方法说明
--------

.. _class_ConvexPolygonShape2D_method_set_point_cloud:

- void **set_point_cloud** **(** :ref:`PoolVector2Array<class_PoolVector2Array>` point_cloud **)**

基于所提供点的集合，使用凸包算法创建和分配 :ref:`points<class_ConvexPolygonShape2D_property_points>`\ 属性。删除所有不需要的点。参阅\ :ref:`Geometry.convex_hull_2d<class_Geometry_method_convex_hull_2d>`\ 。

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
