:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the NetworkedMultiplayerENet.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_NetworkedMultiplayerENet:

NetworkedMultiplayerENet
========================

**Inherits:** :ref:`NetworkedMultiplayerPeer<class_NetworkedMultiplayerPeer>` **<** :ref:`PacketPeer<class_PacketPeer>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

Implementación de PacketPeer usando la biblioteca `ENet <http://enet.bespin.org/index.html>`__.

Descripción
----------------------

A PacketPeer implementation that should be passed to :ref:`SceneTree.network_peer<class_SceneTree_property_network_peer>` after being initialized as either a client or server. Events can then be handled by connecting to :ref:`SceneTree<class_SceneTree>` signals.

ENet's purpose is to provide a relatively thin, simple and robust network communication layer on top of UDP (User Datagram Protocol).

\ **Note:** ENet only uses UDP, not TCP. When forwarding the server port to make your server accessible on the public Internet, you only need to forward the server port in UDP. You can use the :ref:`UPNP<class_UPNP>` class to try to forward the server port automatically when starting the server.

Tutoriales
--------------------

- :doc:`../tutorials/networking/high_level_multiplayer`

- `http://enet.bespin.org/usergroup0.html <http://enet.bespin.org/usergroup0.html>`__

Propiedades
----------------------

+-----------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                                               | :ref:`always_ordered<class_NetworkedMultiplayerENet_property_always_ordered>`     | ``false``                                                                                                             |
+-----------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                                                 | :ref:`channel_count<class_NetworkedMultiplayerENet_property_channel_count>`       | ``3``                                                                                                                 |
+-----------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------+
| :ref:`CompressionMode<enum_NetworkedMultiplayerENet_CompressionMode>` | :ref:`compression_mode<class_NetworkedMultiplayerENet_property_compression_mode>` | ``1``                                                                                                                 |
+-----------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>`                                           | :ref:`dtls_hostname<class_NetworkedMultiplayerENet_property_dtls_hostname>`       | ``""``                                                                                                                |
+-----------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                                               | :ref:`dtls_verify<class_NetworkedMultiplayerENet_property_dtls_verify>`           | ``true``                                                                                                              |
+-----------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                                               | refuse_new_connections                                                            | ``false`` (overrides :ref:`NetworkedMultiplayerPeer<class_NetworkedMultiplayerPeer_property_refuse_new_connections>`) |
+-----------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                                               | :ref:`server_relay<class_NetworkedMultiplayerENet_property_server_relay>`         | ``true``                                                                                                              |
+-----------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                                                 | :ref:`transfer_channel<class_NetworkedMultiplayerENet_property_transfer_channel>` | ``-1``                                                                                                                |
+-----------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------+
| :ref:`TransferMode<enum_NetworkedMultiplayerPeer_TransferMode>`       | transfer_mode                                                                     | ``2`` (overrides :ref:`NetworkedMultiplayerPeer<class_NetworkedMultiplayerPeer_property_transfer_mode>`)              |
+-----------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                                               | :ref:`use_dtls<class_NetworkedMultiplayerENet_property_use_dtls>`                 | ``false``                                                                                                             |
+-----------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------+

Métodos
--------------

+---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`close_connection<class_NetworkedMultiplayerENet_method_close_connection>` **(** :ref:`int<class_int>` wait_usec=100 **)**                                                                                                                                         |
+---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Error<enum_@GlobalScope_Error>` | :ref:`create_client<class_NetworkedMultiplayerENet_method_create_client>` **(** :ref:`String<class_String>` address, :ref:`int<class_int>` port, :ref:`int<class_int>` in_bandwidth=0, :ref:`int<class_int>` out_bandwidth=0, :ref:`int<class_int>` client_port=0 **)** |
+---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Error<enum_@GlobalScope_Error>` | :ref:`create_server<class_NetworkedMultiplayerENet_method_create_server>` **(** :ref:`int<class_int>` port, :ref:`int<class_int>` max_clients=32, :ref:`int<class_int>` in_bandwidth=0, :ref:`int<class_int>` out_bandwidth=0 **)**                                     |
+---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`disconnect_peer<class_NetworkedMultiplayerENet_method_disconnect_peer>` **(** :ref:`int<class_int>` id, :ref:`bool<class_bool>` now=false **)**                                                                                                                   |
+---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                 | :ref:`get_last_packet_channel<class_NetworkedMultiplayerENet_method_get_last_packet_channel>` **(** **)** |const|                                                                                                                                                       |
+---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                 | :ref:`get_packet_channel<class_NetworkedMultiplayerENet_method_get_packet_channel>` **(** **)** |const|                                                                                                                                                                 |
+---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>`           | :ref:`get_peer_address<class_NetworkedMultiplayerENet_method_get_peer_address>` **(** :ref:`int<class_int>` id **)** |const|                                                                                                                                            |
+---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                 | :ref:`get_peer_port<class_NetworkedMultiplayerENet_method_get_peer_port>` **(** :ref:`int<class_int>` id **)** |const|                                                                                                                                                  |
+---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`set_bind_ip<class_NetworkedMultiplayerENet_method_set_bind_ip>` **(** :ref:`String<class_String>` ip **)**                                                                                                                                                        |
+---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`set_dtls_certificate<class_NetworkedMultiplayerENet_method_set_dtls_certificate>` **(** :ref:`X509Certificate<class_X509Certificate>` certificate **)**                                                                                                           |
+---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`set_dtls_key<class_NetworkedMultiplayerENet_method_set_dtls_key>` **(** :ref:`CryptoKey<class_CryptoKey>` key **)**                                                                                                                                               |
+---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`set_peer_timeout<class_NetworkedMultiplayerENet_method_set_peer_timeout>` **(** :ref:`int<class_int>` id, :ref:`int<class_int>` timeout_limit, :ref:`int<class_int>` timeout_min, :ref:`int<class_int>` timeout_max **)**                                         |
+---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Enumeraciones
--------------------------

