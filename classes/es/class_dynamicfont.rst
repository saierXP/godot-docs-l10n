:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the DynamicFont.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_DynamicFont:

DynamicFont
===========

**Inherits:** :ref:`Font<class_Font>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

DynamicFont renderiza archivos de fuentes vectoriales en tiempo de ejecución.

Descripción
----------------------

DynamicFont renders vector font files dynamically at runtime instead of using a prerendered texture atlas like :ref:`BitmapFont<class_BitmapFont>`. This trades the faster loading time of :ref:`BitmapFont<class_BitmapFont>`\ s for the ability to change font parameters like size and spacing during runtime. :ref:`DynamicFontData<class_DynamicFontData>` is used for referencing the font file paths. DynamicFont also supports defining one or more fallback fonts, which will be used when displaying a character not supported by the main font.

DynamicFont uses the `FreeType <https://www.freetype.org/>`__ library for rasterization. Supported formats are TrueType (``.ttf``), OpenType (``.otf``) and Web Open Font Format 1 (``.woff``). Web Open Font Format 2 (``.woff2``) is *not* supported.

::

    var dynamic_font = DynamicFont.new()
    dynamic_font.font_data = load("res://BarlowCondensed-Bold.ttf")
    dynamic_font.size = 64
    $"Label".set("custom_fonts/font", dynamic_font)

\ **Note:** DynamicFont doesn't support features such as kerning, right-to-left typesetting, ligatures, text shaping, variable fonts and optional font features yet. If you wish to "bake" an optional font feature into a TTF font file, you can use `FontForge <https://fontforge.org/>`__ to do so. In FontForge, use **File > Generate Fonts**, click **Options**, choose the desired features then generate the font.

Tutoriales
--------------------

- `3D Voxel Demo <https://godotengine.org/asset-library/asset/676>`__

Propiedades
----------------------

+-----------------------------------------------+------------------------------------------------------------------------------+-------------------------+
| :ref:`int<class_int>`                         | :ref:`extra_spacing_bottom<class_DynamicFont_property_extra_spacing_bottom>` | ``0``                   |
+-----------------------------------------------+------------------------------------------------------------------------------+-------------------------+
| :ref:`int<class_int>`                         | :ref:`extra_spacing_char<class_DynamicFont_property_extra_spacing_char>`     | ``0``                   |
+-----------------------------------------------+------------------------------------------------------------------------------+-------------------------+
| :ref:`int<class_int>`                         | :ref:`extra_spacing_space<class_DynamicFont_property_extra_spacing_space>`   | ``0``                   |
+-----------------------------------------------+------------------------------------------------------------------------------+-------------------------+
| :ref:`int<class_int>`                         | :ref:`extra_spacing_top<class_DynamicFont_property_extra_spacing_top>`       | ``0``                   |
+-----------------------------------------------+------------------------------------------------------------------------------+-------------------------+
| :ref:`DynamicFontData<class_DynamicFontData>` | :ref:`font_data<class_DynamicFont_property_font_data>`                       |                         |
+-----------------------------------------------+------------------------------------------------------------------------------+-------------------------+
| :ref:`Color<class_Color>`                     | :ref:`outline_color<class_DynamicFont_property_outline_color>`               | ``Color( 1, 1, 1, 1 )`` |
+-----------------------------------------------+------------------------------------------------------------------------------+-------------------------+
| :ref:`int<class_int>`                         | :ref:`outline_size<class_DynamicFont_property_outline_size>`                 | ``0``                   |
+-----------------------------------------------+------------------------------------------------------------------------------+-------------------------+
| :ref:`int<class_int>`                         | :ref:`size<class_DynamicFont_property_size>`                                 | ``16``                  |
+-----------------------------------------------+------------------------------------------------------------------------------+-------------------------+
| :ref:`bool<class_bool>`                       | :ref:`use_filter<class_DynamicFont_property_use_filter>`                     | ``false``               |
+-----------------------------------------------+------------------------------------------------------------------------------+-------------------------+
| :ref:`bool<class_bool>`                       | :ref:`use_mipmaps<class_DynamicFont_property_use_mipmaps>`                   | ``false``               |
+-----------------------------------------------+------------------------------------------------------------------------------+-------------------------+

Métodos
--------------

