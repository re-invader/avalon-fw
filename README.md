modified avalon firmware
========================

avalon firmware with modified cgminer

- option for inverted pwm fans
- options to set some previously hardcoded constants 
- a little changes in UI, added calculation of hw errors %

new options description

- [b]--avalon-invert-pwm[/b]
changes behavior of pwm regulation to decrement pwm value instead of increment and vice-versa.
- [b]--avalon-fanfactor[/b]
fan sense multiplier constant, if you fan is higher rpm than 3600 you need to change this value
- [b]--avalon-hysteresis[/b]
hysteresis levels constant, the lower, the faster fan speed regulation would be, not recommended to set more than 4
- [b]--avalon-timeoutfactor[/b]
constant divided by frequency to get timeout value in auto mode