.. _enum_NetworkedMultiplayerENet_CompressionMode:

.. _class_NetworkedMultiplayerENet_constant_COMPRESS_NONE:

.. _class_NetworkedMultiplayerENet_constant_COMPRESS_RANGE_CODER:

.. _class_NetworkedMultiplayerENet_constant_COMPRESS_FASTLZ:

.. _class_NetworkedMultiplayerENet_constant_COMPRESS_ZLIB:

.. _class_NetworkedMultiplayerENet_constant_COMPRESS_ZSTD:

enum **CompressionMode**:

- **COMPRESS_NONE** = **0** --- No compression. This uses the most bandwidth, but has the upside of requiring the fewest CPU resources. This option may also be used to make network debugging using tools like Wireshark easier.

- **COMPRESS_RANGE_CODER** = **1** --- ENet's built-in range encoding. Works well on small packets, but is not the most efficient algorithm on packets larger than 4 KB.

- **COMPRESS_FASTLZ** = **2** --- `Compresión FastLZ <http://fastlz.org/>`__. Esta opción utiliza menos recursos de CPU en comparación con :ref:`COMPRESS_ZLIB<class_NetworkedMultiplayerENet_constant_COMPRESS_ZLIB>`, a expensas de utilizar más ancho de banda.

- **COMPRESS_ZLIB** = **3** --- `Zlib <https://www.zlib.net/>`__ compression. This option uses less bandwidth compared to :ref:`COMPRESS_FASTLZ<class_NetworkedMultiplayerENet_constant_COMPRESS_FASTLZ>`, at the expense of using more CPU resources. Note that this algorithm is not very efficient on packets smaller than 4 KB. Therefore, it's recommended to use other compression algorithms in most cases.

- **COMPRESS_ZSTD** = **4** --- `Compresión estándar  <https://facebook.github.io/zstd/>`__.

Descripciones de Propiedades
--------------------------------------------------------

.. _class_NetworkedMultiplayerENet_property_always_ordered:

