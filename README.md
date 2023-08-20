# Font Lister for FreeGEOS

This little program can help you keep track of all the fonts installed in your
FreeGEOS system by providing an easy way for creating samples of every
printable font.

Usage is really simple: after launching, the program opens a dialog where you
only have to click the "Update List" command to create a list with samples of
all the currently installed fonts. You can use the Edit menu or the mouse to
mark all or parts of the text and transfer it to other applications (typically
GeoWrite), where the samples can be printed.

For each font, the program displays its name and the internal ID number. The
font ID is important for the compatibility of documents you exchange with
other people. After that, two lines of the classic "quick brown fox" text are
used to show all the upper and lower case characters.

The third line shows a selection of special characters to help you in checking
the completeness and proper conversion of the font. The sample line contains
the following components:

 - The word "AVATAR", which is usually a good indication of whether font
   contains any kerning data (rare!) - if so, the "A" letters are drawn
   noticeably closer to the "V" and the "T" to reduce the amount of empty
   space between them.
 - The digits "123" for checking if numbers are included.
 - The punctuation symbols "+;#" (plus, semicolon, hash mark/number sign).
 - The German diacritic symbols for a-Umlaut in upper and lower case (i.e. the
   letter "a"/"A" with two dots above it), together with the German "sz"
   ligature (looks somewhat like a Greek "beta"). If these are properly
   displayed, chances are that most other accented characters are available as
   well.
 - The symbol at position DBh in the Geos character set (key combination:
   Ctrl-Shift-Alt-$). In standard Geos fonts, this is a currency symbol
   consisting of a circle with four little "ears". Burkhard Oerttel proposed
   redefining this character for displaying the new "Euro" currency symbol
   (a captial "C" with two horizontal lines through the middle). This
   convention is used for example by the Optifonts collection.

Alternatively, you can enter your own sample text in the FontList dialog
before clicking "Update List". This can be useful if you want to check
the appearance of a font with a specific passage of text (for example, a few
sentences from a famous speech...).

Another reason to use this is to reduce the complexity of the sample text
(e.g. replacing it by only "ABC") if you experience crashes with a large
number of fonts installed.
