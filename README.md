# Bpy-Logic-Bricks-Book
A book to all Bpy logic brick needs.
# Chapter 1: Creating the logic bricks!
## Sensor
Create: 
```bpy.ops.logic.sensor_add(type="",name='')```

Type:
* ACTUATOR
* ALWAYS
* COLLISION
* DELAY
* JOYSTICK
* KEYBOARD
* MESSAGE
* MOUSE
* MOVEMENT
* NEAR
* PROPERTY
* RADAR
* RANDOM
* RAY

## Controller
Create: 
```bpy.ops.logic.controller_add(type="",name='')```

Type:
* LOGIC_AND
* LOGIC_OR
* LOGIC_NAND
* LOGIC_NOR
* LOGIC_XOR
* LOGIC_XNOR
* EXPRESSION
* PYTHON

## Actuator
Create: 
```bpy.ops.logic.actuator_add(type="",name='')```

Type:
* ACTION
* CAMERA
* CONSTRAINT
* EDIT_OBJECT
* FILTER_2D
* GAME
* MESSAGE
* MOUSE 
* MOTION
* PARENT
* PROPERTY
* RANDOM
* SCENE
* COLLECTION
* STEERING
* SOUND
* STATE
* VIBRATION
* VISIBILITY

# Chapter 2: Editing the Sensors!
Choose Logic Brick:
```bpy.context.object.game.sensors['test'].```

Actuator:
* Actuator: ```bpy.context.object.game.sensors[''].actuator = ''```

Always: 
* Nothing

Collision:
* Use Material: ```bpy.context.object.game.sensors[''].use_material = True/False``` 
* Use Pulse: ```bpy.context.object.game.sensors[''].use_pulse = True/False```
* Material: ```bpy.context.object.game.sensors[''].material = ''```
* Property: ```bpy.context.object.game.sensors[''].property = ''```

Delay:
* Delay: ```bpy.context.object.game.sensors[''].delay = int value```
* Duration: ```bpy.context.object.game.sensors[''].duration = int value```
* Use Repeat: ```bpy.context.object.game.sensors[''].use_repeat = True/False```

Joystick: 
* Joystick Index: ```bpy.context.object.game.sensors[''].joystick_index = 0-7```
* Event Type: ```bpy.context.object.game.sensors[''].event_type = 'STICK_DIRECTIONS', '', '', ''```:
  * Stick Directions:
    * All Events: ```bpy.context.object.game.sensors[''].use_all_events = True/False```
    * Stick: ```bpy.context.object.game.sensors[''].axis_number = 'LEFT_STICK/RIGHT_STICK'
