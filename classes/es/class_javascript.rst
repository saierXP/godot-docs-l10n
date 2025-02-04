:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the JavaScript.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_JavaScript:

JavaScript
==========

**Inherits:** :ref:`Object<class_Object>`

Singleton que conecta el motor con el contexto JavaScript del navegador en la exportación HTML5.

Descripción
----------------------

The JavaScript singleton is implemented only in the HTML5 export. It's used to access the browser's JavaScript context. This allows interaction with embedding pages or calling third-party JavaScript APIs.

\ **Note:** This singleton can be disabled at build-time to improve security. By default, the JavaScript singleton is enabled. Official export templates also have the JavaScript singleton enabled. See :doc:`Compiling for the Web <../development/compiling/compiling_for_web>` in the documentation for more information.

Tutoriales
--------------------

- `#calling-javascript-from-script <../tutorials/export/exporting_for_web.html#calling-javascript-from-script>`__ in :doc:`../tutorials/export/exporting_for_web`

Métodos
--------------

+-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`JavaScriptObject<class_JavaScriptObject>` | :ref:`create_callback<class_JavaScript_method_create_callback>` **(** :ref:`Object<class_Object>` object, :ref:`String<class_String>` method **)**                                                                          |
+-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Variant<class_Variant>`                   | :ref:`create_object<class_JavaScript_method_create_object>` **(** :ref:`String<class_String>` object, ... **)** |vararg|                                                                                                    |
+-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`download_buffer<class_JavaScript_method_download_buffer>` **(** :ref:`PoolByteArray<class_PoolByteArray>` buffer, :ref:`String<class_String>` name, :ref:`String<class_String>` mime="application/octet-stream" **)** |
+-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Variant<class_Variant>`                   | :ref:`eval<class_JavaScript_method_eval>` **(** :ref:`String<class_String>` code, :ref:`bool<class_bool>` use_global_execution_context=false **)**                                                                          |
+-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`JavaScriptObject<class_JavaScriptObject>` | :ref:`get_interface<class_JavaScript_method_get_interface>` **(** :ref:`String<class_String>` interface **)**                                                                                                               |
+-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Descripciones de Métodos
------------------------------------------------

.. _class_JavaScript_method_create_callback:

- :ref:`JavaScriptObject<class_JavaScriptObject>` **create_callback** **(** :ref:`Object<class_Object>` object, :ref:`String<class_String>` method **)**

Creates a reference to a script function that can be used as a callback by JavaScript. The reference must be kept until the callback happens, or it won't be called at all. See :ref:`JavaScriptObject<class_JavaScriptObject>` for usage.

----

.. _class_JavaScript_method_create_object:

- :ref:`Variant<class_Variant>` **create_object** **(** :ref:`String<class_String>` object, ... **)** |vararg|

Creates a new JavaScript object using the ``new`` constructor. The ``object`` must a valid property of the JavaScript ``window``. See :ref:`JavaScriptObject<class_JavaScriptObject>` for usage.

----

.. _class_JavaScript_method_download_buffer:

- void **download_buffer** **(** :ref:`PoolByteArray<class_PoolByteArray>` buffer, :ref:`String<class_String>` name, :ref:`String<class_String>` mime="application/octet-stream" **)**

Prompts the user to download a file containing the specified ``buffer``. The file will have the given ``name`` and ``mime`` type.

\ **Note:** The browser may override the `MIME type <https://en.wikipedia.org/wiki/Media_type>`__ provided based on the file ``name``'s extension.

\ **Note:** Browsers might block the download if :ref:`download_buffer<class_JavaScript_method_download_buffer>` is not being called from a user interaction (e.g. button click).

\ **Note:** Browsers might ask the user for permission or block the download if multiple download requests are made in a quick succession.

----

.. _class_JavaScript_method_eval:

- :ref:`Variant<class_Variant>` **eval** **(** :ref:`String<class_String>` code, :ref:`bool<class_bool>` use_global_execution_context=false **)**

Ejecute la string ``code`` como código JavaScript dentro de la ventana del navegador. Esta es una llamada a la función global actual de JavaScript ``eval()``.

Si ``use_global_execution_context`` es ``true``, el código será evaluado en el contexto de ejecución global. De lo contrario, se evaluará en el contexto de ejecución de una función dentro del entorno de tiempo de ejecución del motor.

----

.. _class_JavaScript_method_get_interface:

- :ref:`JavaScriptObject<class_JavaScriptObject>` **get_interface** **(** :ref:`String<class_String>` interface **)**

Returns an interface to a JavaScript object that can be used by scripts. The ``interface`` must be a valid property of the JavaScript ``window``. The callback must accept a single :ref:`Array<class_Array>` argument, which will contain the JavaScript ``arguments``. See :ref:`JavaScriptObject<class_JavaScriptObject>` for usage.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
