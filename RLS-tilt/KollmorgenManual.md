#  Kollmorgen motor

## ASCII commands

Extensive doc for ASCII commands can be found here :
[http://www.wiki-kollmorgen.eu/](http://www.wiki-kollmorgen.eu/wiki/DanMoBilder/file/s300700help/ASCII.HTML])

A subset of the most useful commands :

    EN		enable drive
    DIS		disable
    CLRFAULT	clear faults
    ANCNFG=8	analog setpoint with OPMODE=5
    SRND		start of range
    ERND		endof range
    SETREF		set current position as reference point
    PRD		absolute position within 1 turn
    PFB		current position (control loop feedback)
    SAVE		save config
    COLDSTART	reboot
    ERRCODE		displays error

## reduction factor

The Kollmorgen motor is a step motor. It is attached to a reductor.

- 10000 step = 1 round
- reduction factor : 1/60 round
- J gives round per minute (rpm)
- ex : J100 = 100 rpm

The total gain depends of the Crankshaft (Système bielle-manivelle, Biela-manivela, Kurbelwelle). One position of the motor axis allows a gain of 1, the other one transform the rotation into a sinusoïd.

In total, J60 gives 1 rpm for the lightsheet, J360 gives 1 Hz.