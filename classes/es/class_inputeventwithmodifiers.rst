:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the InputEventWithModifiers.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_InputEventWithModifiers:

InputEventWithModifiers
=======================

**Inherits:** :ref:`InputEvent<class_InputEvent>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`InputEventGesture<class_InputEventGesture>`, :ref:`InputEventKey<class_InputEventKey>`, :ref:`InputEventMouse<class_InputEventMouse>`

Clase base para eventos clave con modificadores.

Descripción
----------------------

Contains keys events information with modifiers support like ``Shift`` or ``Alt``. See :ref:`Node._input<class_Node_method__input>`.

Tutoriales
--------------------

- :doc:`../tutorials/inputs/inputevent`

Propiedades
----------------------

+-------------------------+----------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>` | :ref:`alt<class_InputEventWithModifiers_property_alt>`         | ``false`` |
+-------------------------+----------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>` | :ref:`command<class_InputEventWithModifiers_property_command>` | ``false`` |
+-------------------------+----------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>` | :ref:`control<class_InputEventWithModifiers_property_control>` | ``false`` |
+-------------------------+----------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>` | :ref:`meta<class_InputEventWithModifiers_property_meta>`       | ``false`` |
+-------------------------+----------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>` | :ref:`shift<class_InputEventWithModifiers_property_shift>`     | ``false`` |
+-------------------------+----------------------------------------------------------------+-----------+

Descripciones de Propiedades
--------------------------------------------------------

.. _class_InputEventWithModifiers_property_alt:

- :ref:`bool<class_bool>` **alt**

+-----------+----------------+
| *Default* | ``false``      |
+-----------+----------------+
| *Setter*  | set_alt(value) |
+-----------+----------------+
| *Getter*  | get_alt()      |
+-----------+----------------+

State of the ``Alt`` modifier.

----

.. _class_InputEventWithModifiers_property_command:

- :ref:`bool<class_bool>` **command**

+-----------+--------------------+
| *Default* | ``false``          |
+-----------+--------------------+
| *Setter*  | set_command(value) |
+-----------+--------------------+
| *Getter*  | get_command()      |
+-----------+--------------------+

State of the ``Command`` modifier.

----

.. _class_InputEventWithModifiers_property_control:

- :ref:`bool<class_bool>` **control**

+-----------+--------------------+
| *Default* | ``false``          |
+-----------+--------------------+
| *Setter*  | set_control(value) |
+-----------+--------------------+
| *Getter*  | get_control()      |
+-----------+--------------------+

State of the ``Ctrl`` modifier.

----

.. _class_InputEventWithModifiers_property_meta:

- :ref:`bool<class_bool>` **meta**

+-----------+--------------------+
| *Default* | ``false``          |
+-----------+--------------------+
| *Setter*  | set_metakey(value) |
+-----------+--------------------+
| *Getter*  | get_metakey()      |
+-----------+--------------------+

State of the ``Meta`` modifier.

----

.. _class_InputEventWithModifiers_property_shift:

- :ref:`bool<class_bool>` **shift**

+-----------+------------------+
| *Default* | ``false``        |
+-----------+------------------+
| *Setter*  | set_shift(value) |
+-----------+------------------+
| *Getter*  | get_shift()      |
+-----------+------------------+

State of the ``Shift`` modifier.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