+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                          | :ref:`add_fallback<class_DynamicFont_method_add_fallback>` **(** :ref:`DynamicFontData<class_DynamicFontData>` data **)**                            |
+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>`                   | :ref:`get_available_chars<class_DynamicFont_method_get_available_chars>` **(** **)** |const|                                                         |
+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`DynamicFontData<class_DynamicFontData>` | :ref:`get_fallback<class_DynamicFont_method_get_fallback>` **(** :ref:`int<class_int>` idx **)** |const|                                             |
+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                         | :ref:`get_fallback_count<class_DynamicFont_method_get_fallback_count>` **(** **)** |const|                                                           |
+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                         | :ref:`get_spacing<class_DynamicFont_method_get_spacing>` **(** :ref:`int<class_int>` type **)** |const|                                              |
+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                          | :ref:`remove_fallback<class_DynamicFont_method_remove_fallback>` **(** :ref:`int<class_int>` idx **)**                                               |
+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                          | :ref:`set_fallback<class_DynamicFont_method_set_fallback>` **(** :ref:`int<class_int>` idx, :ref:`DynamicFontData<class_DynamicFontData>` data **)** |
+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                          | :ref:`set_spacing<class_DynamicFont_method_set_spacing>` **(** :ref:`int<class_int>` type, :ref:`int<class_int>` value **)**                         |
+-----------------------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------+

Enumeraciones
--------------------------

.. _enum_DynamicFont_SpacingType:

.. _class_DynamicFont_constant_SPACING_TOP:

.. _class_DynamicFont_constant_SPACING_BOTTOM:

.. _class_DynamicFont_constant_SPACING_CHAR:

.. _class_DynamicFont_constant_SPACING_SPACE:

enum **SpacingType**:

- **SPACING_TOP** = **0** --- El espacio en la parte superior.

- **SPACING_BOTTOM** = **1** --- El espacio en la parte inferior.

- **SPACING_CHAR** = **2** --- Spacing for each character.

- **SPACING_SPACE** = **3** --- Spacing for the space character.

Descripciones de Propiedades
--------------------------------------------------------

.. _class_DynamicFont_property_extra_spacing_bottom:

- :ref:`int<class_int>` **extra_spacing_bottom**

+-----------+--------------------+
| *Default* | ``0``              |
+-----------+--------------------+
| *Setter*  | set_spacing(value) |
+-----------+--------------------+
| *Getter*  | get_spacing()      |
+-----------+--------------------+

Espacio extra en la parte inferior en píxeles.

----

.. _class_DynamicFont_property_extra_spacing_char:

- :ref:`int<class_int>` **extra_spacing_char**

+-----------+--------------------+
| *Default* | ``0``              |
+-----------+--------------------+
| *Setter*  | set_spacing(value) |
+-----------+--------------------+
| *Getter*  | get_spacing()      |
+-----------+--------------------+

Extra spacing for each character in pixels.

This can be a negative number to make the distance between characters smaller.

----

.. _class_DynamicFont_property_extra_spacing_space:

- :ref:`int<class_int>` **extra_spacing_space**

+-----------+--------------------+
| *Default* | ``0``              |
+-----------+--------------------+
| *Setter*  | set_spacing(value) |
+-----------+--------------------+
| *Getter*  | get_spacing()      |
+-----------+--------------------+

Extra spacing for the space character (in addition to :ref:`extra_spacing_char<class_DynamicFont_property_extra_spacing_char>`) in pixels.

This can be a negative number to make the distance between words smaller.

----

.. _class_DynamicFont_property_extra_spacing_top:

- :ref:`int<class_int>` **extra_spacing_top**

+-----------+--------------------+
| *Default* | ``0``              |
+-----------+--------------------+
| *Setter*  | set_spacing(value) |
+-----------+--------------------+
| *Getter*  | get_spacing()      |
+-----------+--------------------+

Espacio extra en la parte superior en píxeles.

----

.. _class_DynamicFont_property_font_data:

- :ref:`DynamicFontData<class_DynamicFontData>` **font_data**

+----------+----------------------+
| *Setter* | set_font_data(value) |
+----------+----------------------+
| *Getter* | get_font_data()      |
+----------+----------------------+

Los datos de la fuente.

----

.. _class_DynamicFont_property_outline_color:

- :ref:`Color<class_Color>` **outline_color**

+-----------+--------------------------+
| *Default* | ``Color( 1, 1, 1, 1 )``  |
+-----------+--------------------------+
| *Setter*  | set_outline_color(value) |
+-----------+--------------------------+
| *Getter*  | get_outline_color()      |
+-----------+--------------------------+

El color del contorno de la fuente.

\ **Nota:** Se recomienda dejar este valor por defecto para poder ajustarlo en los controles individuales. Por ejemplo, si el contorno se hace negro aquí, no será posible cambiar su color usando un elemento del tema modular el contorno de la fuente de una etiqueta.

----

.. _class_DynamicFont_property_outline_size:

- :ref:`int<class_int>` **outline_size**

+-----------+-------------------------+
| *Default* | ``0``                   |
+-----------+-------------------------+
| *Setter*  | set_outline_size(value) |
+-----------+-------------------------+
| *Getter*  | get_outline_size()      |
+-----------+-------------------------+

El grosor del contorno de la fuente en píxeles (no en relación con el tamaño de la fuente).

----

.. _class_DynamicFont_property_size:

- :ref:`int<class_int>` **size**

+-----------+-----------------+
| *Default* | ``16``          |
+-----------+-----------------+
| *Setter*  | set_size(value) |
+-----------+-----------------+
| *Getter*  | get_size()      |
+-----------+-----------------+

El tamaño de la fuente en píxeles.

----

.. _class_DynamicFont_property_use_filter:

- :ref:`bool<class_bool>` **use_filter**

+-----------+-----------------------+
| *Default* | ``false``             |
+-----------+-----------------------+
| *Setter*  | set_use_filter(value) |
+-----------+-----------------------+
| *Getter*  | get_use_filter()      |
+-----------+-----------------------+

If ``true``, filtering is used. This makes the font blurry instead of pixelated when scaling it if font oversampling is disabled or ineffective. It's recommended to enable this when using the font in a control whose size changes over time, unless a pixel art aesthetic is desired.

----

.. _class_DynamicFont_property_use_mipmaps:

- :ref:`bool<class_bool>` **use_mipmaps**

+-----------+------------------------+
| *Default* | ``false``              |
+-----------+------------------------+
| *Setter*  | set_use_mipmaps(value) |
+-----------+------------------------+
| *Getter*  | get_use_mipmaps()      |
+-----------+------------------------+

If ``true``, mipmapping is used. This improves the font's appearance when downscaling it if font oversampling is disabled or ineffective.

Descripciones de Métodos
------------------------------------------------

.. _class_DynamicFont_method_add_fallback:

- void **add_fallback** **(** :ref:`DynamicFontData<class_DynamicFontData>` data **)**

Añade una fuente alternativa.

----

.. _class_DynamicFont_method_get_available_chars:

- :ref:`String<class_String>` **get_available_chars** **(** **)** |const|

Devuelve una string que contiene todos los caracteres disponibles en la fuente principal y en todas las fuentes secundarias.

Si un carácter determinado se incluye en más de una fuente, aparece sólo una vez en la cadena devuelta.

----

.. _class_DynamicFont_method_get_fallback:

- :ref:`DynamicFontData<class_DynamicFontData>` **get_fallback** **(** :ref:`int<class_int>` idx **)** |const|

Devuelve la fuente de reserva en el índice ``idx``.

----

.. _class_DynamicFont_method_get_fallback_count:

- :ref:`int<class_int>` **get_fallback_count** **(** **)** |const|

Devuelve el número de fuentes de reserva.

----

.. _class_DynamicFont_method_get_spacing:

- :ref:`int<class_int>` **get_spacing** **(** :ref:`int<class_int>` type **)** |const|

Devuelve el espacio para el ``type`` dado (véase :ref:`SpacingType<enum_DynamicFont_SpacingType>`).

----

.. _class_DynamicFont_method_remove_fallback:

- void **remove_fallback** **(** :ref:`int<class_int>` idx **)**

Elimina la fuente de reserva en el índice ``idx``.

----

.. _class_DynamicFont_method_set_fallback:

- void **set_fallback** **(** :ref:`int<class_int>` idx, :ref:`DynamicFontData<class_DynamicFontData>` data **)**

Establece la fuente alternativa en el índice ``idx``.

----

.. _class_DynamicFont_method_set_spacing:

- void **set_spacing** **(** :ref:`int<class_int>` type, :ref:`int<class_int>` value **)**

Establece el espacio para ``type`` (véase :ref:`SpacingType<enum_DynamicFont_SpacingType>`) en ``value`` en píxeles (no en relación con el tamaño de la fuente).

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
