- [Sensor](#Sensor)

- [Controller](#Controller)

- [Actuator](#Actuator)


# Chapter 1: Creating the logic bricks!
## Sensor
Create Sensor Logic Brick: 
```bpy.ops.logic.sensor_add(type="", name='')```

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

name: give the brick a unique name for future use

## Controller
Create Controller Logic Brick:
```bpy.ops.logic.controller_add(type="", name='')```

Type:
* LOGIC_AND
* LOGIC_OR
* LOGIC_NAND
* LOGIC_NOR
* LOGIC_XOR
* LOGIC_XNOR
* EXPRESSION
* PYTHON

name: give the brick a unique name for future use

## Actuator
Create Actuator Logic Brick:
```bpy.ops.logic.actuator_add(type="", name='')```

Type:
* ACTION
* CAMERA
* COLLECTION
* CONSTRAINT
* EDIT_OBJECT
* FILTER_2D
* GAME
* MESSAGE
* MOTION
* MOUSE 
* PARENT
* PROPERTY
* RANDOM
* SCENE
* SOUND
* STATE
* STEERING
* VIBRATION
* VISIBILITY

name: give the brick a unique name for future use
