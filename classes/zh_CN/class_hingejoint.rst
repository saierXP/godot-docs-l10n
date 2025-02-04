:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the HingeJoint.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_HingeJoint:

HingeJoint
==========

**Inherits:** :ref:`Joint<class_Joint>` **<** :ref:`Spatial<class_Spatial>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

两个 3D PhysicsBody 之间的铰链。

描述
----

HingeJoint（铰链关节）通常使用物体 A 的 Z 轴作为铰链轴，但手动添加时可以指定另一个轴。请参阅 :ref:`Generic6DOFJoint<class_Generic6DOFJoint>`\ 。

属性
----

+---------------------------+-------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>` | :ref:`angular_limit/bias<class_HingeJoint_property_angular_limit/bias>`             | ``0.3``   |
+---------------------------+-------------------------------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>`   | :ref:`angular_limit/enable<class_HingeJoint_property_angular_limit/enable>`         | ``false`` |
+---------------------------+-------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>` | :ref:`angular_limit/lower<class_HingeJoint_property_angular_limit/lower>`           | ``-90.0`` |
+---------------------------+-------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>` | :ref:`angular_limit/relaxation<class_HingeJoint_property_angular_limit/relaxation>` | ``1.0``   |
+---------------------------+-------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>` | :ref:`angular_limit/softness<class_HingeJoint_property_angular_limit/softness>`     | ``0.9``   |
+---------------------------+-------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>` | :ref:`angular_limit/upper<class_HingeJoint_property_angular_limit/upper>`           | ``90.0``  |
+---------------------------+-------------------------------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>`   | :ref:`motor/enable<class_HingeJoint_property_motor/enable>`                         | ``false`` |
+---------------------------+-------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>` | :ref:`motor/max_impulse<class_HingeJoint_property_motor/max_impulse>`               | ``1.0``   |
+---------------------------+-------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>` | :ref:`motor/target_velocity<class_HingeJoint_property_motor/target_velocity>`       | ``1.0``   |
+---------------------------+-------------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>` | :ref:`params/bias<class_HingeJoint_property_params/bias>`                           | ``0.3``   |
+---------------------------+-------------------------------------------------------------------------------------+-----------+

方法
----

+---------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`   | :ref:`get_flag<class_HingeJoint_method_get_flag>` **(** :ref:`Flag<enum_HingeJoint_Flag>` flag **)** |const|                               |
+---------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`get_param<class_HingeJoint_method_get_param>` **(** :ref:`Param<enum_HingeJoint_Param>` param **)** |const|                          |
+---------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| void                      | :ref:`set_flag<class_HingeJoint_method_set_flag>` **(** :ref:`Flag<enum_HingeJoint_Flag>` flag, :ref:`bool<class_bool>` enabled **)**      |
+---------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
| void                      | :ref:`set_param<class_HingeJoint_method_set_param>` **(** :ref:`Param<enum_HingeJoint_Param>` param, :ref:`float<class_float>` value **)** |
+---------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+

枚举
----

.. _enum_HingeJoint_Param:

.. _class_HingeJoint_constant_PARAM_BIAS:

.. _class_HingeJoint_constant_PARAM_LIMIT_UPPER:

.. _class_HingeJoint_constant_PARAM_LIMIT_LOWER:

.. _class_HingeJoint_constant_PARAM_LIMIT_BIAS:

.. _class_HingeJoint_constant_PARAM_LIMIT_SOFTNESS:

.. _class_HingeJoint_constant_PARAM_LIMIT_RELAXATION:

.. _class_HingeJoint_constant_PARAM_MOTOR_TARGET_VELOCITY:

.. _class_HingeJoint_constant_PARAM_MOTOR_MAX_IMPULSE:

.. _class_HingeJoint_constant_PARAM_MAX:

enum **Param**:

- **PARAM_BIAS** = **0** --- 两个物体向不同方向移动时被拉回到一起的速度。

- **PARAM_LIMIT_UPPER** = **1** --- 最大的旋转量。只有在\ :ref:`angular_limit/enable<class_HingeJoint_property_angular_limit/enable>`\ 为\ ``true``\ 时才有效。

- **PARAM_LIMIT_LOWER** = **2** --- 最小的旋转量。只有在\ :ref:`angular_limit/enable<class_HingeJoint_property_angular_limit/enable>`\ 为\ ``true``\ 时才有效。

- **PARAM_LIMIT_BIAS** = **3** --- 垂直于铰链的轴线上的旋转得到纠正的速度。

- **PARAM_LIMIT_SOFTNESS** = **4**

- **PARAM_LIMIT_RELAXATION** = **5** --- 该值越低，旋转速度越慢。

- **PARAM_MOTOR_TARGET_VELOCITY** = **6** --- 目标马达的目标速度。

- **PARAM_MOTOR_MAX_IMPULSE** = **7** --- 马达的最大加速度。

- **PARAM_MAX** = **8** --- 表示 :ref:`Param<enum_HingeJoint_Param>` 枚举的大小。

----

.. _enum_HingeJoint_Flag:

.. _class_HingeJoint_constant_FLAG_USE_LIMIT:

.. _class_HingeJoint_constant_FLAG_ENABLE_MOTOR:

.. _class_HingeJoint_constant_FLAG_MAX:

enum **Flag**:

