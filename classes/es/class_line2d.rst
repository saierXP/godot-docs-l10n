:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the Line2D.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_Line2D:

Line2D
======

**Inherits:** :ref:`Node2D<class_Node2D>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

Una línea 2D.

Descripción
----------------------

A line through several points in 2D space.

\ **Note:** By default, Godot can only draw up to 4,096 polygon points at a time. To increase this limit, open the Project Settings and increase :ref:`ProjectSettings.rendering/limits/buffers/canvas_polygon_buffer_size_kb<class_ProjectSettings_property_rendering/limits/buffers/canvas_polygon_buffer_size_kb>` and :ref:`ProjectSettings.rendering/limits/buffers/canvas_polygon_index_buffer_size_kb<class_ProjectSettings_property_rendering/limits/buffers/canvas_polygon_index_buffer_size_kb>`.

Tutoriales
--------------------

- `Matrix Transform Demo <https://godotengine.org/asset-library/asset/584>`__

- `2.5D Demo <https://godotengine.org/asset-library/asset/583>`__

Propiedades
----------------------

+-----------------------------------------------------+---------------------------------------------------------------+-----------------------------+
| :ref:`bool<class_bool>`                             | :ref:`antialiased<class_Line2D_property_antialiased>`         | ``false``                   |
+-----------------------------------------------------+---------------------------------------------------------------+-----------------------------+
| :ref:`LineCapMode<enum_Line2D_LineCapMode>`         | :ref:`begin_cap_mode<class_Line2D_property_begin_cap_mode>`   | ``0``                       |
+-----------------------------------------------------+---------------------------------------------------------------+-----------------------------+
| :ref:`Color<class_Color>`                           | :ref:`default_color<class_Line2D_property_default_color>`     | ``Color( 0.4, 0.5, 1, 1 )`` |
+-----------------------------------------------------+---------------------------------------------------------------+-----------------------------+
| :ref:`LineCapMode<enum_Line2D_LineCapMode>`         | :ref:`end_cap_mode<class_Line2D_property_end_cap_mode>`       | ``0``                       |
+-----------------------------------------------------+---------------------------------------------------------------+-----------------------------+
| :ref:`Gradient<class_Gradient>`                     | :ref:`gradient<class_Line2D_property_gradient>`               |                             |
+-----------------------------------------------------+---------------------------------------------------------------+-----------------------------+
| :ref:`LineJointMode<enum_Line2D_LineJointMode>`     | :ref:`joint_mode<class_Line2D_property_joint_mode>`           | ``0``                       |
+-----------------------------------------------------+---------------------------------------------------------------+-----------------------------+
| :ref:`PoolVector2Array<class_PoolVector2Array>`     | :ref:`points<class_Line2D_property_points>`                   | ``PoolVector2Array(  )``    |
+-----------------------------------------------------+---------------------------------------------------------------+-----------------------------+
| :ref:`int<class_int>`                               | :ref:`round_precision<class_Line2D_property_round_precision>` | ``8``                       |
+-----------------------------------------------------+---------------------------------------------------------------+-----------------------------+
| :ref:`float<class_float>`                           | :ref:`sharp_limit<class_Line2D_property_sharp_limit>`         | ``2.0``                     |
+-----------------------------------------------------+---------------------------------------------------------------+-----------------------------+
| :ref:`Texture<class_Texture>`                       | :ref:`texture<class_Line2D_property_texture>`                 |                             |
+-----------------------------------------------------+---------------------------------------------------------------+-----------------------------+
| :ref:`LineTextureMode<enum_Line2D_LineTextureMode>` | :ref:`texture_mode<class_Line2D_property_texture_mode>`       | ``0``                       |
+-----------------------------------------------------+---------------------------------------------------------------+-----------------------------+
| :ref:`float<class_float>`                           | :ref:`width<class_Line2D_property_width>`                     | ``10.0``                    |
+-----------------------------------------------------+---------------------------------------------------------------+-----------------------------+
| :ref:`Curve<class_Curve>`                           | :ref:`width_curve<class_Line2D_property_width_curve>`         |                             |
+-----------------------------------------------------+---------------------------------------------------------------+-----------------------------+

Métodos
--------------

+-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`add_point<class_Line2D_method_add_point>` **(** :ref:`Vector2<class_Vector2>` position, :ref:`int<class_int>` at_position=-1 **)**      |
+-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`clear_points<class_Line2D_method_clear_points>` **(** **)**                                                                             |
+-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`         | :ref:`get_point_count<class_Line2D_method_get_point_count>` **(** **)** |const|                                                               |
+-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>` | :ref:`get_point_position<class_Line2D_method_get_point_position>` **(** :ref:`int<class_int>` i **)** |const|                                 |
+-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`remove_point<class_Line2D_method_remove_point>` **(** :ref:`int<class_int>` i **)**                                                     |
+-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`set_point_position<class_Line2D_method_set_point_position>` **(** :ref:`int<class_int>` i, :ref:`Vector2<class_Vector2>` position **)** |
+-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+