- :ref:`bool<class_bool>` **always_ordered**

+-----------+---------------------------+
| *Default* | ``false``                 |
+-----------+---------------------------+
| *Setter*  | set_always_ordered(value) |
+-----------+---------------------------+
| *Getter*  | is_always_ordered()       |
+-----------+---------------------------+

Fuerza el orden de los paquetes cuando se utiliza :ref:`NetworkedMultiplayerPeer.TRANSFER_MODE_UNRELIABLE<class_NetworkedMultiplayerPeer_constant_TRANSFER_MODE_UNRELIABLE>` (por lo que se comporta de manera similar a :ref:`NetworkedMultiplayerPeer.TRANSFER_MODE_UNRELIABLE_ORDERED<class_NetworkedMultiplayerPeer_constant_TRANSFER_MODE_UNRELIABLE_ORDERED>`). Esta es la única manera de usar el sistema de pedidos con el sistema RPC.

----

.. _class_NetworkedMultiplayerENet_property_channel_count:

- :ref:`int<class_int>` **channel_count**

+-----------+--------------------------+
| *Default* | ``3``                    |
+-----------+--------------------------+
| *Setter*  | set_channel_count(value) |
+-----------+--------------------------+
| *Getter*  | get_channel_count()      |
+-----------+--------------------------+

El número de canales que será usado por ENet. Los canales se usan para separar diferentes tipos de datos. En el modo fiable o pedido, por ejemplo, la orden de entrega de paquetes se asegura por cada canal. Esto se hace para combatir la latencia y reducir las restricciones de pedido de los paquetes. El estado de entrega de un paquete en un canal no detendrá la entrega de otros paquetes en otro canal.

----

.. _class_NetworkedMultiplayerENet_property_compression_mode:

- :ref:`CompressionMode<enum_NetworkedMultiplayerENet_CompressionMode>` **compression_mode**

+-----------+-----------------------------+
| *Default* | ``1``                       |
+-----------+-----------------------------+
| *Setter*  | set_compression_mode(value) |
+-----------+-----------------------------+
| *Getter*  | get_compression_mode()      |
+-----------+-----------------------------+

The compression method used for network packets. These have different tradeoffs of compression speed versus bandwidth, you may need to test which one works best for your use case if you use compression at all.

\ **Note:** Most games' network design involve sending many small packets frequently (smaller than 4 KB each). If in doubt, it is recommended to keep the default compression algorithm as it works best on these small packets.

\ **Note:** :ref:`compression_mode<class_NetworkedMultiplayerENet_property_compression_mode>` must be set to the same value on both the server and all its clients. Clients will fail to connect if the :ref:`compression_mode<class_NetworkedMultiplayerENet_property_compression_mode>` set on the client differs from the one set on the server. Prior to Godot 3.4, the default :ref:`compression_mode<class_NetworkedMultiplayerENet_property_compression_mode>` was :ref:`COMPRESS_NONE<class_NetworkedMultiplayerENet_constant_COMPRESS_NONE>`. Nonetheless, mixing engine versions between clients and server is not recommended and not officially supported.

----

.. _class_NetworkedMultiplayerENet_property_dtls_hostname:

- :ref:`String<class_String>` **dtls_hostname**

+-----------+--------------------------+
| *Default* | ``""``                   |
+-----------+--------------------------+
| *Setter*  | set_dtls_hostname(value) |
+-----------+--------------------------+
| *Getter*  | get_dtls_hostname()      |
+-----------+--------------------------+

The hostname used for DTLS verification, to be compared against the "CN" value in the certificate provided by the server.

When set to an empty string, the ``address`` parameter passed to :ref:`create_client<class_NetworkedMultiplayerENet_method_create_client>` is used instead.

----

.. _class_NetworkedMultiplayerENet_property_dtls_verify:

- :ref:`bool<class_bool>` **dtls_verify**

+-----------+--------------------------------+
| *Default* | ``true``                       |
+-----------+--------------------------------+
| *Setter*  | set_dtls_verify_enabled(value) |
+-----------+--------------------------------+
| *Getter*  | is_dtls_verify_enabled()       |
+-----------+--------------------------------+