- **FLAG_USE_LIMIT** = **0** --- 如果为\ ``true``,则会对由\ :ref:`angular_limit/lower<class_HingeJoint_property_angular_limit/lower>`\ 和\ :ref:`angular_limit/upper<class_HingeJoint_property_angular_limit/upper>`\ 定义的铰链最大和最小旋转量产生影响。

- **FLAG_ENABLE_MOTOR** = **1** --- 激活后，电机会使铰链转动。

- **FLAG_MAX** = **2** --- 表示\ :ref:`Flag<enum_HingeJoint_Flag>`\ 枚举的大小。

属性说明
--------

.. _class_HingeJoint_property_angular_limit/bias:

- :ref:`float<class_float>` **angular_limit/bias**

+-----------+------------------+
| *Default* | ``0.3``          |
+-----------+------------------+
| *Setter*  | set_param(value) |
+-----------+------------------+
| *Getter*  | get_param()      |
+-----------+------------------+

垂直于铰链的轴线上的旋转得到纠正的速度。

----

.. _class_HingeJoint_property_angular_limit/enable:

- :ref:`bool<class_bool>` **angular_limit/enable**

+-----------+-----------------+
| *Default* | ``false``       |
+-----------+-----------------+
| *Setter*  | set_flag(value) |
+-----------+-----------------+
| *Getter*  | get_flag()      |
+-----------+-----------------+

如果为\ ``true``,则会对由\ :ref:`angular_limit/lower<class_HingeJoint_property_angular_limit/lower>`\ 和\ :ref:`angular_limit/upper<class_HingeJoint_property_angular_limit/upper>`\ 定义的铰链最大和最小旋转量产生影响。

----

.. _class_HingeJoint_property_angular_limit/lower:

- :ref:`float<class_float>` **angular_limit/lower**

+-----------+-----------+
| *Default* | ``-90.0`` |
+-----------+-----------+

最小的旋转量。只有在\ :ref:`angular_limit/enable<class_HingeJoint_property_angular_limit/enable>`\ 为\ ``true``\ 时才有效。

----

.. _class_HingeJoint_property_angular_limit/relaxation:

- :ref:`float<class_float>` **angular_limit/relaxation**

+-----------+------------------+
| *Default* | ``1.0``          |
+-----------+------------------+
| *Setter*  | set_param(value) |
+-----------+------------------+
| *Getter*  | get_param()      |
+-----------+------------------+

该值越低，旋转速度越慢。

----

.. _class_HingeJoint_property_angular_limit/softness:

- :ref:`float<class_float>` **angular_limit/softness**

+-----------+------------------+
| *Default* | ``0.9``          |
+-----------+------------------+
| *Setter*  | set_param(value) |
+-----------+------------------+
| *Getter*  | get_param()      |
+-----------+------------------+

----

.. _class_HingeJoint_property_angular_limit/upper:

- :ref:`float<class_float>` **angular_limit/upper**

+-----------+----------+
| *Default* | ``90.0`` |
+-----------+----------+

最大的旋转量。只有在\ :ref:`angular_limit/enable<class_HingeJoint_property_angular_limit/enable>`\ 为\ ``true``\ 时才有效。

----

.. _class_HingeJoint_property_motor/enable:

- :ref:`bool<class_bool>` **motor/enable**

+-----------+-----------------+
| *Default* | ``false``       |
+-----------+-----------------+
| *Setter*  | set_flag(value) |
+-----------+-----------------+
| *Getter*  | get_flag()      |
+-----------+-----------------+

激活后，电机会使铰链转动。

----

.. _class_HingeJoint_property_motor/max_impulse:

- :ref:`float<class_float>` **motor/max_impulse**

+-----------+------------------+
| *Default* | ``1.0``          |
+-----------+------------------+
| *Setter*  | set_param(value) |
+-----------+------------------+
| *Getter*  | get_param()      |
+-----------+------------------+

马达的最大加速度。

----

.. _class_HingeJoint_property_motor/target_velocity:

- :ref:`float<class_float>` **motor/target_velocity**

+-----------+------------------+
| *Default* | ``1.0``          |
+-----------+------------------+
| *Setter*  | set_param(value) |
+-----------+------------------+
| *Getter*  | get_param()      |
+-----------+------------------+

目标马达的目标速度。

----

.. _class_HingeJoint_property_params/bias:

- :ref:`float<class_float>` **params/bias**

+-----------+------------------+
| *Default* | ``0.3``          |
+-----------+------------------+
| *Setter*  | set_param(value) |
+-----------+------------------+
| *Getter*  | get_param()      |
+-----------+------------------+

两个物体向不同方向移动时被拉回到一起的速度。

方法说明
--------

.. _class_HingeJoint_method_get_flag:

- :ref:`bool<class_bool>` **get_flag** **(** :ref:`Flag<enum_HingeJoint_Flag>` flag **)** |const|

返回指定标志的值。

----

.. _class_HingeJoint_method_get_param:

- :ref:`float<class_float>` **get_param** **(** :ref:`Param<enum_HingeJoint_Param>` param **)** |const|

返回指定参数的值。

----

.. _class_HingeJoint_method_set_flag:

- void **set_flag** **(** :ref:`Flag<enum_HingeJoint_Flag>` flag, :ref:`bool<class_bool>` enabled **)**

如果为 ``true``\ ，启用指定的标志。

----

.. _class_HingeJoint_method_set_param:

- void **set_param** **(** :ref:`Param<enum_HingeJoint_Param>` param, :ref:`float<class_float>` value **)**

设置指定参数的值。

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
