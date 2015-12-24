elm-comidi
===========

This is a parser for MIDI files written in pure elm and using the [elm-combine](https://github.com/Bogdanp/elm-combine) parser combinator library.

It is a component of an intended eventual assemblage of modules that will allow me to replace [MIDI.js](https://github.com/mudcube/MIDI.js/) in my [tradtunestore](https://github.com/newlandsvalley/tradtunestore) web application. This is used to play MIDI files that have been automatically generated from tunes in [abc notation](http://www.lesession.co.uk/abc/abc_notation.htm) and that have been submitted by users. Other modules will include a soundfont loader and a web-audio player.  

Tradtunestore uses only Type-0 (single track) MIDI files which are supported in the parser. The intention is to eventually to provide a fully conformant parser which is also happy with Type-1 and Type-2.

Limitations
-----------

Type-0 files are handled successfully.  Some Type-1 files are parsed and others are not for reasons that are not entirely clear at the moment.  Type-2 has not been tested.

In order to improve Type-1 handling, support fpr Running Status messages has been lost.
 