Habilitar o deshabilitar la verificación del certificado cuando :ref:`use_dtls<class_NetworkedMultiplayerENet_property_use_dtls>` ``true``.

----

.. _class_NetworkedMultiplayerENet_property_server_relay:

- :ref:`bool<class_bool>` **server_relay**

+-----------+---------------------------------+
| *Default* | ``true``                        |
+-----------+---------------------------------+
| *Setter*  | set_server_relay_enabled(value) |
+-----------+---------------------------------+
| *Getter*  | is_server_relay_enabled()       |
+-----------+---------------------------------+

Habilitar o deshabilitar la función del servidor que notifica a los clientes de la conexión/desconexión de otros compañeros, y retransmitir mensajes entre ellos. Cuando esta opción es ``false``, los clientes no serán notificados automáticamente de la conexión/desconexión de otros compañeros y no podrán enviarles paquetes a través del servidor.

----

.. _class_NetworkedMultiplayerENet_property_transfer_channel:

- :ref:`int<class_int>` **transfer_channel**

+-----------+-----------------------------+
| *Default* | ``-1``                      |
+-----------+-----------------------------+
| *Setter*  | set_transfer_channel(value) |
+-----------+-----------------------------+
| *Getter*  | get_transfer_channel()      |
+-----------+-----------------------------+

Establezca el canal predeterminado que se utilizará para la transferencia de datos. Por defecto, este valor es ``-1``, lo que significa que ENet sólo utilizará 2 canales: uno para los paquetes fiables y otro para los no fiables. El canal ``0`` está reservado y no puede ser utilizado. Ajustar este miembro a cualquier valor entre ``0`` y :ref:`channel_count<class_NetworkedMultiplayerENet_property_channel_count>` (excluido) obligará a ENet a utilizar ese canal para enviar datos. Vea :ref:`channel_count<class_NetworkedMultiplayerENet_property_channel_count>` para más información sobre los canales de ENet.

----

.. _class_NetworkedMultiplayerENet_property_use_dtls:

- :ref:`bool<class_bool>` **use_dtls**

+-----------+-------------------------+
| *Default* | ``false``               |
+-----------+-------------------------+
| *Setter*  | set_dtls_enabled(value) |
+-----------+-------------------------+
| *Getter*  | is_dtls_enabled()       |
+-----------+-------------------------+

When enabled, the client or server created by this peer, will use :ref:`PacketPeerDTLS<class_PacketPeerDTLS>` instead of raw UDP sockets for communicating with the remote peer. This will make the communication encrypted with DTLS at the cost of higher resource usage and potentially larger packet size.

\ **Note:** When creating a DTLS server, make sure you setup the key/certificate pair via :ref:`set_dtls_key<class_NetworkedMultiplayerENet_method_set_dtls_key>` and :ref:`set_dtls_certificate<class_NetworkedMultiplayerENet_method_set_dtls_certificate>`. For DTLS clients, have a look at the :ref:`dtls_verify<class_NetworkedMultiplayerENet_property_dtls_verify>` option, and configure the certificate accordingly via :ref:`set_dtls_certificate<class_NetworkedMultiplayerENet_method_set_dtls_certificate>`.

Descripciones de Métodos
------------------------------------------------

.. _class_NetworkedMultiplayerENet_method_close_connection:

- void **close_connection** **(** :ref:`int<class_int>` wait_usec=100 **)**

Cierra la conexión. Ignorado si no se establece ninguna conexión actualmente. Si se trata de un servidor, intenta notificar a todos los clientes antes de desconectarlos por la fuerza. Si se trata de un cliente, simplemente cierra la conexión con el servidor.

----

.. _class_NetworkedMultiplayerENet_method_create_client:

- :ref:`Error<enum_@GlobalScope_Error>` **create_client** **(** :ref:`String<class_String>` address, :ref:`int<class_int>` port, :ref:`int<class_int>` in_bandwidth=0, :ref:`int<class_int>` out_bandwidth=0, :ref:`int<class_int>` client_port=0 **)**

