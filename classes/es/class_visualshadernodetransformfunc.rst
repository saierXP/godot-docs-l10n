:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the VisualShaderNodeTransformFunc.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_VisualShaderNodeTransformFunc:

VisualShaderNodeTransformFunc
=============================

**Inherits:** :ref:`VisualShaderNode<class_VisualShaderNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

Calcula una función :ref:`Transform<class_Transform>` dentro del gráfico shader visual.

Descripción
----------------------

Calcula una función inversa o de transposición en la :ref:`Transform<class_Transform>` proporcionado.

Propiedades
----------------------

+--------------------------------------------------------------+------------------------------------------------------------------------+-------+
| :ref:`Function<enum_VisualShaderNodeTransformFunc_Function>` | :ref:`function<class_VisualShaderNodeTransformFunc_property_function>` | ``0`` |
+--------------------------------------------------------------+------------------------------------------------------------------------+-------+

Enumeraciones
--------------------------

.. _enum_VisualShaderNodeTransformFunc_Function:

.. _class_VisualShaderNodeTransformFunc_constant_FUNC_INVERSE:

.. _class_VisualShaderNodeTransformFunc_constant_FUNC_TRANSPOSE:

enum **Function**:

- **FUNC_INVERSE** = **0** --- Realiza la operación inversa en la matriz de la :ref:`Transform<class_Transform>`.

- **FUNC_TRANSPOSE** = **1** --- Realice la operación de transposición en la matriz :ref:`Transform<class_Transform>`.

Descripciones de Propiedades
--------------------------------------------------------

.. _class_VisualShaderNodeTransformFunc_property_function:

- :ref:`Function<enum_VisualShaderNodeTransformFunc_Function>` **function**

+-----------+---------------------+
| *Default* | ``0``               |
+-----------+---------------------+
| *Setter*  | set_function(value) |
+-----------+---------------------+
| *Getter*  | get_function()      |
+-----------+---------------------+

La función a computar. Ver :ref:`Function<enum_VisualShaderNodeTransformFunc_Function>` para las opciones.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