Enumeraciones
--------------------------

.. _enum_Line2D_LineJointMode:

.. _class_Line2D_constant_LINE_JOINT_SHARP:

.. _class_Line2D_constant_LINE_JOINT_BEVEL:

.. _class_Line2D_constant_LINE_JOINT_ROUND:

enum **LineJointMode**:

- **LINE_JOINT_SHARP** = **0** --- Las articulaciones de la línea serán puntiagudas. Si ``sharp_limit`` es mayor que la rotación de una articulación, se convierte en una articulación en bisel en su lugar.

- **LINE_JOINT_BEVEL** = **1** --- Las uniones de la línea serán biseladas/chamfered.

- **LINE_JOINT_ROUND** = **2** --- Las articulaciones de la línea serán redondeadas.

----

.. _enum_Line2D_LineCapMode:

.. _class_Line2D_constant_LINE_CAP_NONE:

.. _class_Line2D_constant_LINE_CAP_BOX:

.. _class_Line2D_constant_LINE_CAP_ROUND:

enum **LineCapMode**:

- **LINE_CAP_NONE** = **0** --- No dibujes una cubierta de línea.

- **LINE_CAP_BOX** = **1** --- Dibuja la cubierta de la línea como una caja.

- **LINE_CAP_ROUND** = **2** --- Dibuja la cubierta de la línea como un círculo.

----

.. _enum_Line2D_LineTextureMode:

.. _class_Line2D_constant_LINE_TEXTURE_NONE:

.. _class_Line2D_constant_LINE_TEXTURE_TILE:

.. _class_Line2D_constant_LINE_TEXTURE_STRETCH:

enum **LineTextureMode**:

- **LINE_TEXTURE_NONE** = **0** --- Toma los píxeles izquierdos de la textura y la renderiza sobre toda la línea.

- **LINE_TEXTURE_TILE** = **1** --- Tesela la textura sobre la línea. La textura debe ser importada con **Repeat** habilitado para que funcione correctamente.

- **LINE_TEXTURE_STRETCH** = **2** --- Estira la textura a través de la línea. Importa la textura con **Repeat** desactivado para obtener mejores resultados.

Descripciones de Propiedades
--------------------------------------------------------

.. _class_Line2D_property_antialiased:

- :ref:`bool<class_bool>` **antialiased**

+-----------+------------------------+
| *Default* | ``false``              |
+-----------+------------------------+
| *Setter*  | set_antialiased(value) |
+-----------+------------------------+
| *Getter*  | get_antialiased()      |
+-----------+------------------------+

If ``true``, the line's border will be anti-aliased.

\ **Note:** Line2D is not accelerated by batching when being anti-aliased.

----

.. _class_Line2D_property_begin_cap_mode:

- :ref:`LineCapMode<enum_Line2D_LineCapMode>` **begin_cap_mode**

+-----------+---------------------------+
| *Default* | ``0``                     |
+-----------+---------------------------+
| *Setter*  | set_begin_cap_mode(value) |
+-----------+---------------------------+
| *Getter*  | get_begin_cap_mode()      |
+-----------+---------------------------+

Controla el estilo del primer punto de la línea. Usa las constantes :ref:`LineCapMode<enum_Line2D_LineCapMode>`.

----

.. _class_Line2D_property_default_color:

- :ref:`Color<class_Color>` **default_color**

+-----------+-----------------------------+
| *Default* | ``Color( 0.4, 0.5, 1, 1 )`` |
+-----------+-----------------------------+
| *Setter*  | set_default_color(value)    |
+-----------+-----------------------------+
| *Getter*  | get_default_color()         |
+-----------+-----------------------------+

El color de la línea. No se usará si se establece un gradiente.

----

.. _class_Line2D_property_end_cap_mode:

- :ref:`LineCapMode<enum_Line2D_LineCapMode>` **end_cap_mode**

+-----------+-------------------------+
| *Default* | ``0``                   |
+-----------+-------------------------+
| *Setter*  | set_end_cap_mode(value) |
+-----------+-------------------------+
| *Getter*  | get_end_cap_mode()      |
+-----------+-------------------------+

Controla el estilo del último punto de la línea. Usa las constantes :ref:`LineCapMode<enum_Line2D_LineCapMode>`.

----

.. _class_Line2D_property_gradient:

- :ref:`Gradient<class_Gradient>` **gradient**

+----------+---------------------+
| *Setter* | set_gradient(value) |
+----------+---------------------+
| *Getter* | get_gradient()      |
+----------+---------------------+

El gradiente se dibuja a través de toda la línea de principio a fin. El color por defecto no se usará si se establece un gradiente.

----

.. _class_Line2D_property_joint_mode:

- :ref:`LineJointMode<enum_Line2D_LineJointMode>` **joint_mode**

