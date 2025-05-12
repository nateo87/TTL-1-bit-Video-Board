# TTL-1-bit-Video-Board
<s><i><b>UPDATE 2/2/2025:</b></i>

![new board render from KiCad](https://github.com/nateo87/TTL-1-bit-Video-Board/blob/main/gallery/full%20video%20boardREV3.jpg)

Did another revision of the board. The one I had up here previously was one of my first projects in KiCad, moving away from EasyEDA. The main changes with this revision have to do with size: the board is MUCH smaller, and the footprints for a lot of the passive components have been assigned more appropriately sized designs. I also swapped out the no-longer-produced 74LS76 IC with the much easier to source 74LS109. Still functions the exact same, only difference is pinout and 'K' is now active LOW instead of HIGH. ANYWAYS, on to what I wrote previously: </s>

<b>UPDATE: 5/12/2025 </b>
Just built one of the newest revision, and whaddya know, a 74LS109 <i>will not</i> work in place of a 74LS76! I built a board over the weekend, and thought maybe I was dealing with pad PCB design that was creating ringing or cross-talk between signals. But nope - it has to use a <i>negative edge</i> triggered JK flip-flop instead of a positive edge trigger. I bodged in a 74LS112 and all was well. I'm currently working on a revision to use the 74LS112 instead. 

<i>end of update</i>

Here is a TTL-based, 1-bit video board as designed by David L. Heiserman in the book How to Design and Build Your Own Custom TV Games. Corrections have been made from the schematics in the book, mostly just pin number confusions (the later schematics have much more troublesome errors).

The original design has the outputs all going to a card edge connector, but I thought a 40-pin IDC connector would be a little more friendly, and an adapter can easily be purchased so that an IDC cable can plug into a breadboard for experimentation. Another thing that has been changed from the original design is the analog video output. Though it is still B&W composite, the values of the resistors dividing the voltage have changed, in order to massage the signal to be more easily accepted among a wider range of RF modulators and monitors. Some TVs/monitors tend to be a little pickier about the signal being put into them. In my experimentation, most CRT TVs with a direct composite input tend to be more forgiving with the signal. Jumpers can be placed to activate an amplification of the video signal for more selective monitors.

The text of Heiserman's book can easily be found online on [archive.org](https://archive.org/details/howtodesignbuild0000heis_n7e2), and I highly encourage trying some of the builds in the book, if only so that I'm not the only one crazy enough to be working through them! I haven't ordered boards yet from this most recent revision (V3), but once I do, I'll have pics of the assembled product running some experiments. 

Here's a video of an earlier revision of the board running a simple moveable square circuit:
[![2022-11-23](https://user-images.githubusercontent.com/79879072/203691313-1f590cd3-0e1b-4087-b946-11cf27650e67.png)](https://www.youtube.com/watch?v=p2fEVsLSzvE&t=35s)
