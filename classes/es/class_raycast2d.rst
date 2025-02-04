:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the RayCast2D.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_RayCast2D:

RayCast2D
=========

**Inherits:** :ref:`Node2D<class_Node2D>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

Busca el objeto más cercano que intersecta un rayo.

Descripción
----------------------

Un RayCast representa una línea desde su origen hasta su posición de destino, ``cast_to``. Se utiliza para consultar el espacio 2D con el fin de encontrar el objeto más cercano a lo largo de la trayectoria del rayo.

RayCast2D puede ignorar algunos objetos añadiéndolos a la lista de excepciones mediante ``add_exception``, estableciendo un filtrado adecuado con las capas de colisión, o filtrando los tipos de objetos con máscaras de tipo.

RayCast2D puede ser configurado para reportar colisiones con :ref:`Area2D<class_Area2D>`\ s (:ref:`collide_with_areas<class_RayCast2D_property_collide_with_areas>`) y/o :ref:`PhysicsBody2D<class_PhysicsBody2D>`\ s (:ref:`collide_with_bodies<class_RayCast2D_property_collide_with_bodies>`).

Sólo las emisiones de rayos habilitadas podrán consultar el espacio e informar de las colisiones.

RayCast2D calcula la intersección de cada cuadro de física (ver :ref:`Node<class_Node>`), y el resultado se almacena en caché para poder ser utilizado más tarde hasta el siguiente cuadro. Si se requieren múltiples consultas entre marcos físicos (o durante el mismo marco) utilice :ref:`force_raycast_update<class_RayCast2D_method_force_raycast_update>` después de ajustar el raycast.

Tutoriales
--------------------

- :doc:`../tutorials/physics/ray-casting`

Propiedades
----------------------

+-------------------------------+--------------------------------------------------------------------------+----------------------+
| :ref:`Vector2<class_Vector2>` | :ref:`cast_to<class_RayCast2D_property_cast_to>`                         | ``Vector2( 0, 50 )`` |
+-------------------------------+--------------------------------------------------------------------------+----------------------+
| :ref:`bool<class_bool>`       | :ref:`collide_with_areas<class_RayCast2D_property_collide_with_areas>`   | ``false``            |
+-------------------------------+--------------------------------------------------------------------------+----------------------+
| :ref:`bool<class_bool>`       | :ref:`collide_with_bodies<class_RayCast2D_property_collide_with_bodies>` | ``true``             |
+-------------------------------+--------------------------------------------------------------------------+----------------------+
| :ref:`int<class_int>`         | :ref:`collision_mask<class_RayCast2D_property_collision_mask>`           | ``1``                |
+-------------------------------+--------------------------------------------------------------------------+----------------------+
| :ref:`bool<class_bool>`       | :ref:`enabled<class_RayCast2D_property_enabled>`                         | ``false``            |
+-------------------------------+--------------------------------------------------------------------------+----------------------+
| :ref:`bool<class_bool>`       | :ref:`exclude_parent<class_RayCast2D_property_exclude_parent>`           | ``true``             |
+-------------------------------+--------------------------------------------------------------------------+----------------------+

Métodos
--------------

+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`add_exception<class_RayCast2D_method_add_exception>` **(** :ref:`Object<class_Object>` node **)**                                           |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`add_exception_rid<class_RayCast2D_method_add_exception_rid>` **(** :ref:`RID<class_RID>` rid **)**                                          |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`clear_exceptions<class_RayCast2D_method_clear_exceptions>` **(** **)**                                                                      |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`force_raycast_update<class_RayCast2D_method_force_raycast_update>` **(** **)**                                                              |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Object<class_Object>`   | :ref:`get_collider<class_RayCast2D_method_get_collider>` **(** **)** |const|                                                                      |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`         | :ref:`get_collider_shape<class_RayCast2D_method_get_collider_shape>` **(** **)** |const|                                                          |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`get_collision_mask_bit<class_RayCast2D_method_get_collision_mask_bit>` **(** :ref:`int<class_int>` bit **)** |const|                        |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>` | :ref:`get_collision_normal<class_RayCast2D_method_get_collision_normal>` **(** **)** |const|                                                      |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>` | :ref:`get_collision_point<class_RayCast2D_method_get_collision_point>` **(** **)** |const|                                                        |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`is_colliding<class_RayCast2D_method_is_colliding>` **(** **)** |const|                                                                      |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`remove_exception<class_RayCast2D_method_remove_exception>` **(** :ref:`Object<class_Object>` node **)**                                     |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`remove_exception_rid<class_RayCast2D_method_remove_exception_rid>` **(** :ref:`RID<class_RID>` rid **)**                                    |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`set_collision_mask_bit<class_RayCast2D_method_set_collision_mask_bit>` **(** :ref:`int<class_int>` bit, :ref:`bool<class_bool>` value **)** |
+-------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------+

Descripciones de Propiedades
--------------------------------------------------------

.. _class_RayCast2D_property_cast_to:

- :ref:`Vector2<class_Vector2>` **cast_to**

+-----------+----------------------+
| *Default* | ``Vector2( 0, 50 )`` |
+-----------+----------------------+
| *Setter*  | set_cast_to(value)   |
+-----------+----------------------+
| *Getter*  | get_cast_to()        |
+-----------+----------------------+

El punto de destino del rayo, relativo a la ``position`` del RayCast.

----

.. _class_RayCast2D_property_collide_with_areas:

- :ref:`bool<class_bool>` **collide_with_areas**

+-----------+---------------------------------+
| *Default* | ``false``                       |
+-----------+---------------------------------+
| *Setter*  | set_collide_with_areas(value)   |
+-----------+---------------------------------+
| *Getter*  | is_collide_with_areas_enabled() |
+-----------+---------------------------------+

Si ``true``, se informará de la colisión con :ref:`Area2D<class_Area2D>`\ s.

----

.. _class_RayCast2D_property_collide_with_bodies:

- :ref:`bool<class_bool>` **collide_with_bodies**

+-----------+----------------------------------+
| *Default* | ``true``                         |
+-----------+----------------------------------+
| *Setter*  | set_collide_with_bodies(value)   |
+-----------+----------------------------------+
| *Getter*  | is_collide_with_bodies_enabled() |
+-----------+----------------------------------+

Si ``true``, se informará de la colisión con :ref:`PhysicsBody2D<class_PhysicsBody2D>`.

----

.. _class_RayCast2D_property_collision_mask:

- :ref:`int<class_int>` **collision_mask**

+-----------+---------------------------+
| *Default* | ``1``                     |
+-----------+---------------------------+
| *Setter*  | set_collision_mask(value) |
+-----------+---------------------------+
| *Getter*  | get_collision_mask()      |
+-----------+---------------------------+

The ray's collision mask. Only objects in at least one collision layer enabled in the mask will be detected. See `Collision layers and masks <../tutorials/physics/physics_introduction.html#collision-layers-and-masks>`__ in the documentation for more information.