Crear el cliente que se conecta a un servidor en la ``address`` usando el ``port`` especificado. La dirección especificada debe ser un nombre de dominio completamente cualificado (por ejemplo, ``"www.example.com"``) o una dirección IP en formato IPv4 o IPv6 (por ejemplo, ``"192.168.1.1"``). El ``port`` es el puerto en el que el servidor está escuchando. Los parámetros ``in_bandwith`` y ``out_bandwidth`` pueden utilizarse para limitar el ancho de banda de entrada y de salida al número dado de bytes por segundo. El valor predeterminado de 0 significa ancho de banda ilimitado. Tenga en cuenta que el ENet dejará caer estratégicamente paquetes en lados específicos de una conexión entre pares para asegurarse de que el ancho de banda del par no se vea sobrepasado. Los parámetros de ancho de banda también determinan el tamaño de la ventana de una conexión que limita la cantidad de paquetes confiables que pueden estar en tránsito en un momento dado. Devuelve :ref:`@GlobalScope.OK<class_@GlobalScope_constant_OK>` si se creó un cliente, :ref:`@GlobalScope.ERR_ALREADY_IN_USE<class_@GlobalScope_constant_ERR_ALREADY_IN_USE>` si esta instancia NetworkedMultiplayerENet ya tiene una conexión abierta (en cuyo caso necesita llamar primero a :ref:`close_connection<class_NetworkedMultiplayerENet_method_close_connection>`) o :ref:`@GlobalScope.ERR_CANT_CREATE<class_@GlobalScope_constant_ERR_CANT_CREATE>` si no se pudo crear el cliente. Si se especifica ``client_port``, el cliente también escuchará el puerto dado; esto es útil para algunas técnicas de travesía de NAT.

----

.. _class_NetworkedMultiplayerENet_method_create_server:

- :ref:`Error<enum_@GlobalScope_Error>` **create_server** **(** :ref:`int<class_int>` port, :ref:`int<class_int>` max_clients=32, :ref:`int<class_int>` in_bandwidth=0, :ref:`int<class_int>` out_bandwidth=0 **)**

Crear un servidor que escuche las conexiones a través de ``port``. El puerto debe ser un puerto disponible y no utilizado entre 0 y 65535. Tenga en cuenta que los puertos por debajo de 1024 son privilegiados y pueden requerir permisos elevados dependiendo de la plataforma. Para cambiar la interfaz en la que escucha el servidor, utilice :ref:`set_bind_ip<class_NetworkedMultiplayerENet_method_set_bind_ip>`. La IP por defecto es el comodín ``"*"``, que escucha en todas las interfaces disponibles. ``max_clients`` es el número máximo de clientes que se permiten a la vez, se puede utilizar cualquier número hasta 4095, aunque el número alcanzable de clientes simultáneos puede ser muy inferior y depende de la aplicación. Para más detalles sobre los parámetros de ancho de banda, véase :ref:`create_client<class_NetworkedMultiplayerENet_method_create_client>`. Devuelve :ref:`@GlobalScope.OK<class_@GlobalScope_constant_OK>` si se ha creado un servidor, :ref:`@GlobalScope.ERR_ALREADY_IN_USE<class_@GlobalScope_constant_ERR_ALREADY_IN_USE>` si esta instancia NetworkedMultiplayerENet ya tiene una conexión abierta (en cuyo caso hay que llamar primero a :ref:`close_connection<class_NetworkedMultiplayerENet_method_close_connection>`) o :ref:`@GlobalScope.ERR_CANT_CREATE<class_@GlobalScope_constant_ERR_CANT_CREATE>` si no se ha podido crear el servidor.

----

.. _class_NetworkedMultiplayerENet_method_disconnect_peer:

- void **disconnect_peer** **(** :ref:`int<class_int>` id, :ref:`bool<class_bool>` now=false **)**

