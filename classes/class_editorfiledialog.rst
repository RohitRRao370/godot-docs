:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/EditorFileDialog.xml.

.. _class_EditorFileDialog:

EditorFileDialog
================

**Inherits:** :ref:`ConfirmationDialog<class_ConfirmationDialog>` **<** :ref:`AcceptDialog<class_AcceptDialog>` **<** :ref:`Window<class_Window>` **<** :ref:`Viewport<class_Viewport>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

A modified version of :ref:`FileDialog<class_FileDialog>` used by the editor.

.. rst-class:: classref-introduction-group

Description
-----------

**EditorFileDialog** is an enhanced version of :ref:`FileDialog<class_FileDialog>` available only to editor plugins. Additional features include list of favorited/recent files and the ability to see files as thumbnails grid instead of list.

Unlike :ref:`FileDialog<class_FileDialog>`, **EditorFileDialog** does not have a property for using native dialogs. Instead, native dialogs can be enabled globally via the :ref:`EditorSettings.interface/editor/use_native_file_dialogs<class_EditorSettings_property_interface/editor/use_native_file_dialogs>` editor setting. They are also enabled automatically when running in sandbox (e.g. on macOS).

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`Access<enum_EditorFileDialog_Access>`           | :ref:`access<class_EditorFileDialog_property_access>`                                       | ``0``                                                                                    |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`String<class_String>`                           | :ref:`current_dir<class_EditorFileDialog_property_current_dir>`                             |                                                                                          |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`String<class_String>`                           | :ref:`current_file<class_EditorFileDialog_property_current_file>`                           |                                                                                          |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`String<class_String>`                           | :ref:`current_path<class_EditorFileDialog_property_current_path>`                           |                                                                                          |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                               | dialog_hide_on_ok                                                                           | ``false`` (overrides :ref:`AcceptDialog<class_AcceptDialog_property_dialog_hide_on_ok>`) |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                               | :ref:`disable_overwrite_warning<class_EditorFileDialog_property_disable_overwrite_warning>` | ``false``                                                                                |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`DisplayMode<enum_EditorFileDialog_DisplayMode>` | :ref:`display_mode<class_EditorFileDialog_property_display_mode>`                           | ``0``                                                                                    |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`FileMode<enum_EditorFileDialog_FileMode>`       | :ref:`file_mode<class_EditorFileDialog_property_file_mode>`                                 | ``4``                                                                                    |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`PackedStringArray<class_PackedStringArray>`     | :ref:`filters<class_EditorFileDialog_property_filters>`                                     | ``PackedStringArray()``                                                                  |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                                 | :ref:`option_count<class_EditorFileDialog_property_option_count>`                           | ``0``                                                                                    |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                               | :ref:`show_hidden_files<class_EditorFileDialog_property_show_hidden_files>`                 | ``false``                                                                                |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+
   | :ref:`String<class_String>`                           | title                                                                                       | ``"Save a File"`` (overrides :ref:`Window<class_Window_property_title>`)                 |
   +-------------------------------------------------------+---------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                            | :ref:`add_filter<class_EditorFileDialog_method_add_filter>`\ (\ filter\: :ref:`String<class_String>`, description\: :ref:`String<class_String>` = ""\ )                                                        |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                            | :ref:`add_option<class_EditorFileDialog_method_add_option>`\ (\ name\: :ref:`String<class_String>`, values\: :ref:`PackedStringArray<class_PackedStringArray>`, default_value_index\: :ref:`int<class_int>`\ ) |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                            | :ref:`add_side_menu<class_EditorFileDialog_method_add_side_menu>`\ (\ menu\: :ref:`Control<class_Control>`, title\: :ref:`String<class_String>` = ""\ )                                                        |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                            | :ref:`clear_filename_filter<class_EditorFileDialog_method_clear_filename_filter>`\ (\ )                                                                                                                        |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                            | :ref:`clear_filters<class_EditorFileDialog_method_clear_filters>`\ (\ )                                                                                                                                        |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`String<class_String>`                       | :ref:`get_filename_filter<class_EditorFileDialog_method_get_filename_filter>`\ (\ ) |const|                                                                                                                    |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`LineEdit<class_LineEdit>`                   | :ref:`get_line_edit<class_EditorFileDialog_method_get_line_edit>`\ (\ )                                                                                                                                        |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                             | :ref:`get_option_default<class_EditorFileDialog_method_get_option_default>`\ (\ option\: :ref:`int<class_int>`\ ) |const|                                                                                      |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`String<class_String>`                       | :ref:`get_option_name<class_EditorFileDialog_method_get_option_name>`\ (\ option\: :ref:`int<class_int>`\ ) |const|                                                                                            |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedStringArray<class_PackedStringArray>` | :ref:`get_option_values<class_EditorFileDialog_method_get_option_values>`\ (\ option\: :ref:`int<class_int>`\ ) |const|                                                                                        |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Dictionary<class_Dictionary>`               | :ref:`get_selected_options<class_EditorFileDialog_method_get_selected_options>`\ (\ ) |const|                                                                                                                  |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`VBoxContainer<class_VBoxContainer>`         | :ref:`get_vbox<class_EditorFileDialog_method_get_vbox>`\ (\ )                                                                                                                                                  |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                            | :ref:`invalidate<class_EditorFileDialog_method_invalidate>`\ (\ )                                                                                                                                              |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                            | :ref:`popup_file_dialog<class_EditorFileDialog_method_popup_file_dialog>`\ (\ )                                                                                                                                |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                            | :ref:`set_filename_filter<class_EditorFileDialog_method_set_filename_filter>`\ (\ filter\: :ref:`String<class_String>`\ )                                                                                      |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                            | :ref:`set_option_default<class_EditorFileDialog_method_set_option_default>`\ (\ option\: :ref:`int<class_int>`, default_value_index\: :ref:`int<class_int>`\ )                                                 |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                            | :ref:`set_option_name<class_EditorFileDialog_method_set_option_name>`\ (\ option\: :ref:`int<class_int>`, name\: :ref:`String<class_String>`\ )                                                                |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                            | :ref:`set_option_values<class_EditorFileDialog_method_set_option_values>`\ (\ option\: :ref:`int<class_int>`, values\: :ref:`PackedStringArray<class_PackedStringArray>`\ )                                    |
   +---------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Signals
-------

.. _class_EditorFileDialog_signal_dir_selected:

.. rst-class:: classref-signal

**dir_selected**\ (\ dir\: :ref:`String<class_String>`\ ) :ref:`🔗<class_EditorFileDialog_signal_dir_selected>`

Emitted when a directory is selected.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_signal_file_selected:

.. rst-class:: classref-signal

**file_selected**\ (\ path\: :ref:`String<class_String>`\ ) :ref:`🔗<class_EditorFileDialog_signal_file_selected>`

Emitted when a file is selected.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_signal_filename_filter_changed:

.. rst-class:: classref-signal

**filename_filter_changed**\ (\ filter\: :ref:`String<class_String>`\ ) :ref:`🔗<class_EditorFileDialog_signal_filename_filter_changed>`

Emitted when the filter for file names changes.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_signal_files_selected:

.. rst-class:: classref-signal

**files_selected**\ (\ paths\: :ref:`PackedStringArray<class_PackedStringArray>`\ ) :ref:`🔗<class_EditorFileDialog_signal_files_selected>`

Emitted when multiple files are selected.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Enumerations
------------

.. _enum_EditorFileDialog_FileMode:

.. rst-class:: classref-enumeration

enum **FileMode**: :ref:`🔗<enum_EditorFileDialog_FileMode>`

.. _class_EditorFileDialog_constant_FILE_MODE_OPEN_FILE:

.. rst-class:: classref-enumeration-constant

:ref:`FileMode<enum_EditorFileDialog_FileMode>` **FILE_MODE_OPEN_FILE** = ``0``

The **EditorFileDialog** can select only one file. Accepting the window will open the file.

.. _class_EditorFileDialog_constant_FILE_MODE_OPEN_FILES:

.. rst-class:: classref-enumeration-constant

:ref:`FileMode<enum_EditorFileDialog_FileMode>` **FILE_MODE_OPEN_FILES** = ``1``

The **EditorFileDialog** can select multiple files. Accepting the window will open all files.

.. _class_EditorFileDialog_constant_FILE_MODE_OPEN_DIR:

.. rst-class:: classref-enumeration-constant

:ref:`FileMode<enum_EditorFileDialog_FileMode>` **FILE_MODE_OPEN_DIR** = ``2``

The **EditorFileDialog** can select only one directory. Accepting the window will open the directory.

.. _class_EditorFileDialog_constant_FILE_MODE_OPEN_ANY:

.. rst-class:: classref-enumeration-constant

:ref:`FileMode<enum_EditorFileDialog_FileMode>` **FILE_MODE_OPEN_ANY** = ``3``

The **EditorFileDialog** can select a file or directory. Accepting the window will open it.

.. _class_EditorFileDialog_constant_FILE_MODE_SAVE_FILE:

.. rst-class:: classref-enumeration-constant

:ref:`FileMode<enum_EditorFileDialog_FileMode>` **FILE_MODE_SAVE_FILE** = ``4``

The **EditorFileDialog** can select only one file. Accepting the window will save the file.

.. rst-class:: classref-item-separator

----

.. _enum_EditorFileDialog_Access:

.. rst-class:: classref-enumeration

enum **Access**: :ref:`🔗<enum_EditorFileDialog_Access>`

.. _class_EditorFileDialog_constant_ACCESS_RESOURCES:

.. rst-class:: classref-enumeration-constant

:ref:`Access<enum_EditorFileDialog_Access>` **ACCESS_RESOURCES** = ``0``

The **EditorFileDialog** can only view ``res://`` directory contents.

.. _class_EditorFileDialog_constant_ACCESS_USERDATA:

.. rst-class:: classref-enumeration-constant

:ref:`Access<enum_EditorFileDialog_Access>` **ACCESS_USERDATA** = ``1``

The **EditorFileDialog** can only view ``user://`` directory contents.

.. _class_EditorFileDialog_constant_ACCESS_FILESYSTEM:

.. rst-class:: classref-enumeration-constant

:ref:`Access<enum_EditorFileDialog_Access>` **ACCESS_FILESYSTEM** = ``2``

The **EditorFileDialog** can view the entire local file system.

.. rst-class:: classref-item-separator

----

.. _enum_EditorFileDialog_DisplayMode:

.. rst-class:: classref-enumeration

enum **DisplayMode**: :ref:`🔗<enum_EditorFileDialog_DisplayMode>`

.. _class_EditorFileDialog_constant_DISPLAY_THUMBNAILS:

.. rst-class:: classref-enumeration-constant

:ref:`DisplayMode<enum_EditorFileDialog_DisplayMode>` **DISPLAY_THUMBNAILS** = ``0``

The **EditorFileDialog** displays resources as thumbnails.

.. _class_EditorFileDialog_constant_DISPLAY_LIST:

.. rst-class:: classref-enumeration-constant

:ref:`DisplayMode<enum_EditorFileDialog_DisplayMode>` **DISPLAY_LIST** = ``1``

The **EditorFileDialog** displays resources as a list of filenames.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_EditorFileDialog_property_access:

.. rst-class:: classref-property

:ref:`Access<enum_EditorFileDialog_Access>` **access** = ``0`` :ref:`🔗<class_EditorFileDialog_property_access>`

.. rst-class:: classref-property-setget

- |void| **set_access**\ (\ value\: :ref:`Access<enum_EditorFileDialog_Access>`\ )
- :ref:`Access<enum_EditorFileDialog_Access>` **get_access**\ (\ )

The location from which the user may select a file, including ``res://``, ``user://``, and the local file system.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_current_dir:

.. rst-class:: classref-property

:ref:`String<class_String>` **current_dir** :ref:`🔗<class_EditorFileDialog_property_current_dir>`

.. rst-class:: classref-property-setget

- |void| **set_current_dir**\ (\ value\: :ref:`String<class_String>`\ )
- :ref:`String<class_String>` **get_current_dir**\ (\ )

The currently occupied directory.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_current_file:

.. rst-class:: classref-property

:ref:`String<class_String>` **current_file** :ref:`🔗<class_EditorFileDialog_property_current_file>`

.. rst-class:: classref-property-setget

- |void| **set_current_file**\ (\ value\: :ref:`String<class_String>`\ )
- :ref:`String<class_String>` **get_current_file**\ (\ )

The currently selected file.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_current_path:

.. rst-class:: classref-property

:ref:`String<class_String>` **current_path** :ref:`🔗<class_EditorFileDialog_property_current_path>`

.. rst-class:: classref-property-setget

- |void| **set_current_path**\ (\ value\: :ref:`String<class_String>`\ )
- :ref:`String<class_String>` **get_current_path**\ (\ )

The file system path in the address bar.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_disable_overwrite_warning:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **disable_overwrite_warning** = ``false`` :ref:`🔗<class_EditorFileDialog_property_disable_overwrite_warning>`

.. rst-class:: classref-property-setget

- |void| **set_disable_overwrite_warning**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_overwrite_warning_disabled**\ (\ )

If ``true``, the **EditorFileDialog** will not warn the user before overwriting files.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_display_mode:

.. rst-class:: classref-property

:ref:`DisplayMode<enum_EditorFileDialog_DisplayMode>` **display_mode** = ``0`` :ref:`🔗<class_EditorFileDialog_property_display_mode>`

.. rst-class:: classref-property-setget

- |void| **set_display_mode**\ (\ value\: :ref:`DisplayMode<enum_EditorFileDialog_DisplayMode>`\ )
- :ref:`DisplayMode<enum_EditorFileDialog_DisplayMode>` **get_display_mode**\ (\ )

The view format in which the **EditorFileDialog** displays resources to the user.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_file_mode:

.. rst-class:: classref-property

:ref:`FileMode<enum_EditorFileDialog_FileMode>` **file_mode** = ``4`` :ref:`🔗<class_EditorFileDialog_property_file_mode>`

.. rst-class:: classref-property-setget

- |void| **set_file_mode**\ (\ value\: :ref:`FileMode<enum_EditorFileDialog_FileMode>`\ )
- :ref:`FileMode<enum_EditorFileDialog_FileMode>` **get_file_mode**\ (\ )

The dialog's open or save mode, which affects the selection behavior.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_filters:

.. rst-class:: classref-property

:ref:`PackedStringArray<class_PackedStringArray>` **filters** = ``PackedStringArray()`` :ref:`🔗<class_EditorFileDialog_property_filters>`

.. rst-class:: classref-property-setget

- |void| **set_filters**\ (\ value\: :ref:`PackedStringArray<class_PackedStringArray>`\ )
- :ref:`PackedStringArray<class_PackedStringArray>` **get_filters**\ (\ )

The available file type filters. For example, this shows only ``.png`` and ``.gd`` files: ``set_filters(PackedStringArray(["*.png ; PNG Images","*.gd ; GDScript Files"]))``. Multiple file types can also be specified in a single filter. ``"*.png, *.jpg, *.jpeg ; Supported Images"`` will show both PNG and JPEG files when selected.

**Note:** The returned array is *copied* and any changes to it will not update the original property value. See :ref:`PackedStringArray<class_PackedStringArray>` for more details.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_option_count:

.. rst-class:: classref-property

:ref:`int<class_int>` **option_count** = ``0`` :ref:`🔗<class_EditorFileDialog_property_option_count>`

.. rst-class:: classref-property-setget

- |void| **set_option_count**\ (\ value\: :ref:`int<class_int>`\ )
- :ref:`int<class_int>` **get_option_count**\ (\ )

The number of additional :ref:`OptionButton<class_OptionButton>`\ s and :ref:`CheckBox<class_CheckBox>`\ es in the dialog.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_property_show_hidden_files:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **show_hidden_files** = ``false`` :ref:`🔗<class_EditorFileDialog_property_show_hidden_files>`

.. rst-class:: classref-property-setget

- |void| **set_show_hidden_files**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_showing_hidden_files**\ (\ )

If ``true``, hidden files and directories will be visible in the **EditorFileDialog**. This property is synchronized with :ref:`EditorSettings.filesystem/file_dialog/show_hidden_files<class_EditorSettings_property_filesystem/file_dialog/show_hidden_files>`.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_EditorFileDialog_method_add_filter:

.. rst-class:: classref-method

|void| **add_filter**\ (\ filter\: :ref:`String<class_String>`, description\: :ref:`String<class_String>` = ""\ ) :ref:`🔗<class_EditorFileDialog_method_add_filter>`

Adds a comma-separated file name ``filter`` option to the **EditorFileDialog** with an optional ``description``, which restricts what files can be picked.

A ``filter`` should be of the form ``"filename.extension"``, where filename and extension can be ``*`` to match any string. Filters starting with ``.`` (i.e. empty filenames) are not allowed.

For example, a ``filter`` of ``"*.tscn, *.scn"`` and a ``description`` of ``"Scenes"`` results in filter text "Scenes (\*.tscn, \*.scn)".

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_add_option:

.. rst-class:: classref-method

|void| **add_option**\ (\ name\: :ref:`String<class_String>`, values\: :ref:`PackedStringArray<class_PackedStringArray>`, default_value_index\: :ref:`int<class_int>`\ ) :ref:`🔗<class_EditorFileDialog_method_add_option>`

Adds an additional :ref:`OptionButton<class_OptionButton>` to the file dialog. If ``values`` is empty, a :ref:`CheckBox<class_CheckBox>` is added instead.

\ ``default_value_index`` should be an index of the value in the ``values``. If ``values`` is empty it should be either ``1`` (checked), or ``0`` (unchecked).

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_add_side_menu:

.. rst-class:: classref-method

|void| **add_side_menu**\ (\ menu\: :ref:`Control<class_Control>`, title\: :ref:`String<class_String>` = ""\ ) :ref:`🔗<class_EditorFileDialog_method_add_side_menu>`

Adds the given ``menu`` to the side of the file dialog with the given ``title`` text on top. Only one side menu is allowed.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_clear_filename_filter:

.. rst-class:: classref-method

|void| **clear_filename_filter**\ (\ ) :ref:`🔗<class_EditorFileDialog_method_clear_filename_filter>`

Clear the filter for file names.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_clear_filters:

.. rst-class:: classref-method

|void| **clear_filters**\ (\ ) :ref:`🔗<class_EditorFileDialog_method_clear_filters>`

Removes all filters except for "All Files (\*.\*)".

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_get_filename_filter:

.. rst-class:: classref-method

:ref:`String<class_String>` **get_filename_filter**\ (\ ) |const| :ref:`🔗<class_EditorFileDialog_method_get_filename_filter>`

Returns the value of the filter for file names.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_get_line_edit:

.. rst-class:: classref-method

:ref:`LineEdit<class_LineEdit>` **get_line_edit**\ (\ ) :ref:`🔗<class_EditorFileDialog_method_get_line_edit>`

Returns the LineEdit for the selected file.

\ **Warning:** This is a required internal node, removing and freeing it may cause a crash. If you wish to hide it or any of its children, use their :ref:`CanvasItem.visible<class_CanvasItem_property_visible>` property.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_get_option_default:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_option_default**\ (\ option\: :ref:`int<class_int>`\ ) |const| :ref:`🔗<class_EditorFileDialog_method_get_option_default>`

Returns the default value index of the :ref:`OptionButton<class_OptionButton>` or :ref:`CheckBox<class_CheckBox>` with index ``option``.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_get_option_name:

.. rst-class:: classref-method

:ref:`String<class_String>` **get_option_name**\ (\ option\: :ref:`int<class_int>`\ ) |const| :ref:`🔗<class_EditorFileDialog_method_get_option_name>`

Returns the name of the :ref:`OptionButton<class_OptionButton>` or :ref:`CheckBox<class_CheckBox>` with index ``option``.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_get_option_values:

.. rst-class:: classref-method

:ref:`PackedStringArray<class_PackedStringArray>` **get_option_values**\ (\ option\: :ref:`int<class_int>`\ ) |const| :ref:`🔗<class_EditorFileDialog_method_get_option_values>`

Returns an array of values of the :ref:`OptionButton<class_OptionButton>` with index ``option``.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_get_selected_options:

.. rst-class:: classref-method

:ref:`Dictionary<class_Dictionary>` **get_selected_options**\ (\ ) |const| :ref:`🔗<class_EditorFileDialog_method_get_selected_options>`

Returns a :ref:`Dictionary<class_Dictionary>` with the selected values of the additional :ref:`OptionButton<class_OptionButton>`\ s and/or :ref:`CheckBox<class_CheckBox>`\ es. :ref:`Dictionary<class_Dictionary>` keys are names and values are selected value indices.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_get_vbox:

.. rst-class:: classref-method

:ref:`VBoxContainer<class_VBoxContainer>` **get_vbox**\ (\ ) :ref:`🔗<class_EditorFileDialog_method_get_vbox>`

Returns the :ref:`VBoxContainer<class_VBoxContainer>` used to display the file system.

\ **Warning:** This is a required internal node, removing and freeing it may cause a crash. If you wish to hide it or any of its children, use their :ref:`CanvasItem.visible<class_CanvasItem_property_visible>` property.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_invalidate:

.. rst-class:: classref-method

|void| **invalidate**\ (\ ) :ref:`🔗<class_EditorFileDialog_method_invalidate>`

Notify the **EditorFileDialog** that its view of the data is no longer accurate. Updates the view contents on next view update.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_popup_file_dialog:

.. rst-class:: classref-method

|void| **popup_file_dialog**\ (\ ) :ref:`🔗<class_EditorFileDialog_method_popup_file_dialog>`

Shows the **EditorFileDialog** at the default size and position for file dialogs in the editor, and selects the file name if there is a current file.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_set_filename_filter:

.. rst-class:: classref-method

|void| **set_filename_filter**\ (\ filter\: :ref:`String<class_String>`\ ) :ref:`🔗<class_EditorFileDialog_method_set_filename_filter>`

Sets the value of the filter for file names.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_set_option_default:

.. rst-class:: classref-method

|void| **set_option_default**\ (\ option\: :ref:`int<class_int>`, default_value_index\: :ref:`int<class_int>`\ ) :ref:`🔗<class_EditorFileDialog_method_set_option_default>`

Sets the default value index of the :ref:`OptionButton<class_OptionButton>` or :ref:`CheckBox<class_CheckBox>` with index ``option``.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_set_option_name:

.. rst-class:: classref-method

|void| **set_option_name**\ (\ option\: :ref:`int<class_int>`, name\: :ref:`String<class_String>`\ ) :ref:`🔗<class_EditorFileDialog_method_set_option_name>`

Sets the name of the :ref:`OptionButton<class_OptionButton>` or :ref:`CheckBox<class_CheckBox>` with index ``option``.

.. rst-class:: classref-item-separator

----

.. _class_EditorFileDialog_method_set_option_values:

.. rst-class:: classref-method

|void| **set_option_values**\ (\ option\: :ref:`int<class_int>`, values\: :ref:`PackedStringArray<class_PackedStringArray>`\ ) :ref:`🔗<class_EditorFileDialog_method_set_option_values>`

Sets the option values of the :ref:`OptionButton<class_OptionButton>` with index ``option``.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
