:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the AudioStreamRandomPitch.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_AudioStreamRandomPitch:

AudioStreamRandomPitch
======================

**Inherits:** :ref:`AudioStream<class_AudioStream>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

Reproduce el audio con un cambio de tono aleatorio.

Descripción
----------------------

Varía aleatoriamente el tono en cada inicio.

Propiedades
----------------------

+---------------------------------------+-------------------------------------------------------------------------+---------+
| :ref:`AudioStream<class_AudioStream>` | :ref:`audio_stream<class_AudioStreamRandomPitch_property_audio_stream>` |         |
+---------------------------------------+-------------------------------------------------------------------------+---------+
| :ref:`float<class_float>`             | :ref:`random_pitch<class_AudioStreamRandomPitch_property_random_pitch>` | ``1.1`` |
+---------------------------------------+-------------------------------------------------------------------------+---------+

Descripciones de Propiedades
--------------------------------------------------------

.. _class_AudioStreamRandomPitch_property_audio_stream:

- :ref:`AudioStream<class_AudioStream>` **audio_stream**

+----------+-------------------------+
| *Setter* | set_audio_stream(value) |
+----------+-------------------------+
| *Getter* | get_audio_stream()      |
+----------+-------------------------+

El actual :ref:`AudioStream<class_AudioStream>`.

----

.. _class_AudioStreamRandomPitch_property_random_pitch:

- :ref:`float<class_float>` **random_pitch**

+-----------+-------------------------+
| *Default* | ``1.1``                 |
+-----------+-------------------------+
| *Setter*  | set_random_pitch(value) |
+-----------+-------------------------+
| *Getter*  | get_random_pitch()      |
+-----------+-------------------------+

La intensidad de la variación del tono aleatorio.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
