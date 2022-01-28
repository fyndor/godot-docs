:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the CollisionObject3D.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_CollisionObject3D:

CollisionObject3D
=================

**Inherits:** :ref:`Node3D<class_Node3D>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`Area3D<class_Area3D>`, :ref:`PhysicsBody3D<class_PhysicsBody3D>`

Base node for collision objects.

Description
-----------

CollisionObject3D is the base class for physics objects. It can hold any number of collision :ref:`Shape3D<class_Shape3D>`\ s. Each shape must be assigned to a *shape owner*. The CollisionObject3D can have any number of shape owners. Shape owners are not nodes and do not appear in the editor, but are accessible through code using the ``shape_owner_*`` methods.

Properties
----------

+--------------------------------------------------------+--------------------------------------------------------------------------------------+-----------+
| :ref:`int<class_int>`                                  | :ref:`collision_layer<class_CollisionObject3D_property_collision_layer>`             | ``1``     |
+--------------------------------------------------------+--------------------------------------------------------------------------------------+-----------+
| :ref:`int<class_int>`                                  | :ref:`collision_mask<class_CollisionObject3D_property_collision_mask>`               | ``1``     |
+--------------------------------------------------------+--------------------------------------------------------------------------------------+-----------+
| :ref:`DisableMode<enum_CollisionObject3D_DisableMode>` | :ref:`disable_mode<class_CollisionObject3D_property_disable_mode>`                   | ``0``     |
+--------------------------------------------------------+--------------------------------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>`                                | :ref:`input_capture_on_drag<class_CollisionObject3D_property_input_capture_on_drag>` | ``false`` |
+--------------------------------------------------------+--------------------------------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>`                                | :ref:`input_ray_pickable<class_CollisionObject3D_property_input_ray_pickable>`       | ``true``  |
+--------------------------------------------------------+--------------------------------------------------------------------------------------+-----------+

Methods
-------

+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`_input_event<class_CollisionObject3D_method__input_event>` **(** :ref:`Camera3D<class_Camera3D>` camera, :ref:`InputEvent<class_InputEvent>` event, :ref:`Vector3<class_Vector3>` position, :ref:`Vector3<class_Vector3>` normal, :ref:`int<class_int>` shape_idx **)** |virtual| |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                 | :ref:`create_shape_owner<class_CollisionObject3D_method_create_shape_owner>` **(** :ref:`Object<class_Object>` owner **)**                                                                                                                                                              |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`               | :ref:`get_collision_layer_value<class_CollisionObject3D_method_get_collision_layer_value>` **(** :ref:`int<class_int>` layer_number **)** |const|                                                                                                                                       |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`               | :ref:`get_collision_mask_value<class_CollisionObject3D_method_get_collision_mask_value>` **(** :ref:`int<class_int>` layer_number **)** |const|                                                                                                                                         |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`RID<class_RID>`                 | :ref:`get_rid<class_CollisionObject3D_method_get_rid>` **(** **)** |const|                                                                                                                                                                                                              |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Array<class_Array>`             | :ref:`get_shape_owners<class_CollisionObject3D_method_get_shape_owners>` **(** **)**                                                                                                                                                                                                    |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`               | :ref:`is_shape_owner_disabled<class_CollisionObject3D_method_is_shape_owner_disabled>` **(** :ref:`int<class_int>` owner_id **)** |const|                                                                                                                                               |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`remove_shape_owner<class_CollisionObject3D_method_remove_shape_owner>` **(** :ref:`int<class_int>` owner_id **)**                                                                                                                                                                 |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`set_collision_layer_value<class_CollisionObject3D_method_set_collision_layer_value>` **(** :ref:`int<class_int>` layer_number, :ref:`bool<class_bool>` value **)**                                                                                                                |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`set_collision_mask_value<class_CollisionObject3D_method_set_collision_mask_value>` **(** :ref:`int<class_int>` layer_number, :ref:`bool<class_bool>` value **)**                                                                                                                  |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                 | :ref:`shape_find_owner<class_CollisionObject3D_method_shape_find_owner>` **(** :ref:`int<class_int>` shape_index **)** |const|                                                                                                                                                          |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`shape_owner_add_shape<class_CollisionObject3D_method_shape_owner_add_shape>` **(** :ref:`int<class_int>` owner_id, :ref:`Shape3D<class_Shape3D>` shape **)**                                                                                                                      |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`shape_owner_clear_shapes<class_CollisionObject3D_method_shape_owner_clear_shapes>` **(** :ref:`int<class_int>` owner_id **)**                                                                                                                                                     |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Object<class_Object>`           | :ref:`shape_owner_get_owner<class_CollisionObject3D_method_shape_owner_get_owner>` **(** :ref:`int<class_int>` owner_id **)** |const|                                                                                                                                                   |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Shape3D<class_Shape3D>`         | :ref:`shape_owner_get_shape<class_CollisionObject3D_method_shape_owner_get_shape>` **(** :ref:`int<class_int>` owner_id, :ref:`int<class_int>` shape_id **)** |const|                                                                                                                   |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                 | :ref:`shape_owner_get_shape_count<class_CollisionObject3D_method_shape_owner_get_shape_count>` **(** :ref:`int<class_int>` owner_id **)** |const|                                                                                                                                       |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                 | :ref:`shape_owner_get_shape_index<class_CollisionObject3D_method_shape_owner_get_shape_index>` **(** :ref:`int<class_int>` owner_id, :ref:`int<class_int>` shape_id **)** |const|                                                                                                       |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Transform3D<class_Transform3D>` | :ref:`shape_owner_get_transform<class_CollisionObject3D_method_shape_owner_get_transform>` **(** :ref:`int<class_int>` owner_id **)** |const|                                                                                                                                           |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`shape_owner_remove_shape<class_CollisionObject3D_method_shape_owner_remove_shape>` **(** :ref:`int<class_int>` owner_id, :ref:`int<class_int>` shape_id **)**                                                                                                                     |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`shape_owner_set_disabled<class_CollisionObject3D_method_shape_owner_set_disabled>` **(** :ref:`int<class_int>` owner_id, :ref:`bool<class_bool>` disabled **)**                                                                                                                   |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`shape_owner_set_transform<class_CollisionObject3D_method_shape_owner_set_transform>` **(** :ref:`int<class_int>` owner_id, :ref:`Transform3D<class_Transform3D>` transform **)**                                                                                                  |
+---------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Signals
-------

