##Z0 Stepper - Front Left
[stepper_z]
step_pin: PF11
dir_pin: PG3
enable_pin: !PG5
rotation_distance: 4    
microsteps: 32
endstop_pin: probe:z_virtual_endstop
##All builds use same Max Z
position_max: 200
position_min: -6
homing_speed: 7.0 # Leadscrews are slower than 2.4, 10 is a recommended max.
second_homing_speed: 3
homing_retract_dist: 3

[tmc2209 stepper_z]
uart_pin: PC6
interpolate: False
run_current: 0.6
sense_resistor: 0.110
stealthchop_threshold: 0

##Z1 Stepper - Rear Center
[stepper_z1]
step_pin: PG4
dir_pin: PC1
enable_pin: !PA0
#Rotation Distance for TR8x8 = 8, TR8x4 = 4, TR8x2 = 2
rotation_distance: 4
microsteps: 32

[tmc2209 stepper_z1]
uart_pin: PC7
interpolate: False
run_current: 0.6
sense_resistor: 0.110
stealthchop_threshold: 0

##Z2 Stepper - Front Right
[stepper_z2]
step_pin: PF9
dir_pin: PF10
enable_pin: !PG2
#Rotation Distance for TR8x8 = 8, TR8x4 = 4, TR8x2 = 2
rotation_distance: 4 
microsteps: 32

[tmc2209 stepper_z2]
uart_pin: PF2
interpolate: False
run_current: 0.6
sense_resistor: 0.110
stealthchop_threshold: 0
