# Bpy-Logic-Bricks-Book
A book to all Bpy logic brick needs.


- [Sensor](#Sensor)
  - [Create](#Sensor)
- [Controller](#Controller)
  - [Create](#Controller)
- [Actuator](#Actuator)
  - [Create](#Actuator)

# Chapter 1: Creating the logic bricks!
## Sensor
Create Sensor Logic Brick: 
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
Create Controller Logic Brick:
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
Create Actuator Logic Brick:
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
* Event Type: ```bpy.context.object.game.sensors[''].event_type = 'STICK_DIRECTIONS', 'STICK_AXIS', 'SHOULDER_TRIGGERS', 'BUTTONS'```:
  * Stick Directions:
    * All Events: ```bpy.context.object.game.sensors[''].use_all_events = True/False```
    * Stick: ```bpy.context.object.game.sensors[''].axis_number = 'LEFT_STICK/RIGHT_STICK'```
    * Stick Direction: ```bpy.context.object.game.sensors[''].axis_direction = 'RIGHTAXIS', 'UPAXIS', 'LEFTAXIS', 'DOWNAXIS'```
    * Threshold: ```bpy.context.object.game.sensors[''].axis_threshold = int value```
  * Stick Axis: 
    * Stick Axis: ```bpy.context.object.game.sensors['']single_axis_number = 'LEFT_STICK_HORIZONTAL, LEFT_STICK_VERTICAL, RIGHT_STICK_HORIZONTAL, RIGHT_STICK_VERTICAL'```
    * Threshold: ```bpy.context.object.game.sensors[''].axis_threshold = int value```
  * Shoulder Triggers:
    * Triggers: ```bpy.context.object.game.sensors['test'].axis_trigger_number = 'LEFT_SHOULDER_TRIGGER, RIGHT_SHOULDER_TRIGGER'```
    * Threshold: ```bpy.context.object.game.sensors[''].axis_threshold = int value```
  * Buttons:
    * All Events: ```bpy.context.object.game.sensors[''].use_all_events = True/False```
    * Button: ```bpy.context.object.game.sensors[''].button_number = 'BUTTON_A', 'BUTTON_B', 'BUTTON_X', 'BUTTON_Y', 'BUTTON_BACK', 'BUTTON_GUIDE', 'BUTTON_START', 'BUTTON_STICK_LEFT', 'BUTTON_STICK_RIGHT', 'BUTTON_SHOULDER_LEFT', 'BUTTON_SHOULDER_RIGHT', 'BUTTON_DPAD_UP', 'BUTTON_DPAD_DOWN', 'BUTTON_DPAD_LEFT', 'BUTTON_DPAD_RIGHT'```
     
Keyboard:
* Key: ```bpy.context.object.game.sensors[''].key = 'A-Z, 0-8, NUMPAD_0-8, ect```
https://docs.blender.org/api/blender_python_api_2_77_0/bpy.types.KeyboardSensor.html#bpy.types.KeyboardSensor