----

.. _class_RayCast2D_property_enabled:

- :ref:`bool<class_bool>` **enabled**

+-----------+--------------------+
| *Default* | ``false``          |
+-----------+--------------------+
| *Setter*  | set_enabled(value) |
+-----------+--------------------+
| *Getter*  | is_enabled()       |
+-----------+--------------------+

Si ``true``, se informará de las colisiones.

----

.. _class_RayCast2D_property_exclude_parent:

- :ref:`bool<class_bool>` **exclude_parent**

+-----------+--------------------------------+
| *Default* | ``true``                       |
+-----------+--------------------------------+
| *Setter*  | set_exclude_parent_body(value) |
+-----------+--------------------------------+
| *Getter*  | get_exclude_parent_body()      |
+-----------+--------------------------------+

Si ``true``, el nodo padre será excluido de la detección de colisiones.

Descripciones de Métodos
------------------------------------------------

.. _class_RayCast2D_method_add_exception:

- void **add_exception** **(** :ref:`Object<class_Object>` node **)**

Añade una excepción de colisión para que el rayo no informe de las colisiones con el nodo especificado.

----

.. _class_RayCast2D_method_add_exception_rid:

- void **add_exception_rid** **(** :ref:`RID<class_RID>` rid **)**

Añade una excepción de colisión para que el rayo no reporte colisiones con el :ref:`RID<class_RID>` especificado.

----

.. _class_RayCast2D_method_clear_exceptions:

- void **clear_exceptions** **(** **)**

Elimina todas las excepciones de colisión para este rayo.

----

.. _class_RayCast2D_method_force_raycast_update:

- void **force_raycast_update** **(** **)**

Updates the collision information for the ray. Use this method to update the collision information immediately instead of waiting for the next ``_physics_process`` call, for example if the ray or its parent has changed state.

\ **Note:** ``enabled`` is not required for this to work.

----

.. _class_RayCast2D_method_get_collider:

- :ref:`Object<class_Object>` **get_collider** **(** **)** |const|

Devuelve el primer objeto que el rayo intersecta, o ``null`` si no hay ningún objeto que intersecte el rayo (es decir, :ref:`is_colliding<class_RayCast2D_method_is_colliding>` devuelve ``false``).

----

.. _class_RayCast2D_method_get_collider_shape:

- :ref:`int<class_int>` **get_collider_shape** **(** **)** |const|

Devuelve el ID de la forma del primer objeto que el rayo intersecta, o ``0`` si no hay ningún objeto que intersecte el rayo (es decir, :ref:`is_colliding<class_RayCast2D_method_is_colliding>` devuelve ``false``).

----

.. _class_RayCast2D_method_get_collision_mask_bit:

- :ref:`bool<class_bool>` **get_collision_mask_bit** **(** :ref:`int<class_int>` bit **)** |const|

Devuelve un bit individual de la máscara de colisión.

----

.. _class_RayCast2D_method_get_collision_normal:

- :ref:`Vector2<class_Vector2>` **get_collision_normal** **(** **)** |const|

Devuelve la normalidad de la forma del objeto que se intersecta en el punto de colisión.

----

.. _class_RayCast2D_method_get_collision_point:

- :ref:`Vector2<class_Vector2>` **get_collision_point** **(** **)** |const|

Devuelve el punto de colisión en el que el rayo intersecta el objeto más cercano.

\ **Nota:** Este punto está en el sistema de coordenadas **global**.

----

.. _class_RayCast2D_method_is_colliding:

- :ref:`bool<class_bool>` **is_colliding** **(** **)** |const|

Devuelve si algún objeto se cruza con el vector del rayo (considerando la longitud del vector).

----

.. _class_RayCast2D_method_remove_exception:

- void **remove_exception** **(** :ref:`Object<class_Object>` node **)**

Elimina una excepción de colisión para que el rayo informe de las colisiones con el nodo especificado.

----

.. _class_RayCast2D_method_remove_exception_rid:

- void **remove_exception_rid** **(** :ref:`RID<class_RID>` rid **)**

Elimina una excepción de colisión para que el rayo reporte colisiones con el :ref:`RID<class_RID>` especificado.

----

.. _class_RayCast2D_method_set_collision_mask_bit:

- void **set_collision_mask_bit** **(** :ref:`int<class_int>` bit, :ref:`bool<class_bool>` value **)**

Establece o borra bits individuales en la máscara de colisión. Esto hace que la selección de las áreas escaneadas sea más fácil.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
