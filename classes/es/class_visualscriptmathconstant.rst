:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the VisualScriptMathConstant.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_VisualScriptMathConstant:

VisualScriptMathConstant
========================

**Inherits:** :ref:`VisualScriptNode<class_VisualScriptNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

Constantes matemáticas comúnmente usadas.

Descripción
----------------------

Proporciona constantes matemáticas comunes, como Pi, en un puerto de salida de datos.

\ **Puertos de entrada:**\ 

ninguno

\ **Puertos de salida:**\ 

- Datos (variante): ``get``

Propiedades
----------------------

+-----------------------------------------------------------------+-------------------------------------------------------------------+-------+
| :ref:`MathConstant<enum_VisualScriptMathConstant_MathConstant>` | :ref:`constant<class_VisualScriptMathConstant_property_constant>` | ``0`` |
+-----------------------------------------------------------------+-------------------------------------------------------------------+-------+

Enumeraciones
--------------------------

.. _enum_VisualScriptMathConstant_MathConstant:

.. _class_VisualScriptMathConstant_constant_MATH_CONSTANT_ONE:

.. _class_VisualScriptMathConstant_constant_MATH_CONSTANT_PI:

.. _class_VisualScriptMathConstant_constant_MATH_CONSTANT_HALF_PI:

.. _class_VisualScriptMathConstant_constant_MATH_CONSTANT_TAU:

.. _class_VisualScriptMathConstant_constant_MATH_CONSTANT_E:

.. _class_VisualScriptMathConstant_constant_MATH_CONSTANT_SQRT2:

.. _class_VisualScriptMathConstant_constant_MATH_CONSTANT_INF:

.. _class_VisualScriptMathConstant_constant_MATH_CONSTANT_NAN:

.. _class_VisualScriptMathConstant_constant_MATH_CONSTANT_MAX:

enum **MathConstant**:

- **MATH_CONSTANT_ONE** = **0** --- Unity: ``1``.

- **MATH_CONSTANT_PI** = **1** --- Pi: ``3.141593``.

- **MATH_CONSTANT_HALF_PI** = **2** --- Pi dividido por dos: ``1.570796``.

- **MATH_CONSTANT_TAU** = **3** --- Tau: ``6.283185``.

- **MATH_CONSTANT_E** = **4** --- Constante Matemática ``e``,base de logaritmo natural ``2.718282``.

- **MATH_CONSTANT_SQRT2** = **5** --- Raíz cuadrada de dos: ``1.414214``.

- **MATH_CONSTANT_INF** = **6** --- Infinito: ``inf``.

- **MATH_CONSTANT_NAN** = **7** --- No un nombre: ``nan``.

- **MATH_CONSTANT_MAX** = **8** --- Representa el tamaño del enum :ref:`MathConstant<enum_VisualScriptMathConstant_MathConstant>`.

Descripciones de Propiedades
--------------------------------------------------------

.. _class_VisualScriptMathConstant_property_constant:

- :ref:`MathConstant<enum_VisualScriptMathConstant_MathConstant>` **constant**

+-----------+--------------------------+
| *Default* | ``0``                    |
+-----------+--------------------------+
| *Setter*  | set_math_constant(value) |
+-----------+--------------------------+
| *Getter*  | get_math_constant()      |
+-----------+--------------------------+

La constante matemática.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