+-----------+-----------------------+
| *Default* | ``0``                 |
+-----------+-----------------------+
| *Setter*  | set_joint_mode(value) |
+-----------+-----------------------+
| *Getter*  | get_joint_mode()      |
+-----------+-----------------------+

El estilo de los puntos entre el comienzo y el final.

----

.. _class_Line2D_property_points:

- :ref:`PoolVector2Array<class_PoolVector2Array>` **points**

+-----------+--------------------------+
| *Default* | ``PoolVector2Array(  )`` |
+-----------+--------------------------+
| *Setter*  | set_points(value)        |
+-----------+--------------------------+
| *Getter*  | get_points()             |
+-----------+--------------------------+

The points that form the lines. The line is drawn between every point set in this array. Points are interpreted as local vectors.

----

.. _class_Line2D_property_round_precision:

- :ref:`int<class_int>` **round_precision**

+-----------+----------------------------+
| *Default* | ``8``                      |
+-----------+----------------------------+
| *Setter*  | set_round_precision(value) |
+-----------+----------------------------+
| *Getter*  | get_round_precision()      |
+-----------+----------------------------+

La suavidad de las articulaciones redondeadas y las cubiertas. Esto sólo se usa si una cubierta o articulación se establece como redonda.

----

.. _class_Line2D_property_sharp_limit:

- :ref:`float<class_float>` **sharp_limit**

+-----------+------------------------+
| *Default* | ``2.0``                |
+-----------+------------------------+
| *Setter*  | set_sharp_limit(value) |
+-----------+------------------------+
| *Getter*  | get_sharp_limit()      |
+-----------+------------------------+

The direction difference in radians between vector points. This value is only used if :ref:`joint_mode<class_Line2D_property_joint_mode>` is set to :ref:`LINE_JOINT_SHARP<class_Line2D_constant_LINE_JOINT_SHARP>`.

----

.. _class_Line2D_property_texture:

- :ref:`Texture<class_Texture>` **texture**

+----------+--------------------+
| *Setter* | set_texture(value) |
+----------+--------------------+
| *Getter* | get_texture()      |
+----------+--------------------+

La textura usada para la textura de la línea. Utiliza ``texture_mode`` para el estilo de dibujo.

----

.. _class_Line2D_property_texture_mode:

- :ref:`LineTextureMode<enum_Line2D_LineTextureMode>` **texture_mode**

+-----------+-------------------------+
| *Default* | ``0``                   |
+-----------+-------------------------+
| *Setter*  | set_texture_mode(value) |
+-----------+-------------------------+
| *Getter*  | get_texture_mode()      |
+-----------+-------------------------+

El estilo para renderizar la ``texture`` en la línea. Usa las constantes de :ref:`LineTextureMode<enum_Line2D_LineTextureMode>`.

----

.. _class_Line2D_property_width:

- :ref:`float<class_float>` **width**

+-----------+------------------+
| *Default* | ``10.0``         |
+-----------+------------------+
| *Setter*  | set_width(value) |
+-----------+------------------+
| *Getter*  | get_width()      |
+-----------+------------------+

El ancho de la línea.

----

.. _class_Line2D_property_width_curve:

- :ref:`Curve<class_Curve>` **width_curve**

+----------+------------------+
| *Setter* | set_curve(value) |
+----------+------------------+
| *Getter* | get_curve()      |
+----------+------------------+

El ancho de la línea varía con la curva. El ancho original simplemente se multiplica por el valor de la curva.

Descripciones de Métodos
------------------------------------------------

.. _class_Line2D_method_add_point:

- void **add_point** **(** :ref:`Vector2<class_Vector2>` position, :ref:`int<class_int>` at_position=-1 **)**

Añade un punto en la ``position``. Añade el punto al final de la línea.

Si se da ``at_position``, el punto se inserta antes del número de punto ``at_position``, desplazando ese punto (y todos los puntos posteriores) después del punto insertado. Si no se da ``at_position``, o es un valor ilegal (``at_position < 0`` o ``at_position >= [method get_point_count]``), el punto se añadirá al final de la lista de puntos.

----

.. _class_Line2D_method_clear_points:

- void **clear_points** **(** **)**

Elimina todos los puntos de la línea.

----

.. _class_Line2D_method_get_point_count:

- :ref:`int<class_int>` **get_point_count** **(** **)** |const|

Devuelve la cantidad de puntos de Line2D.

----

.. _class_Line2D_method_get_point_position:

- :ref:`Vector2<class_Vector2>` **get_point_position** **(** :ref:`int<class_int>` i **)** |const|

Devuelve la posición del punto ``i``.

----

.. _class_Line2D_method_remove_point:

- void **remove_point** **(** :ref:`int<class_int>` i **)**

Elimina el punto en el índice ``i`` de la línea.

----

.. _class_Line2D_method_set_point_position:

- void **set_point_position** **(** :ref:`int<class_int>` i, :ref:`Vector2<class_Vector2>` position **)**

Sobrescribe la posición en el punto ``i`` con la ``position`` suministrada.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
