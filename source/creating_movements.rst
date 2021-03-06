.. _creating_movements:

Creating Movements
==================
Each scene has a series of objects that can be moved and transformed: they are xsheet columns and pegbars, table and cameras.

Every movement or transformation you set for an object at a specific frame automatically defines a key position. When keys are defined at different frames, in-between positions are automatically interpolated.

To create more complex animation, you can also work in a 3D environment, where camera and scene elements can be placed like on a stage at different distances one from another.




.. _using_the_stage_schematic:

Using the Stage Schematic
-------------------------
The stage schematic contains all the objects used in a scene, making it possible to manage the way they are linked to each other. It is organized in a hierarchy starting from the animation table, where all the pegbars and columns are placed. A camera is available as well, and other cameras can be defined.

By default the stage schematic contains one camera, the table, pegbar 1 and 2, and column 1 and 2 nodes, linked in the following way: column 1 is linked to pegbar 1, and this is linked to the table; column 2 is linked to pegbar 2, and this is linked to the table.

Columns are added as soon as you load or create some content for them; new pegbars and cameras can be added at any time. Any other column you use will be linked by default to pegbar 2; new pegbars will be automatically linked to the table.

When more than one camera is defined, you can set which is the current camera used in the work area; the current camera is displayed in blue while the others are left idle in grey. Each camera can have a different size and resolution, and each of them can be animated independently (see  :ref:`Defining Camera Settings <defining_camera_settings>`  ).

Objects can be easily added and arranged, and they can be selected in order to be cut, copied, pasted or deleted. When selected, objects are highlighted in white; the current object has its label in red; when at least one object is selected, the related links are displayed in blue.

It is also possible to group several objects in one single node, in order to better manage the whole stage schematic. Groups can be opened to be examined, and its components can be selected for further operations, like creating animations, or new groups.

.. note:: Column nodes have the camera stand ( |Toonz71_267| ) and the render (

 |Toonz71_268| ) toggles on the top right: these toggles are the same as the toggles available in the xsheet column headers (see 

:ref:`Working with Xsheet Columns <working_with_xsheet_columns>`  ).



.. tip:: **To access the stage schematic:**

    Click the schematic toggle button ( |Toonz71_269| ) in the bottom bar of a schematic window until the title bar displays Stage Schematic.



.. tip:: **To navigate the stage schematic:**

    Do one of the following:

    - Use the mouse wheel, or the zoom shortcut keys (by default + and - keys) to zoom in and zoom out.

    - Middle-click and drag to scroll in any direction.

    - Use the Fit to Window button ( |Toonz71_270| ) in the bottom bar of the stage window to display all the objects in the current window.



    - Use the Focus on Current button ( |Toonz71_271| ) in the bottom bar of the stage window to center the stage on the current object.

    - Use the Reset Size button ( |Toonz71_272| ) in the bottom bar of the stage window, or use the reset view shortcut (by default the 0 key) to display all the objects at the default size.

.. tip:: **To add a column:**

    Load or create some content for the xsheet column: it will be automatically displayed in the stage.

.. tip:: **To add a pegbar:**

    Do one of the following:

    - Click the New Pegbar button ( |Toonz71_273| ) in the bottom bar of the stage window.



    - Right-click in the stage and choose New Pegbar from the menu that opens.

.. tip:: **To add a camera:**

    Do one of the following:

    - Click the New Camera button ( |Toonz71_274| ) in the bottom bar of the stage window.



    - Right-click in the stage and choose New Camera from the menu that opens.

.. tip:: **To set the current camera:**

    In the stage right-click the camera you want to set as current and choose Activate from the menu that opens.

.. tip:: **To name an object:**

    Double-click the object name and type a new name.

.. tip:: **To minimize/maximize the column nodes:**

    Do one of the following: 

    - Click the arrowhead next to the column name to minimize/maximize columns selectively.

    - Click the Minimize/Maximize ( |Toonz71_275| /

 |Toonz71_276| ) button in the bottom bar of the stage window to minimize/maximize all the column nodes.



.. tip:: **To select objects and links:**

    Do one of the following:

    - Click to select an object.

    - Click and drag to select a group of objects.

    - Ctrl-click (PC) or Cmd-click (Mac) to add an object to, or remove it from the selection.

.. note:: Links can be selected together with objects (see  :ref:`Linking Objects <linking_objects>`  ).

.. tip:: **To move the selection:**

    Click and drag any object of the selection.

.. tip:: **To edit an objects selection:**

    Do one of the following:

    - Use the Copy command to keep the selection in memory for further operations.

    - Use the Cut command to eliminate the selection from the schematic and keep it in memory for further operations.

    - Use the Paste command to paste the selection kept in memory in the stage schematic: the pasted selection is linked to the same object to which the copied or cut objects were linked. 

    - Use the Delete command to delete the selection.

.. note:: All these commands are available in the menu that opens when right-clicking nodes and links. 

.. note:: The table, the default cameras, pegbars 1 and 2, and columns 1 and 2 cannot be removed from the schematic.

.. tip:: **To group selected objects:**

    Right-click any selected object and choose Group from the menu that opens.

.. note:: Objects can only be grouped if they share a parent object, and the parent object is included in the selection.

.. tip:: **To open a group:**

    Right-click the group and choose Open Group from the menu that opens: the group objects are displayed in a box, showing links between group nodes, and links with nodes outside of the group. 

.. note:: In the stage schematic, when the content of a group is displayed it is not possible to edit the links between group objects, and links with objects outside of the group.

