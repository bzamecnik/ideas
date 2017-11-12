# Coloring of the chromatic circle relative to a key

The goal is assign colors to all pitch classes given a particular key. The color should tell how much the tone is "inside" or "outside" the key or if it's on the boundary of the base key and its mirror key.

Solution:

We can take a circle of fifths starting at the key's base pitch class.

    C, G, D, A, E, B, Gb, Db, Ab, Eb, Bb, F

Then we reverse the second part.

    C, G, D, A, E, B, F, Bb, Eb, Ab, Db, Gb

Finally, we colorize the tones smoothly from green though yellow to red.

![](key_coloring.png)

Python code: https://gist.github.com/bzamecnik/641edbe0585547e13dd4a333eb698bb8
