# Learning journal example

### 29/9/2015

Tripped up by language. Variable called 'introduced' meaning "I introduced myself" but latter used as "object was introduced this frame." In the first sense the variable starts false and then turns true. In the second it starts true and then turns false. Good blog post material. (Use as an example of a work journal / learning journal entry.)

### 4/10/2016

It's important to keep a backup of lecture notes and example files in case you get locked out of Moodle!

### 7/10/2016

Tracked down a bug in our GPS prediction code. It seems the prediction was quantising the locations to values approximately 32 cm apart in the latitude only. The problem turned out to be due to the limited precision of floating point numbers combined with an unexpected handling of typecasting.

### 10/10/2016

I thought we had an issue with the ground speed as reported by our GPS unit being almost twice as big as it should be. But it actually turned out to be that the time step in my data was actually 50Hz rather than the 20 Hz I had assumed.

### 12/10/2016

I had a 2D FIFO buffer storing X and Y coordinates. The function treated the X and Y entries as a pair, but I was calling it twice, once for X and once for Y, so the entries got added twice. This halved the size of my FIFO and caused an error in my prediction.

### 17/10/2016

I had a condition to check if the drone was in position hold mode and a separate condition to set and reset the position hold location. This meant that it was position to not have the hold position set (actually it retained the previous value) while the position hold mode remained active.