.. _class_CollisionObject3D_signal_input_event:

- **input_event** **(** :ref:`Node<class_Node>` camera, :ref:`InputEvent<class_InputEvent>` event, :ref:`Vector3<class_Vector3>` position, :ref:`Vector3<class_Vector3>` normal, :ref:`int<class_int>` shape_idx **)**

Emitted when the object receives an unhandled :ref:`InputEvent<class_InputEvent>`. ``position`` is the location in world space of the mouse pointer on the surface of the shape with index ``shape_idx`` and ``normal`` is the normal vector of the surface at that point.

----

.. _class_CollisionObject3D_signal_mouse_entered:

- **mouse_entered** **(** **)**

Emitted when the mouse pointer enters any of this object's shapes.

----

.. _class_CollisionObject3D_signal_mouse_exited:

- **mouse_exited** **(** **)**

Emitted when the mouse pointer exits all this object's shapes.

Enumerations
------------

.. _enum_CollisionObject3D_DisableMode:

.. _class_CollisionObject3D_constant_DISABLE_MODE_REMOVE:

.. _class_CollisionObject3D_constant_DISABLE_MODE_MAKE_STATIC:

.. _class_CollisionObject3D_constant_DISABLE_MODE_KEEP_ACTIVE:

enum **DisableMode**:

- **DISABLE_MODE_REMOVE** = **0** --- When :ref:`Node.process_mode<class_Node_property_process_mode>` is set to :ref:`Node.PROCESS_MODE_DISABLED<class_Node_constant_PROCESS_MODE_DISABLED>`, remove from the physics simulation to stop all physics interactions with this ``CollisionObject3D``.

Automatically re-added to the physics simulation when the :ref:`Node<class_Node>` is processed again.

- **DISABLE_MODE_MAKE_STATIC** = **1** --- When :ref:`Node.process_mode<class_Node_property_process_mode>` is set to :ref:`Node.PROCESS_MODE_DISABLED<class_Node_constant_PROCESS_MODE_DISABLED>`, make the body static. Doesn't affect :ref:`Area2D<class_Area2D>`. :ref:`PhysicsBody3D<class_PhysicsBody3D>` can't be affected by forces or other bodies while static.

Automatically set :ref:`PhysicsBody3D<class_PhysicsBody3D>` back to its original mode when the :ref:`Node<class_Node>` is processed again.

- **DISABLE_MODE_KEEP_ACTIVE** = **2** --- When :ref:`Node.process_mode<class_Node_property_process_mode>` is set to :ref:`Node.PROCESS_MODE_DISABLED<class_Node_constant_PROCESS_MODE_DISABLED>`, do not affect the physics simulation.

Property Descriptions
---------------------

.. _class_CollisionObject3D_property_collision_layer:

- :ref:`int<class_int>` **collision_layer**

+-----------+----------------------------+
| *Default* | ``1``                      |
+-----------+----------------------------+
| *Setter*  | set_collision_layer(value) |
+-----------+----------------------------+
| *Getter*  | get_collision_layer()      |
+-----------+----------------------------+