.. tip:: **To close a group:**

    Click the close button on the right of the group box bar. 

.. tip:: **To release a group:**

    Right-click the group and choose Ungroup from the menu that opens.

.. tip:: **To reorder nodes in the stage schematic:**

    Click the Reorder Nodes button ( |Toonz71_277| ) in the bottom bar of the stage window.



.. _linking_objects:

Linking Objects
---------------
Objects can be linked in order to create shared movements, that is to say a movement that all the linked objects share with the parent object, and relative movements, that is to say a movement that is the sum of the object own movement and the movement of its parent object. 

As parent objects can be linked in their turn to other moving objects, it is possible to define a complex hierarchy of movements.

The hierarchy between objects can be edited by setting links that allow you to set parent and linked objects: columns can be linked to other columns, pegbars, table and cameras; pegbars can be linked to other pegbars, table and cameras; cameras can be linked to any object in order to create complex shots, for example with a camera following the movement of a character in the scene.

Links can be set by using ports located around the object node: 

- The port on the left is for linking the object to another object.

- The port on the right is for accepting links from other objects.

- The port at the bottom is for assigning a motion path to the object (see for  :ref:`Creating a Movement along a Motion Path <creating_a_movement_along_a_motion_path>`  s).

Links can also be selected in order to be deleted: when selected, links are highlighted in white; when at least one object is selected, the related links are displayed in blue.

Columns and pegbars are always linked, at least to the table: this means that their links cannot be deleted, but only replaced with different ones or restored to their default, i.e. pegbars to the table and columns to the pegbar 2.

Letters displayed on the ports set the center of the object: center B is the geometrical center of each object, while center A is placed 8 inches to the left and center C, 8 inches to the right, etc. When a link is created, the letters at its ends set the way the linked object overlaps the parent object. If at both ends of the link you set the same letter, the two object overlap with no offset; while if, for example, a column centered on B is linked to a pegbar center A, it will have an offset of 8 inches to the left.

Each object has always a free port in order to accept a link to a different center. In this way if you want to link another object to the same parent object, you can choose whether to use the same center or a new one.

.. note:: Apart from the letters, columns have number centers as well for setting hook centers (see  :ref:`Using Hooks <using_hooks>`  ).

.. note:: By defining parent and linked objects you can also create cutout animation (see  :ref:`Creating Cutout Animation <creating_cutout_animation>`  ).

.. tip:: **To link an object to another:**

    In the stage, click and drag the object left port to the parent object right port.

.. tip:: **To set the center of an object:**

    1. Place the pointer on the object left port and wait for the double-arrow button to appear.

    2. Click and drag up or down the double-arrow button to scroll the options available: letters and numbers for columns, and letters for all the other objects.

.. tip:: **To set the way a linked object overlaps the parent object:**

    Do any of the following:

    - Set the same letter for the two ports at the end of a link to overlap the objects without an offset.

    - Set the following letter in the alphabetical order on the left port of the linked object to offset it to the right: for each letter there is an offset of 8 inches to the right.

    - Set the previous letter in the alphabetical order on the linked object left port to offset it to the left: for each letter there is an offset of 8 inches to the left.

.. tip:: **To link a column to another object:**

    Do any of the following:

    - To link a column to any other object, define the link in the schematic.

    - To link a column to a pegbar or another column, choose the object and the center in the column header of the xsheet.

    - To link a column to another column, select the Edit tool ( |Toonz71_278| ) with the Pick option to Column, and in the work area shift-click the column contents to which you want to link the current column.



.. tip:: **To select the linked object to edit in the hierarchy:**

    Do one of the following:

    - Select it in the stage schematic. 

    - Use the Edit tool ( |Toonz71_279| ) with the Pick option set to Pegbar to click a drawing in the work area and select the first pegbar in the hierarchy the column containing the drawing is linked to.



    - Right-click in the work area a drawing to choose from the menu that opens the Select command related to the object hierarchically linked that you want to edit, from the first one up to the table.

.. note:: The right-click menu first lists all the columns containing overlapping drawings, then the columns and objects that are hierarchically linked to the clicked one.

.. tip:: **To select links:**

    Do one of the following:

    - Click to select a link.

    - Click and drag to select several links.

    - Ctrl-click (PC) or Cmd-click (Mac) to add a link to, or remove it from the selection.

.. note:: Objects can be selected together with links (see  :ref:`Using the Stage Schematic <using_the_stage_schematic>`  ).

.. tip:: **To remove selected links:**

    Choose Edit > Delete: links will be replaced by default ones, i.e pegbars will be linked to the table and columns to the pegbar 2.

.. _using_hooks:

