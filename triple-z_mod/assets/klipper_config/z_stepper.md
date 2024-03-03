##Z0 Stepper - Front Left <br>
[stepper_z] <br>
step_pin: PF11 <br>
dir_pin: PG3 <br>
enable_pin: !PG5 <br>
rotation_distance: 4  <br>   
microsteps: 32 <br>
endstop_pin: probe:z_virtual_endstop <br>
##All builds use same Max Z <br>
position_max: 200 <br>
position_min: -6 <br>
homing_speed: 7.0 # Leadscrews are slower than 2.4, 10 is a recommended max. <br>
second_homing_speed: 3 <br>
homing_retract_dist: 3 <br>
 <br>
[tmc2209 stepper_z] <br>
uart_pin: PC6 <br>
interpolate: False <br>
run_current: 0.6 <br>
sense_resistor: 0.110 <br>
stealthchop_threshold: 0 <br>
 <br>
##Z1 Stepper - Rear Center <br>
[stepper_z1] <br>
step_pin: PG4 <br>
dir_pin: PC1 <br>
enable_pin: !PA0 <br>
#Rotation Distance for TR8x8 = 8, TR8x4 = 4, TR8x2 = 2 <br>
rotation_distance: 4 <br>
microsteps: 32 <br>
 <br>
[tmc2209 stepper_z1] <br>
uart_pin: PC7 <br>
interpolate: False <br>
run_current: 0.6 <br>
sense_resistor: 0.110 <br>
stealthchop_threshold: 0 <br>
 <br>
##Z2 Stepper - Front Right <br>
[stepper_z2] <br>
step_pin: PF9 <br>
dir_pin: PF10 <br>
enable_pin: !PG2 <br>
#Rotation Distance for TR8x8 = 8, TR8x4 = 4, TR8x2 = 2 <br>
rotation_distance: 4  <br>
microsteps: 32 <br>
 <br>
[tmc2209 stepper_z2] <br>
uart_pin: PF2 <br>
interpolate: False <br>
run_current: 0.6 <br>
sense_resistor: 0.110 <br>
stealthchop_threshold: 0
