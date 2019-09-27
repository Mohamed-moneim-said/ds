<h1>Dark star</h1>

<h2>infromnation about dark star project</h2>

<p>.This is a project to create a new operating system in assembly language 6085
To run on a darkstar machine.</p>
<h2>how to write file in project</h2>	
<p>. It should be taken into account when writing a new file written in the first file after write "processor 6085" write include" fr / system.fr". if you want to create a file related to my font write include"darkstar/font.fr".</p>
<pr>This is large - 111k. It includes a loader, the DeskTop app (with both main memory and aux memory segments, filling everything from $4000 to $FFFF (except for I/O space ), and still having more code segments swapped in dynamically.

The file is broken down into multiple segments:

segment 0: load - A$2000-$257F, L$0580, mark $000000 (Loader)
segment 1: aux - A$4000-$BFFF, L$8000, mark $000580 (MGTK, DeskTop)
segment 2: auxlc - A$D000-$ECFF, L$1D00, mark $008580 (DeskTop)
segment 3: auxlc - A$FB00-$FFFF, L$0500, mark $00A280 (DeskTop)
segment 4: main - A$4000-$BEFF, L$7F00, mark $00A780 (DeskTop)
segment 5: main - A$0800-$0FFF, L$0800, mark $012680 (Initializer)
segment 6: main - A$0290-$03EF, L$0160, mark $012E80 (Invoker)
segments dynamically loaded for these actions:
disk copy - A$0800, L$0200, mark $012FE0
format/erase - A$0800, L$1400, mark $0160E0
selector - A$9000, L$1000, mark $0174E0
common - A$5000, L$2000, mark $0184E0 (used by selector, copy, delete)
file copy - A$7000, L$0800, mark $01A4E0
file delete - A$7000, L$0800, mark $01ACE0
selector - A$7000, L$0800, mark $01B4E0
(EOF is $01BCE0)
</pr>
<br>
<img src="https://engblg.livingcomputers.org/wp-content/uploads/2019/01/viewpoint-final-ui-1024x886.png" alt="XEROX VIEW POINT">
<p>This is an illustrative image of a form that should be an operating system on it if you are in addition to a form written in comments</p>
<h2>files in progress</h2>

<h3>font.fr:5% incomplet</h3>
<h3>mose.fr:99% incomplet</h3>
<h3>system.fr:85% incomplet</h3>
<h3>system.s:10% incomplet</h3>
<h3>10 files not started</h3>