The physics layers this CollisionObject3D **is in**. Collision objects can exist in one or more of 32 different layers. See also :ref:`collision_mask<class_CollisionObject3D_property_collision_mask>`.

**Note:** Object A can detect a contact with object B only if object B is in any of the layers that object A scans. See `Collision layers and masks <../tutorials/physics/physics_introduction.html#collision-layers-and-masks>`__ in the documentation for more information.

----

.. _class_CollisionObject3D_property_collision_mask:

- :ref:`int<class_int>` **collision_mask**

+-----------+---------------------------+
| *Default* | ``1``                     |
+-----------+---------------------------+
| *Setter*  | set_collision_mask(value) |
+-----------+---------------------------+
| *Getter*  | get_collision_mask()      |
+-----------+---------------------------+

The physics layers this CollisionObject3D **scans**. Collision objects can scan one or more of 32 different layers. See also :ref:`collision_layer<class_CollisionObject3D_property_collision_layer>`.

**Note:** Object A can detect a contact with object B only if object B is in any of the layers that object A scans. See `Collision layers and masks <../tutorials/physics/physics_introduction.html#collision-layers-and-masks>`__ in the documentation for more information.

----

.. _class_CollisionObject3D_property_disable_mode:

- :ref:`DisableMode<enum_CollisionObject3D_DisableMode>` **disable_mode**

+-----------+-------------------------+
| *Default* | ``0``                   |
+-----------+-------------------------+
| *Setter*  | set_disable_mode(value) |
+-----------+-------------------------+
| *Getter*  | get_disable_mode()      |
+-----------+-------------------------+

Defines the behavior in physics when :ref:`Node.process_mode<class_Node_property_process_mode>` is set to :ref:`Node.PROCESS_MODE_DISABLED<class_Node_constant_PROCESS_MODE_DISABLED>`. See :ref:`DisableMode<enum_CollisionObject3D_DisableMode>` for more details about the different modes.

----

.. _class_CollisionObject3D_property_input_capture_on_drag:

- :ref:`bool<class_bool>` **input_capture_on_drag**

+-----------+----------------------------------+
| *Default* | ``false``                        |
+-----------+----------------------------------+
| *Setter*  | set_capture_input_on_drag(value) |
+-----------+----------------------------------+
| *Getter*  | get_capture_input_on_drag()      |
+-----------+----------------------------------+

If ``true``, the ``CollisionObject3D`` will continue to receive input events as the mouse is dragged across its shapes.

----

.. _class_CollisionObject3D_property_input_ray_pickable:

- :ref:`bool<class_bool>` **input_ray_pickable**

+-----------+-------------------------+
| *Default* | ``true``                |
+-----------+-------------------------+
| *Setter*  | set_ray_pickable(value) |
+-----------+-------------------------+
| *Getter*  | is_ray_pickable()       |
+-----------+-------------------------+

If ``true``, the ``CollisionObject3D``'s shapes will respond to :ref:`RayCast3D<class_RayCast3D>`\ s.

Method Descriptions
-------------------

.. _class_CollisionObject3D_method__input_event:

- void **_input_event** **(** :ref:`Camera3D<class_Camera3D>` camera, :ref:`InputEvent<class_InputEvent>` event, :ref:`Vector3<class_Vector3>` position, :ref:`Vector3<class_Vector3>` normal, :ref:`int<class_int>` shape_idx **)** |virtual|

Receives unhandled :ref:`InputEvent<class_InputEvent>`\ s. ``position`` is the location in world space of the mouse pointer on the surface of the shape with index ``shape_idx`` and ``normal`` is the normal vector of the surface at that point. Connect to the :ref:`input_event<class_CollisionObject3D_signal_input_event>` signal to easily pick up these events.

----

.. _class_CollisionObject3D_method_create_shape_owner:

- :ref:`int<class_int>` **create_shape_owner** **(** :ref:`Object<class_Object>` owner **)**

Creates a new shape owner for the given object. Returns ``owner_id`` of the new owner for future reference.

----

.. _class_CollisionObject3D_method_get_collision_layer_value:

- :ref:`bool<class_bool>` **get_collision_layer_value** **(** :ref:`int<class_int>` layer_number **)** |const|

Returns whether or not the specified layer of the :ref:`collision_layer<class_CollisionObject3D_property_collision_layer>` is enabled, given a ``layer_number`` between 1 and 32.

----

.. _class_CollisionObject3D_method_get_collision_mask_value:

- :ref:`bool<class_bool>` **get_collision_mask_value** **(** :ref:`int<class_int>` layer_number **)** |const|

Returns whether or not the specified layer of the :ref:`collision_mask<class_CollisionObject3D_property_collision_mask>` is enabled, given a ``layer_number`` between 1 and 32.

----

.. _class_CollisionObject3D_method_get_rid:

