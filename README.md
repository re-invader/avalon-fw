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

fan sense multiplier constant, if you fans has higher rpm than standart fans you need to change this value
to return correct rpm value divide your fan max rpm by 32 ( 3840 / 32 = 120 ) 
- --avalon-hysteresis

hysteresis levels constant, the lower, the faster fan speed regulation would be.
can produce oscillations if value changed and min/max fan limit difference is high 
not recommended to set more than 4

- --avalon-timeoutfactor

constant divided by frequency to get timeout value in auto mode