Using Hooks
'''''''''''
Hooks are reference points that can be defined for any animation level directly in the work area by using the Hook tool ( |Toonz71_280| ).



Once defined they can be used in the stage schematic to link an object to the column where the hooked level is exposed according to a specific hook set, or to move the column according to any of its hook sets.

In the first case the hook is used as a tracking point to link an object, for example another column or a camera, to a specific feature of the animation level. For example, if you have a character carrying a lamp, you can track the lamp position with a hook set and link a radial gradient to it to create a glow placed over the lamp for every frame of the animation.

In the second case the hook is used as the center of the column where the hooked level is exposed, thus creating a different center and offset for each level frame. For example, if you have a walking animation cycle, you can set a new center following the character’s feet with a hook set, and make the level move accordingly to prevent a moon-walking effect on the background. 

Hooks can also be split and passed from one drawing feature to another, automatically creating an offset position. For example the hook following the character’s foot feature can pass from one foot to another, in order to make the character move continuously onward.




A hook set can be created starting from any frame. Once it is created, it will appear on the following level frames in the same position, from where it can be moved.

You can use up to 20 hook sets for each level; each hook set is labeled with a number, to retrieve it in each level frame. 

By activating the Snap option, hooks for the current level can be placed by snapping them exactly in the same position of hooks defined for the other animation levels visible in the work area. In case the current level is a Toonz vector level, hooks will snap also at the center of any closed shapes it may contain (e.g. rectangles, circles or single vector shapes closed with the Tape tool). This option may prove useful especially when defining hooks for cutout animation models (see  :ref:`Creating Cutout Animation <creating_cutout_animation>`  ).

Hook information is saved along with the level as a file in XML format named as the file with the _hooks suffix. For example, hooks defined for the level ``mouse``  will be saved in the file ``mouse_hooks.xml`` .

.. note:: Hooks are also visible in onion skin mode (see  :ref:`Using Onion Skin <using_onion_skin>`  ).

.. note:: Hooks can be also used to create a cutout animation model, as they allows you to link the model sections according to specific pivot points (see  :ref:`Creating Cutout Animation <creating_cutout_animation>`  ).

.. tip:: **To define a hook set for a level:**

    1. Select a frame from the level you want to set hooks for.

    2. Choose the Hook tool ( |Toonz71_282| ).

    3. Do one of the following:

    - Click to create a hook set and drag to define the hook starting position.

    - Click elsewhere to create another hook set and the related hook starting position.

.. tip:: **To select hooks:**

    Do one of the following:

    - Click a hook to select it.

    - Ctrl-click (PC) or Cmd-click (Mac) to add a hook to, or remove it from the selection.

.. tip:: **To move selected hooks:**

    Do one of the following:

    - Drag them to a new position.

    - Shift-drag to constrain an horizontal or vertical movement.

    - Activate the Snap option to place the hook exactly in the same position of hooks defined for other animation levels visible in the work area, or in case the level is a Toonz vector level, at the center of closed shapes.

.. tip:: **To pass a hook from one position to another:**

    1. Alt-click and drag the hook to split it in two.

    2. Place the double circle where the hook has to be for the current frame.

    3. Place the cross where you want the reference point to be from the next frame onwards.

.. tip:: **To delete a hook set:**

    Select the related hook in any frame and choose Edit > Delete.

.. tip:: **To link an object to a level hook set:**

    1. Link the object to the column where the hooked level is exposed.

    2. Place the pointer on the column right port and wait for the double-arrow button to appear.

    3. Click and drag up the double-arrow button to scroll the numbers available before letter A, and release the mouse button to define the hook set to be used.

.. tip:: **To make the level move according to one of its hook set:**

    1. Place the pointer left port of the column where the level is exposed, and wait for the double-arrow button to appear.

    2. Click and drag up the double-arrow button to scroll the numbers available before letter A, and release the mouse button to define the hook set to be used.

.. tip:: **To prevent an animation walking cycle from moon-walking:**

    Define a hook set by following these guidelines:

    - Place the hook on the same foot feature along the whole sequence, for example the tip of the foot.

    - If the character is supposed to be moving horizontally on the ground, the hook should always lie on the ground line without changing its vertical position along the sequence. If the feature you are following leaves the ground, place the hook on the ground line, under the feature you were following.

    - When both feet are on the ground line you can split the hook to pass it form one foot to the other.

    - If the animation is a cycle and you want the character to keep on walking, the last hook position has to be connected to the first and the hook has to pass from one foot to the other by splitting it, and then to the first one by splitting it again. 

.. _tracking_points:

Tracking Points
'''''''''''''''
It is possible to automatically track specific regions in a sequence of images by using the Tracker tool ( |Toonz71_284| ). The results of the tool are a series of hooks that can be used to link an object to another (see above).



When selected the Tracker tool ( |Toonz71_285| ) allows you to define one or several regions in an image by defining a center and a size; regions can also be connected to one another to better track points having a visual geometrical relationship. The region defined with the tool defines both the pattern that the tracking system will try to recognize in the following images, and the size of the area where it will look for it (approximately twice the region).



Once areas to be tracked are defined in the first frame of a range, it is possible to automatically tracks the regions in a selected range, by specifying the following options:

- Threshold sets the amount of difference between the defined pattern and the recognized one. When using low values, the tracking system will look for an area with an almost identical pattern, and when using high values, for an area that can be quite different from the original one. This means that if the value is too low, it’s likely the tracking will fail on certain images; if too high, the tracking may follow the wrong areas. 

- Sensitivity sets how often the defined pattern has to be updated according to the variation it may have in the following images. For the maximum value, the pattern will be updated after each image is tracked.

- Variable Region Size, when activated, will look for the defined pattern considering also the different sizes that it can have in the following images. 

- Include Background, when activated, considers the background as part of the defined pattern. It can be deactivated when tracking an element whose background does not affect the pattern, such as a blue screen background.

.. tip:: **To define a region to be tracked:**

    1. Choose the Tracker tool () and click and drag in the image.

    2. Use the handles along the defined region bounding box to resize it.

    3. Click and drag elsewhere to define a second region: the center of the region will be labelled with a different letter.

.. tip:: **To define a region connected to another one:**

    1. Choose the Tracker tool () and select the region to which you want to connect another region.

    2. Click and drag elsewhere to define a connected region: the center of the region will be labelled with the same letter of the first one.

