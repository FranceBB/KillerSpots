# KillerSpots
Spot removal function for Avisynth based on Didée's idea from 2010 that makes use of MVTools analysis and RemoveDirt to detect and clean up spots with adiacent pixels.
<br>
All credits to Didée, GMJCZP and John Meyer.

**Requirements:**
<br>
AviSynth+ or AviSynth 2.6
<br>
Supported color formats: Y8, YV12, YV16, YV24
<br>
AviSynth+: All planar Y and YUV formats (8/10/12/14/16-bit) are supported, but NOT 32bit float.

**External filters:**
<br>
- MVTools2
- RGTools
- RemoveDirt

**Syntax and Parameters:**
<br>
KillerSpots(clip, int "limit", bool "advanced", bool "comp")

*bool advanced = false*
<br>
it triggers the use of the spot removal limit parameters, however it's disabled by default for legacy reason

*int limit = 10*
<br>
when advanced mode is turned on, this parameter limits the threshold based on which spots are detected and removed

*bool comp = false*
<br>
this parameters allows a comparison between the cleaned clip and the source without the user having to use StackHorizontal etc.


![Screenshot from 2021-10-23 10-04-34](https://user-images.githubusercontent.com/18946343/138550289-b24be84d-0a5c-445e-87d2-304b5b6c45c4.png)
![Screenshot from 2021-10-23 10-04-47](https://user-images.githubusercontent.com/18946343/138550290-9679bee4-372e-450b-8732-26379513e284.png)
