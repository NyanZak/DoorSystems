Door Systems Guide
==================

This documentation describes how to use the `Door Systems` component in
your project.

Behaviours
----------

-   \[`DoorTriggerPressurePlate`\]
-   \[`KeyDoor`\]
-   \[`TriggerDoor`\]
-   \[`TriggerDoorKeyboard`\]
-   \[`UI_KeyHolder`\]

DoorTriggerPressurePlate
------------------------

This behaviour allows the user to use pressure plates to open and close
doors.

### Properties

-   `Door` Reference to the door parent object to get the animator
    component.
-   `timeToStayOpen` this float determines how long the door stays open
    after the user steps off of the pressure plate.

KeyDoor
-------

This behaviour allows the user to destroy a door by having the correct
key equipped and being nearby to the assigned door.

-   `Door` Reference to the door parent object to get the animator
    component.
-   `Key Type` - References the key required in order to open the door.
-   `Open Speed Curve` - Animation for the door opening
-   `Direction` - Determines which direction the door opens.
-   `Open Distance` - Float for how far the door opens.
-   `Open Speed Multiplier` - Float for how fast the door opens.
-   `Door Body` Reference to the door's model to open.

TriggerDoor && TriggerDoorKeyboard
----------------------------------

These scripts allow the player to open the door by being nearby //
pressing a key on the keyboard.

-   `Open Speed Curve` - Animation for the door opening
-   `Direction` - Determines which direction the door opens.
-   `Open Distance` - Float for how far the door opens.
-   `Open Speed Multiplier` - Float for how fast the door opens.
-   `Door Body` Reference to the door's model to open.

Custom Axis is used for the key press, default `K`, editable in the
Input Manager.

UI\_KeyHolder
-------------

This behaviour allows the user to see the keys they currently have in
their inventory, once they open a door the key is removed from the UI.

-   `keyHolder` Reference to the key holder script on the Player.