.. tip:: **To delete a defined region:**

    1. Choose the Tracker tool () and select the region you want to delete.

    2. Choose Edit > Delete.

.. tip:: **To track a defined region in a series of images:**

    1. Select the first image of the range you want to track.

    2. Choose the Tracker tool ( |Toonz71_289| ) and define the regions to be tracked.

    3. Select the frame range in the xsheet or in the level strip.

    4. Choose Level > Tracking, set the tracking options and click the Track button.

.. tip:: **To link an object to the tracked region:**

    Link the object to the hook automatically defined by the tracking process (see  :ref:`Using Hooks <using_hooks>`  ).

.. _animating_objects:

Animating Objects
-----------------
You can edit, move, rotate, scale and shear columns, pegbars, the table and cameras by using the Edit tool ( |Toonz71_290| ). Objects to be animated can be selected in the stage schematic, in the work area and in the xsheet.



In the tool options bar you can set the following:

- An option button ( |Toonz71_291| ) lets you set which tool options have to be displayed in the bar.



    - Pick lets you choose if you want to select automatically the column or pegbar to be animated by clicking it in the viewer: when set to column, clicking a drawing automatically selects the related column; when set to pegbar, clicking a drawing automatically selects the pegbar to which the column containing the drawing is linked.

    - Position N/S and E/W sets the vertical and horizontal positions of the selected object, position Z sets the position along the Z axis (see  :ref:`Working in a 3D Environment <working_in_a_3d_environment>`  ), and position SO sets the column stacking order that can be different from the one defined in the xsheet (see  :ref:`Changing Columns Stacking Order <changing_columns_stacking_order>`  ).

    - Rotation sets the rotation of the selected object.

    - Scale Global, H and V sets the global, horizontal and vertical scaling of the selected object. Maintain sets the constraint for scaling operations performed by using the Edit tool handle: if it is set to A/R the object will maintain its proportions, if it is set to Mass the object will maintain its overall size even when changing proportions.

    - Shear H and V sets the horizontal and vertical shearing of the selected object.

    - Center N/S and E/W sets the vertical and horizontal position of the center of the selected object. 

    - Global Key when activated sets a key for all the object transformations as soon as a key for one transformation is set by using the Edit tool handle. For example if you change the position of an object, thus defining a key position, automatically a key will be defined for the rotation, scaling and shearing transformations as well.

    - A lock button ( |Toonz71_292| ) defines which transformations have to be locked while transforming the object.

.. note:: If the tool options bar is too short to display all the tool options, it can be scrolled by using arrow buttons available at its ends.

.. note:: Position values are expressed in the default unit of measure set in the Preferences > Interface dialog (see  :ref:`Choosing the Working Unit <choosing_the_working_unit>`  ).

To control interactively transformation values you can also use the handle available in the work area. The handle is made of an inner double circle with three arms that allows you to perform the following transformations:

- Click and drag the circle end to rotate the object;

- Click and drag the outer square of the double-square end to scale the object uniformly on the vertical and horizontal; click and drag the inner square of the double-square end to scale the object according to the constraint set in the options bar; if no constraint is set and the Shift key is pressed while dragging, the scaling will be uniform.

- Click and drag the parallelogram end to shear the object; if the Shift key is pressed while dragging, the shearing will be constrained in the horizontal or vertical direction.

- Click and drag the double circle at the center to change the center of the object.

.. note:: The object center can be moved, but cannot change its position during the animation: once it is set, or modified, it is retained during all of the animation. If the center is changed many times, and you want to set it back to its original position, right-click the object in the schematic and choose Reset Center from the menu that opens.

- Click and drag anywhere to move the object; if the Shift key is pressed while dragging, the movement will be constrained in the horizontal or vertical direction.

.. note:: As you roll over the handles, the cursor changes shape to indicate to you the operations you may perform. 

When entering a value or operating the handle, a key position will be automatically generated at the current frame only for the set transformation; if the Global Key option is activated, keys will be generated for all of the transformations.

If you want to set a key for an object transformation leaving its value as it is at the current frame, you can just hit Enter on the displayed value; if the Global Key option is activated, keys will be generated for all of the transformations. If you want to set keys for all of the object transformations leaving their values as they are at the current frame, you can use the Set Key button ( |Toonz71_293| ) available in the bottom bar of the viewer; in this case keys are created for all of the object transformations regardless of the Global Key option.



.. note:: Objects can also be animated by working in the Function Editor (see  :ref:`Editing Curves and Numerical Columns <editing_curves_and_numerical_columns>`  ).

.. note:: The movement of the column contents can be checked by activating the onion skin mode, as it will display the position of drawings contained in the current column at different frames (see  :ref:`Using Onion Skin <using_onion_skin>`  ).

.. tip:: **To select the object to edit:**

    1. Do one of the following:

    - Select it in the stage schematic. 

    - If the object is a column, select it in the xsheet.

    - Use the Edit tool ( |Toonz71_294| ) with the Pick option set to Column to click a drawing in the work area to select the related column.

    - Use the Edit tool ( |Toonz71_295| ) with the Pick option set to Pegbar to click a drawing in the work area to select the pegbar that the column containing the drawing is linked to.

    - Right-click in the work area a drawing to select an object from the list of the objects hierarchically linked to the column containing the drawing, from the first one up to the table and current camera (see  :ref:`Linking Objects <linking_objects>`  ). 