Desconecta el par dado. Si "ahora" está configurado como ``true``, la conexión se cerrará inmediatamente sin eliminar los mensajes de la cola.

----

.. _class_NetworkedMultiplayerENet_method_get_last_packet_channel:

- :ref:`int<class_int>` **get_last_packet_channel** **(** **)** |const|

Devuelve el canal del último paquete obtenido a través del :ref:`PacketPeer.get_packet<class_PacketPeer_method_get_packet>`.

----

.. _class_NetworkedMultiplayerENet_method_get_packet_channel:

- :ref:`int<class_int>` **get_packet_channel** **(** **)** |const|

Devuelve el canal del siguiente paquete que será recuperado a través del :ref:`PacketPeer.get_packet<class_PacketPeer_method_get_packet>`.

----

.. _class_NetworkedMultiplayerENet_method_get_peer_address:

- :ref:`String<class_String>` **get_peer_address** **(** :ref:`int<class_int>` id **)** |const|

Devuelve la dirección IP del par dado.

----

.. _class_NetworkedMultiplayerENet_method_get_peer_port:

- :ref:`int<class_int>` **get_peer_port** **(** :ref:`int<class_int>` id **)** |const|

Devuelve el puerto remoto del par dado.

----

.. _class_NetworkedMultiplayerENet_method_set_bind_ip:

- void **set_bind_ip** **(** :ref:`String<class_String>` ip **)**

La IP usada cuando se crea un servidor. Está configurada por defecto con el comodín ``"*"``, que se une a todas las interfaces disponibles. La IP dada debe estar en formato de dirección IPv4 o IPv6, por ejemplo: ``"192.168.1.1"``.

----

.. _class_NetworkedMultiplayerENet_method_set_dtls_certificate:

- void **set_dtls_certificate** **(** :ref:`X509Certificate<class_X509Certificate>` certificate **)**

Configure el :ref:`X509Certificate<class_X509Certificate>` para usarlo cuando :ref:`use_dtls<class_NetworkedMultiplayerENet_property_use_dtls>` sea ``true[/code Configure el [X509Certificate] para usarlo cuando [member use_dtls] sea [code]true``. Para los servidores, también debe configurar la :ref:`CryptoKey<class_CryptoKey>` mediante el :ref:`set_dtls_key<class_NetworkedMultiplayerENet_method_set_dtls_key>`.]. Para los servidores, también debe configurar la :ref:`CryptoKey<class_CryptoKey>` a través de :ref:`set_dtls_key<class_NetworkedMultiplayerENet_method_set_dtls_key>`.

----

.. _class_NetworkedMultiplayerENet_method_set_dtls_key:

- void **set_dtls_key** **(** :ref:`CryptoKey<class_CryptoKey>` key **)**

Configure el :ref:`X509Certificate<class_X509Certificate>` para usarlo cuando :ref:`use_dtls<class_NetworkedMultiplayerENet_property_use_dtls>` sea ``true``. Para los servidores, también debe configurar la :ref:`CryptoKey<class_CryptoKey>` mediante el :ref:`set_dtls_key<class_NetworkedMultiplayerENet_method_set_dtls_key>`.

----

.. _class_NetworkedMultiplayerENet_method_set_peer_timeout:

- void **set_peer_timeout** **(** :ref:`int<class_int>` id, :ref:`int<class_int>` timeout_limit, :ref:`int<class_int>` timeout_min, :ref:`int<class_int>` timeout_max **)**

Sets the timeout parameters for a peer.	The timeout parameters control how and when a peer will timeout from a failure to acknowledge reliable traffic. Timeout values are expressed in milliseconds.

The ``timeout_limit`` is a factor that, multiplied by a value based on the average round trip time, will determine the timeout limit for a reliable packet. When that limit is reached, the timeout will be doubled, and the peer will be disconnected if that limit has reached ``timeout_min``. The ``timeout_max`` parameter, on the other hand, defines a fixed timeout for which any packet must be acknowledged or the peer will be dropped.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
