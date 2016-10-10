# Learning journal example

### 29/9/2015

Tripped up by language. Variable called 'introduced' meaning "I introduced myself" but latter used as "object was introduced this frame." In the first sense the variable starts false and then turns true. In the second it starts true and then turns false. Good blog post material. (Use as an example of a work journal / learning journal entry.)

### 4/10/2016

It's important to keep a backup of lecture notes and example files in case you get locked out of Moodle!

### 7/10/2016

Tracked down a bug in our GPS prediction code. It seems the prediction was quantising the locations to values approximately 32 cm apart in the latitude only. The problem turned out to be due to the limited precision of floating point numbers combined with an unexpected handling of typecasting.

### 10/10/2016

I thought we had an issue with the ground speed as reported by our GPS unit being almost twice as big as it should be. But it actually turned out to be that the time step in my data was actually 50Hz rather than the 20 Hz I had assumed.