- :ref:`RID<class_RID>` **get_rid** **(** **)** |const|

Returns the object's :ref:`RID<class_RID>`.

----

.. _class_CollisionObject3D_method_get_shape_owners:

- :ref:`Array<class_Array>` **get_shape_owners** **(** **)**

Returns an :ref:`Array<class_Array>` of ``owner_id`` identifiers. You can use these ids in other methods that take ``owner_id`` as an argument.

----

.. _class_CollisionObject3D_method_is_shape_owner_disabled:

- :ref:`bool<class_bool>` **is_shape_owner_disabled** **(** :ref:`int<class_int>` owner_id **)** |const|

If ``true``, the shape owner and its shapes are disabled.

----

.. _class_CollisionObject3D_method_remove_shape_owner:

- void **remove_shape_owner** **(** :ref:`int<class_int>` owner_id **)**

Removes the given shape owner.

----

.. _class_CollisionObject3D_method_set_collision_layer_value:

- void **set_collision_layer_value** **(** :ref:`int<class_int>` layer_number, :ref:`bool<class_bool>` value **)**

Based on ``value``, enables or disables the specified layer in the :ref:`collision_layer<class_CollisionObject3D_property_collision_layer>`, given a ``layer_number`` between 1 and 32.

----

.. _class_CollisionObject3D_method_set_collision_mask_value:

- void **set_collision_mask_value** **(** :ref:`int<class_int>` layer_number, :ref:`bool<class_bool>` value **)**

Based on ``value``, enables or disables the specified layer in the :ref:`collision_mask<class_CollisionObject3D_property_collision_mask>`, given a ``layer_number`` between 1 and 32.

----

.. _class_CollisionObject3D_method_shape_find_owner:

- :ref:`int<class_int>` **shape_find_owner** **(** :ref:`int<class_int>` shape_index **)** |const|

Returns the ``owner_id`` of the given shape.

----

.. _class_CollisionObject3D_method_shape_owner_add_shape:

- void **shape_owner_add_shape** **(** :ref:`int<class_int>` owner_id, :ref:`Shape3D<class_Shape3D>` shape **)**

Adds a :ref:`Shape3D<class_Shape3D>` to the shape owner.

----

.. _class_CollisionObject3D_method_shape_owner_clear_shapes:

- void **shape_owner_clear_shapes** **(** :ref:`int<class_int>` owner_id **)**

Removes all shapes from the shape owner.

----

.. _class_CollisionObject3D_method_shape_owner_get_owner:

- :ref:`Object<class_Object>` **shape_owner_get_owner** **(** :ref:`int<class_int>` owner_id **)** |const|

Returns the parent object of the given shape owner.

----

.. _class_CollisionObject3D_method_shape_owner_get_shape:

- :ref:`Shape3D<class_Shape3D>` **shape_owner_get_shape** **(** :ref:`int<class_int>` owner_id, :ref:`int<class_int>` shape_id **)** |const|

Returns the :ref:`Shape3D<class_Shape3D>` with the given id from the given shape owner.

----

.. _class_CollisionObject3D_method_shape_owner_get_shape_count:

- :ref:`int<class_int>` **shape_owner_get_shape_count** **(** :ref:`int<class_int>` owner_id **)** |const|

Returns the number of shapes the given shape owner contains.

----

.. _class_CollisionObject3D_method_shape_owner_get_shape_index:

- :ref:`int<class_int>` **shape_owner_get_shape_index** **(** :ref:`int<class_int>` owner_id, :ref:`int<class_int>` shape_id **)** |const|

Returns the child index of the :ref:`Shape3D<class_Shape3D>` with the given id from the given shape owner.

----

.. _class_CollisionObject3D_method_shape_owner_get_transform:

- :ref:`Transform3D<class_Transform3D>` **shape_owner_get_transform** **(** :ref:`int<class_int>` owner_id **)** |const|

Returns the shape owner's :ref:`Transform3D<class_Transform3D>`.

----

.. _class_CollisionObject3D_method_shape_owner_remove_shape:

- void **shape_owner_remove_shape** **(** :ref:`int<class_int>` owner_id, :ref:`int<class_int>` shape_id **)**

Removes a shape from the given shape owner.

----

.. _class_CollisionObject3D_method_shape_owner_set_disabled:

- void **shape_owner_set_disabled** **(** :ref:`int<class_int>` owner_id, :ref:`bool<class_bool>` disabled **)**

If ``true``, disables the given shape owner.

----

.. _class_CollisionObject3D_method_shape_owner_set_transform:

- void **shape_owner_set_transform** **(** :ref:`int<class_int>` owner_id, :ref:`Transform3D<class_Transform3D>` transform **)**

Sets the :ref:`Transform3D<class_Transform3D>` of the given shape owner.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`