.. tip:: **To animate an object with the Edit tool:**

    1. Select the object you want to edit.

    2. Choose the Edit tool ( |Toonz71_296| ). 

    3. Set the frame where you want to define the key by doing one of the following:

    - Move the current frame cursor in the xsheet or in the function editor.

    - Use the frame bar or the playback buttons in the bottom bar of the work area.

    - When animating columns only, select the related cell in the column.

    4. Define a key position.

    5. Select a different frame, and go on defining key positions.

.. tip:: **To define a key position only for some object transformations:**

    1. Deactivate the Global Key option in the tool options bar.

    2. Do one of the following:

    - Enter values in the Edit tool options bar for the object transformations you want to set a key for. 

    - Operate the handle to move, scale, rotate or shear the object, automatically generating a key only for the modified transformation. 

.. note:: As this key position is partial and refers only to some transformations, the Set Key button turns striped-blue.

.. tip:: **To define a key position for all the object transformations:**

    1. Activate the Global Key option in the tool options bar.

    2. Do one of the following:

    - Enter values you want to modify in the Edit tool options bar. 

    - Operate the handle to move, scale, rotate or shear the object. 

.. note:: As this key position is global and refers to all the transformations, the Set Key button turns blue.

.. tip:: **To define a key for an object transformation leaving its value as it is at the current frame:**

    1. Deactivate the Global Key option in the tool options bar.

    2. In the Edit tool options bar click in the field of the object transformations you want to set a key for, and press the Enter key. 

.. note:: As this key position is partial and refers only to some transformations, the Set Key button turns striped-blue.

.. tip:: **To define keys for all of the object transformations leaving their values as they are at the current frame:**

    Do one of the following:

    - Activate the Global Key option in the tool options bar, click in any object transformations field, and press the Enter key.

    - Click the Set Key button ( |Toonz71_297| ).



    - When animating columns only, right-click in the column cell and choose Set Key from the menu that opens. 

.. note:: As this key position is global and refers to all the transformations, the Set Key button turns blue.

.. tip:: **To turn a partial key position to a global key:**

    Click the Set Key button ( |Toonz71_298| ): it turns from blue-striped to blue.



.. tip:: **To remove a set key position from the viewer bottom bar:**

    Do one of the following:

    - If the key position is global, click the Set Key button ( |Toonz71_299| ): it turns from blue to grey.



    - If the key position is partial, click twice the Set Key button ( |Toonz71_300| ): with the first click it turns from striped-blue to blue, with the second from blue to grey.

.. tip:: **To navigate frames where key positions are defined in the viewer bottom bar:**

    Use the Next ( |Toonz71_301| ) and Previous Key buttons (

 |Toonz71_302| ) available at the side of the Set Key button.



.. note:: Keys can also be removed or navigated by working in the Function Editor (see  :ref:`Editing Curves and Numerical Columns <editing_curves_and_numerical_columns>`  ).

.. tip:: **To customize the Edit tool options bar:**

    Do any of the following:

    - Use the option button ( |Toonz71_303| ) to choose which tool options have to be displayed: only selected items will be displayed.



    - Use the lock button ( |Toonz71_304| ) to choose which transformations have to be locked while transforming the object: only selected items will be locked.

.. _changing_columns_stacking_order:

Changing Columns Stacking Order
'''''''''''''''''''''''''''''''
The column stacking order, which sets which drawings and images are placed on top, or behind, other images, by default depends on how columns are placed in the xsheet: its direction is from left to right, making what is on the left is behind what is on the right. 

This means that if an animation element has to move behind another animation element, and then in front of it, it has to be exposed in two different columns, one before and one after the column containing the second animation element.

By editing the position SO (i.e. stacking order) value it is possible to change and animate the stacking order without editing the columns position in the xsheet.

The SO default value for all the columns is 0, meaning that the xsheet column order is taken into account when there are no modifications of the SO position. As soon as a column has a higher SO value, it will be placed on top, regardless of the position of the column in the xsheet; if the value is lower it will be placed behind.

.. note:: In case the columns Z position is edited, columns closer to the camera are displayed on top of the others, ignoring both the xsheet stacking order and the SO value (see  :ref:`Working in a 3D Environment <working_in_a_3d_environment>`  ).

.. tip:: **To edit and animate the columns SO value:**

    1. Select the column to which you want to edit the SO value.

    2. Choose the Edit tool ( |Toonz71_305| ). 

    3. Set the frame where you want to define the key.

    4. In the tool options bar enter the value in the SO position field.

.. note:: Columns SO values can also be edited and animated by working in the Function Editor (see  :ref:`Editing Curves and Numerical Columns <editing_curves_and_numerical_columns>`  ).

.. _creating_a_movement_along_a_motion_path:

