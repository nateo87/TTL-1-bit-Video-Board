# TTL-1-bit-Video-Board
Here is a TTL-based, 1-bit video board as designed by David L. Heiserman in the book How to Design and Build Your Own Custom TV Games. Corrections have been made from the schematics in the book, mostly just pin number confusions (the later schematics have much more troublesome errors).

The original design has the outputs all going to a card edge connector, but I thought a 40-pin IDC connector would be a little more friendly, and an adapter can easily be purchased so that an IDC cable can plug into a breadboard for experimentation. Another thing that has been changed from the original design is the analog video output. Though it is still B&W composite, the values of the resistors dividing the voltage have changed, in order to massage the signal to be more easily accepted among a wider range of RF modulators and monitors. Some TVs/monitors tend to be a little pickier about the signal being put into them. In my experimentation, most CRT TVs with a direct composite input tend to be more forgiving with the signal. Jumpers can be placed to activate an amplification of the video signal for more selective monitors.

The text of Heiserman's book can easily be found online on archive.org, and I highly encourage trying some of the builds in the book, if only so that I'm not the only one crazy enough to be working through them! I haven't ordered boards yet from this most recent revision (V3), but once I do, I'll have pics of the assembled product running some experiments. 

Here's a video of an earlier revision of the board running a simple moveable square circuit:
[![2022-11-23](https://user-images.githubusercontent.com/79879072/203691313-1f590cd3-0e1b-4087-b946-11cf27650e67.png)](https://www.youtube.com/watch?v=p2fEVsLSzvE&t=35s)
