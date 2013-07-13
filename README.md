modified avalon firmware
========================

avalon firmware with modified cgminer

- option for inverted pwm fans
- options to set some previously hardcoded constants 
- a little changes in UI, added calculation of hw errors %

new options description

- --avalon-invert-pwm

changes behavior of pwm regulation to decrement pwm value instead of increment and vice-versa.
- --avalon-fanfactor

fan sense multiplier constant, if you fan is higher rpm than 3600 you need to change this value
- --avalon-hysteresis

hysteresis levels constant, the lower, the faster fan speed regulation would be, not recommended to set more than 4
- --avalon-timeoutfactor

constant divided by frequency to get timeout value in auto mode