Creating a Movement along a Motion Path
'''''''''''''''''''''''''''''''''''''''
Objects can be moved along a motion path according to two different type of movements: one without changing the object orientation, and the other with an automatic orientation set according to the direction of the motion path.

A motion path can be assigned to an object in the stage schematic, and it can be defined with drawing tools and edited in the work area as if it was a vector. Once defined it is displayed as a dashed red line, with small numbers indicating the control points defining the vector shape.

 |Toonz71_306| 

As soon as a path is assigned to an object, the object will be automatically placed at the beginning of the path according to its center, and it will only be able to move along it, and not in the E/W and N/S directions anymore.

The key positions of the object on the motion path can be defined by dragging the object along it, and they are expressed as a percentage where 0 is the starting point and 100 is the ending point of the path. 

It is also possible to link the key positions of the objects to the positions of the control points defining the motion path, so that they remain consistent when the motion path is edited. To help you better understand where the control points are, the object snaps to them when it is dragged along the motion path.

.. note:: If you want to change the center of the object, you can move it with the Edit tool ( |Toonz71_307| ) and then use the Reset Center command in the stage.



.. note:: A motion path can also be created by copying and pasting a drawing vector, and a drawing vector can be created by copying and pasting a motion path.

.. tip:: **To create a motion path:**

    1. Select the object for which you want to define a motion path.

    2. Do one of the following:

    - Click the New Motion Path button ( |Toonz71_308| ) in the bottom bar of the stage window.

    - Right-click in the stage and choose New Motion Path from the menu that opens.

.. tip:: **To define and edit a motion path:**

    Select the motion path in the stage and do any of the following:

    - Use the drawing tools to define it in the work area.

    - Use the modifier tools to edit it. 

    - Draw a new line, and confirm in the dialog that opens, to replace a previously created motion path with a new one. 

.. tip:: **To assign a motion path to an object:**

    Click and drag the motion path top port to the object bottom port. 

.. tip:: **To remove a motion path from an object:**

    1. Select the link between the object and the motion path. 

    2. Choose Edit > Delete.

.. tip:: **To set the type of movement along a motion path:**

    Click the button at the far left of the object bottom port to switch between two options: the square ( |Toonz71_309| ) will preserve the object original orientation, and the rotated square (

 |Toonz71_310| ) will automatically rotate the object according to the motion path direction.



.. tip:: **To link the object key positions to the control points defining the motion path:**

    Click the button at the left of the object bottom port to activate or deactivate the Link to Control Points option ( |Toonz71_311| ).



.. tip:: **To change the center of the object:**

    1. Choose the Edit tool ().

    2. Move the center of the object to the new position.

    3. Right-click the object in the stage and select Reset Center from the menu that opens.

.. tip:: **To save a motion path:**

    1. Right-click it and select Save Motion Path from the menu that opens. 

    2. In the browser choose a location and a name and click the Save button. The file will be saved with the MPATH extension.

.. tip:: **To load a motion path:**

    1. Right-click the motion path and select Load Motion Path from the menu that opens. 

    2. In the browser retrieve the MPATH file you want to load and click the Load button.

.. tip:: **To use a drawing vector as a motion path:**

    1. Select the vector you want to use as a motion path with the Selection tool ().

    2. Copy/cut it.

    3. Select the motion path you want to paste to in the stage.

    4. Click in the work area and paste the copied/cut vector that automatically becomes a motion path.

.. tip:: **To use a motion path as a vector:**

    1. Select the motion path in the stage.

    2. Select the motion path with the Selection tool ( |Toonz71_314| ) in the work area.

    3. Copy/cut it.

    4. Select the drawing where you want to paste the new vector.

    5. Paste the copied/cut motion path that automatically becomes a vector.

.. tip:: **To remove a motion path from the stage:**

    Do one of the following:

    - Select the motion path node and choose Edit > Delete.

    - Right-click the motion path node and choose Delete from the menu that opens.

.. _using_column_keys:

Using Column Keys
-----------------
When columns are animated, their animation can be controlled in a quick way by managing key positions and interpolations directly in the xsheet, with no need to use the function editor.

As soon as a key position is defined for a column, a related icon is displayed on the right of the column cell to which it refers; the key is displayed regardless of how many parameters are animated. Keys can be moved within the column they refer to, and selected in order to be copied/cut and pasted from one cell to another. 




When the Global Key option is activated for the Edit tool, and the default interpolation is not set to Linear, as soon as at least two key positions are created for a column a vertical line connecting them with two arrowheads is displayed (see  :ref:`Animating Objects <animating_objects>`  and  :ref:`Setting Segment Interpolations <setting_segment_interpolations>`  ). The two arrowheads divide the line into three sections indicating the speed in, the constant speed and speed out phases of all the transformations defined for the movement. This allows you to control the speed of the movement between the two keys as you wish, including a constant speed movement.

You can also cycle previously created keys, in order to repeat automatically all the previously defined keys for the whole length of the scene, with no need to copy and paste keys from cells to cells.

All animations and interpolations set for the column can be visible and edited with the function editor. When you edit any column transformation in the function editor, the arrowheads will not be displayed anymore between keys, to stress the fact that a specific interpolation has been modified with the function editor. If needed you can reset the whole column transformation to the default interpolation values, and make the arrowheads available again (see  :ref:`Editing Curves and Numerical Columns <editing_curves_and_numerical_columns>`  ). 

.. tip:: **To modify a key:**

    1. Select the cell the key refers to.

    2. Do one of the following:

    - Use the Edit tool ( |Toonz71_316| ) to modify position and size.

    - Enter values you want to modify in the Edit tool ( |Toonz71_317| ) options bar. 

.. tip:: **To select keys:**

    Do one of the following:

    - Click a key icon to select it.

    - Click a key icon and drag to select a range of keys on different columns and at different frames.

    - Shift-click to extend the selection to a specific key. 

    - Ctrl-click (PC) or Cmd-click (Mac) to add to, or remove a key to the selection.

    - Right-click a key icon and choose the related command from the menu that opens to perform specific selections, such as all keys in the row, all previous ones, all following ones, etc.

.. tip:: **To move a key selection:**

    Click any of the selected keys and drag the selection to the new position. Dragging is allowed only vertically.

.. tip:: **To edit a key selection:**

    Do one of the following:

    - Use the Copy command to keep the selection in memory for further operations.

    - Use the Cut command to eliminate the selection from the scene and keep it in memory for further operations.

    - Use the Paste command to paste the selection kept in memory starting from the selected cell. 

    - Use the Delete command to delete the selection.

.. note:: All these commands are also available in the menu that opens when right-clicking the key icon.

.. tip:: **To set the speed of the movement or transformation:**

    Click the arrowheads available on the vertical line connecting two subsequent keys, and drag them up or down to the new position. In particular:

    - To set a constant speed, drag the top arrowhead close to the first key icon to eliminate the ease in section, and the bottom arrowhead close to the second key icon to eliminate the ease out section.

    - To set a continuous acceleration, drag both arrowheads close to the second key icon in order to increase the speed in section.

    - To set a continuous deceleration, drag both arrowheads close to the first key icon in order to increase the speed out section.

.. tip:: **To make the arrowheads available when they are not:**

    Right-click the vertical line connecting two subsequent keys and choose Reset Interpolation from the menu that opens.

.. tip:: **To activate/deactivate the cycling of previously created keys:**

    Click the tab with a circular arrow ( |Toonz71_318| ) visible after the last key of a series.The cells affected by the cycled 

movement are marked on the right by a vertical zigzagged line. 



.. tip:: **To open the function editor:**

    Do one of the following:

    - Double-click a key. 

    - Right-click a key and choose Function Editor from the menu that opens.

.. _working_with_multiple_column_keys:

Working with Multiple Column Keys
'''''''''''''''''''''''''''''''''
It is possible to insert or delete keys affecting the xsheet as a whole, or a selection of xsheet columns. 

