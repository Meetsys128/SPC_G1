# SPC_G1
A library for playing music with one passive buzzer, loading the songs and sounds from FLASH. Requires Ticker and Eeprom_rotate to be installed. It is strongly advised to modify the "data.txt" file, then use the FileToFlash function.
The structure of data.txt:
//one song (songs separated by ; alone on a line)

mpr:
(millis per row)
(space)
pidxs:
0
2
0
1
5
4
5
3
//...
(space)
patterns:
(
<NOTE>(space)<OCTAVE>(space)<LENGHT>(space)<EFFECT>
C 4 3 0
note c, octave 4, played for 3 * the mpr(ms per row), no effect)
...
, // empty line with only ,
...
;
...

