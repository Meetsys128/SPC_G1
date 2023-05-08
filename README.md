# SPC_G1
A library for playing music with one passive buzzer, loading the songs and sounds from FLASH. Requires Ticker and Eeprom_rotate to be installed. It is strongly advised to modify the "data.txt" file, then use the FileToFlash function.
The structure of data.txt:
//one song (songs separated by ; alone on a line)

mpr: <br/>
(millis per row)<br/>
(space)<br/>
pidxs:<br/>
0<br/>
2<br/>
0<br/>
1<br/>
5<br/>
4<br/>
5<br/>
3<br/>
//...<br/>
(space)<br/>
patterns:<br/>
(<br/>
<NOTE>(space)<OCTAVE>(space)<LENGHT>(space)<EFFECT><br/>
C 4 3 0<br/>
note c, octave 4, played for 3 * the mpr(ms per row), no effect)<br/>
...<br/>
, // empty line with only ,<br/>
...<br/>
;<br/>
...<br/>

