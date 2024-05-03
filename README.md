# DSiInfo
info I've learned about the DSi hardware, you can use this as a reference if you wish

I'm releasing this info into the public domain, but credit is appreciated if you make use of it

Top Screen
i numbered the color bits from most to least significant (eg. bit 1 is most significant, bit 6 is least significant)

```
pin 1 ~15 volts, controls brightness. 13.4V level 1, 13.8v level 2, 14.2v level 3, 14.8v level 4, 15.2v level 5
------be careful poking at this pin, accidentally shorting this with the
------adjacent one will turn off ur DS and could cause damage
  pin 2 VDD 480mV
pin 3 higher freq clock
  pin 4 ~354kHz matches pin 10
pin 5 higher freq clock
  pin 6 ~354kHz matches pin 10
pin 7 higher freq clock
  pin 8 ~354kHz matches pin 10
pin 9 higher freq clock
  pin 10 ~354kHz 45 cycles per cycle on pin 47
pin 11 VDD -5v
  pin 12 10.2V
pin 13 VDD 5v?
  pin 14 GND
pin 15 VDD 3.3v?
  pin 16 VDD 3.2v
pin 17 VDD 3.3v?
  pin 18 VDD 3.2v
pin 19 horizontal+vertical blank? more testing needed
  pin 20 blue bit 6  (least significant)
pin 21 blue bit 5
  pin 22 blue bit 4
pin 23 blue bit 3
  pin 24 blue bit 2
pin 25 blue bit 1    (most significant)
  pin 26 green bit 6 (least significant)
pin 27 green bit 5
  pin 28 green bit 4
pin 29 ground
  pin 30 green bit 3
pin 31 greed bit 2
  pin 32 green bit 1 (most significant)
pin 33 red bit 6     (least significant)
  pin 34 red bit 5
pin 35 red bit 4
  pin 36 red bit 3
pin 37 red bit 2
  pin 38 red bit 1  (most significant)
pin 39 ground
  pin 40 1,752,230Hz
pin 41 clock with tiny duty cycle, probably indicates each frame
  pin 42 280ns pulse every 63.52us 15,734.3Hz, pulses on every rising and falling edge of pin 47
pin 43 ground
  pin 44 5v clock clock matches pin 47
pin 45 3.3v clock matches pin 47
  pin 46 GND
pin 47 5v clock ~7867hz
```