Inserting or deleting multiple keys allows you to manage keys for several columns at the same time, for instance when you are working on a cutout animation where keys may be required for all the columns where model sections are exposed (see  :ref:`Creating Cutout Animation <creating_cutout_animation>`  ). 

.. note:: Inserted keys are created for all the column transformations.

When a multiple key is inserted at the current frame, a key is created for each xsheet column where an animation level is exposed; if a column selection is defined, keys are created in selected columns only (see  :ref:`Working with Xsheet Columns <working_with_xsheet_columns>`  ).

When a multiple key is deleted at the current frame, any key available in any xsheet column at the current frame, is deleted; if a column selection is defined, keys are deleted in selected columns only.

.. tip:: **To create several keys at once:**

    1. Do one of the following:

    - Select the columns for which you want to create keys.

    - Select no column by clicking anywhere in the xsheet, to create keys for all the xsheet columns.

    2. Select the frame where you want to insert keys.

    3. Choose Xsheet > Insert Multiple Keys.

.. tip:: **To remove several keys at once:**

    1. Do one of the following:

    - Select the columns from which you want to delete keys.

    - Select no column by clicking anywhere in the xsheet, to delete keys from all the xsheet columns.

    2. Select the frame where you want to delete keys.

    3. Choose Xsheet > Remove Multiple Keys.

.. _working_in_a_3d_environment:

Working in a 3D Environment
---------------------------
You can place and move cameras, the table, pegbars and columns in a 3D environment, as if they were elements on a real 3D stage. 

This means that it is possible to move the camera automatically generating a multiplane effect, or truck it through characters and elements simulating a perspective effect, or create complex 3D motion paths for any element by combining a depth movement with movements in the E/W and N/S directions.

The 3D environment can be activated, or deactivated, with the 3D button ( |Toonz71_319| ) available in the viewer title bar. When activated the viewer displays the cone of the camera and all of the scene contents along the Z axis, which is the direction from the camera to the table. The area displayed can be moved and rotated to set the best viewing angle, and a side or top view can be set. 



By default all the pegbars and columns are on the table: their Z position is equal to the number of horizontal fields defined for the default camera, as the value represents the size of the area that is shot by the camera (see  :ref:`Defining Camera Settings <defining_camera_settings>`  ). By increasing the field value, objects are placed farther from the camera; by decreasing it, objects are placed closer to the camera; at zero they are at the same Z position as the camera and for negative value they are behind the camera.

As concerning the camera, by default its Z position is equal to the number of horizontal fields defined for the default camera. By increasing the field value, the camera moves further from the table; by decreasing it, closer; at zero it is at the same Z position of the table and for negative value it is behind the table.

As soon as objects are moved, projections on an imaginary floor and side wall let you understand the position of the drawings in relation to each other and to the camera. If the current object is a column, a dotted bounding box displays the way the column content will be shot by the camera.

The size of the objects changes according to its Z position, like in a real 3D environment, decreasing when an object is farther from the camera and increasing when closer. To keep control of this behaviour it is possible to define an additional Z position value in the tool options bar that sets the position at which the object has to keep its original size. 

.. note:: Columns closer to the camera are displayed on top of the others, ignoring the xsheet stacking order and the position SO value. In case two or several columns have exactly the same distance, the SO value prevails; if two or several columns have exactly the same distance and SO value, the xsheet stacking order prevails (see  :ref:`Changing Columns Stacking Order <changing_columns_stacking_order>`  ).

.. tip:: **To enter the 3D environment:**

    Click the 3D view button ( |Toonz71_320| ) available on the right of the viewer title bar.



.. tip:: **To set an object position in the 3D environment:**

    1. Activate the 3D view.

    2. Select the object you want to move.

    3. Select the Edit tool ( |Toonz71_321| ).

    4. Do one of the following:

    - Enter a value for the Z position in the tool options bar.

    - Use the double-arrow handle parallel to the floor of the 3D environment to move the selected object and set its Z position.

.. tip:: **To set at which position the object has to keep its original size:**

    Enter a value for the additional Z position field displayed in brackets in the tool options bar. For example if you want a column content to keep its original size when placed at the Z position 8, enter 8 as the value in brackets.

.. tip:: **To move the work area displayed in 3D:**

    Select the Hand tool( |Toonz71_322| ) and drag in the viewer.



.. tip:: **To rotate the work area displayed in 3D:**

    Select the Rotate tool( |Toonz71_323| ) and drag in the viewer.



.. tip:: **To set a side or a top view:**

    Do one of the following:

    - To set a side view use the button ( |Toonz71_324| ) available on the side wall or the 3D environment.



    - To set a top view use the button ( |Toonz71_325| ) available on the floor or the 3D environment.

.. tip:: **To exit the 3D environment:**

    Click the standard ( |Toonz71_326| ) or camera view button (

 |Toonz71_327| ) available on the right of the viewer title bar.



.. |Toonz71_267| image:: /_static/Toonz71/Toonz71_267.gif
.. |Toonz71_268| image:: /_static/Toonz71/Toonz71_268.gif
.. |Toonz71_269| image:: /_static/Toonz71/Toonz71_269.gif
.. |Toonz71_270| image:: /_static/Toonz71/Toonz71_270.gif
.. |Toonz71_271| image:: /_static/Toonz71/Toonz71_271.gif
.. |Toonz71_272| image:: /_static/Toonz71/Toonz71_272.gif
.. |Toonz71_273| image:: /_static/Toonz71/Toonz71_273.gif
.. |Toonz71_274| image:: /_static/Toonz71/Toonz71_274.gif
.. |Toonz71_275| image:: /_static/Toonz71/Toonz71_275.gif
.. |Toonz71_276| image:: /_static/Toonz71/Toonz71_276.gif
.. |Toonz71_277| image:: /_static/Toonz71/Toonz71_277.gif
.. |Toonz71_278| image:: /_static/Toonz71/Toonz71_278.gif
.. |Toonz71_279| image:: /_static/Toonz71/Toonz71_279.gif
.. |Toonz71_280| image:: /_static/Toonz71/Toonz71_280.gif
.. |Toonz71_282| image:: /_static/Toonz71/Toonz71_282.gif
.. |Toonz71_284| image:: /_static/Toonz71/Toonz71_284.gif
.. |Toonz71_285| image:: /_static/Toonz71/Toonz71_285.gif
.. |Toonz71_289| image:: /_static/Toonz71/Toonz71_289.gif
.. |Toonz71_290| image:: /_static/Toonz71/Toonz71_290.gif
.. |Toonz71_291| image:: /_static/Toonz71/Toonz71_291.gif
.. |Toonz71_292| image:: /_static/Toonz71/Toonz71_292.gif
.. |Toonz71_293| image:: /_static/Toonz71/Toonz71_293.gif
.. |Toonz71_294| image:: /_static/Toonz71/Toonz71_294.gif
.. |Toonz71_295| image:: /_static/Toonz71/Toonz71_295.gif
.. |Toonz71_296| image:: /_static/Toonz71/Toonz71_296.gif
.. |Toonz71_297| image:: /_static/Toonz71/Toonz71_297.gif
.. |Toonz71_298| image:: /_static/Toonz71/Toonz71_298.gif
.. |Toonz71_299| image:: /_static/Toonz71/Toonz71_299.gif
.. |Toonz71_300| image:: /_static/Toonz71/Toonz71_300.gif
.. |Toonz71_301| image:: /_static/Toonz71/Toonz71_301.gif
.. |Toonz71_302| image:: /_static/Toonz71/Toonz71_302.gif
.. |Toonz71_303| image:: /_static/Toonz71/Toonz71_303.gif
.. |Toonz71_304| image:: /_static/Toonz71/Toonz71_304.gif
.. |Toonz71_305| image:: /_static/Toonz71/Toonz71_305.gif
.. |Toonz71_306| image:: /_static/Toonz71/Toonz71_306.gif
.. |Toonz71_307| image:: /_static/Toonz71/Toonz71_307.gif
.. |Toonz71_308| image:: /_static/Toonz71/Toonz71_308.gif
.. |Toonz71_309| image:: /_static/Toonz71/Toonz71_309.gif
.. |Toonz71_310| image:: /_static/Toonz71/Toonz71_310.gif
.. |Toonz71_311| image:: /_static/Toonz71/Toonz71_311.gif
.. |Toonz71_314| image:: /_static/Toonz71/Toonz71_314.gif
.. |Toonz71_316| image:: /_static/Toonz71/Toonz71_316.gif
.. |Toonz71_317| image:: /_static/Toonz71/Toonz71_317.gif
.. |Toonz71_318| image:: /_static/Toonz71/Toonz71_318.gif
.. |Toonz71_319| image:: /_static/Toonz71/Toonz71_319.gif
.. |Toonz71_320| image:: /_static/Toonz71/Toonz71_320.gif
.. |Toonz71_321| image:: /_static/Toonz71/Toonz71_321.gif
.. |Toonz71_322| image:: /_static/Toonz71/Toonz71_322.gif
.. |Toonz71_323| image:: /_static/Toonz71/Toonz71_323.gif
.. |Toonz71_324| image:: /_static/Toonz71/Toonz71_324.gif
.. |Toonz71_325| image:: /_static/Toonz71/Toonz71_325.gif
.. |Toonz71_326| image:: /_static/Toonz71/Toonz71_326.gif
.. |Toonz71_327| image:: /_static/Toonz71/Toonz71_327.gif
