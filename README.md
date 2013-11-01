ArduinoMidiSequencer
====================

 A simple firmware MIDI sequencer program for an Arduino board with a 
 SparkFun MIDI Shield or equivalent

 This is an Arduino "sketch" (project), intended to be compiled using the 
 free Arduino development software.  It is intended to be run on standard
 sized Arduino boards such as the Arduino Uno, with a daughter board.

 This sketch provides a fully functional MIDI sequencer, and is designed to 
 work with the SparkFun MIDI Shield.  The shield has MIDI In, MIDI Out,
 three buttons and two potentiometers (knobs you can turn).
 
 If you hold the shield with the MIDI connectors at the bottom, the buttons,
 from left to right are Play, Stop and Record.  The knobs, again from left
 to right are Tempo and Velocity.
 
 The sketch comes up with the sequence from Pink Floyd's song On The Run
 (from the Dark Side of the Moon CD), which is legal "fair use" because I 
 am providing it for educational purposes only.  It's only 8 notes, which
 are listed on the Wikipedia page for the song, so I'm not revealing any
 secret musical arrangement.
 
 The sequencer plays a sequence of MIDI notes when you connect the MIDI 
 Out of the shield to the MIDI In of a synthesizer and press the Play 
 button.  All the notes have an equal duration.  The green LED on the
 shield will light while it is playing.
 
 You can input a different series of MIDI notes to the sequencer to play 
 by connecting the MIDI Out of a keyboard (or other MIDI instrument) to
 the MIDI In of the shield.  Note: There is a switch on the MIDI Shield, 
 and for inputting notes, it must be in the Run position; for writing a 
 sketch to the Arduino, it must be in the Prog position.
 
 To change the sequence, make sure the playback is stopped, press the 
 Record button, and the red LED will light.  Then play the notes you 
 want in the order you want them played.  When inputting, you do not need 
 to play fast or even, just in the right order.  If you make a mistake press 
 the Stop button and start over.  If you complete playing the sequence in 
 the correct order, press the Record button again.  it will immediately 
 begin playing your new sequence.

 
 The circuit for the MIDI shield can be found here:
 https://www.sparkfun.com/datasheets/DevTools/Arduino/MIDI_Shield-v13.pdf

 The sketch uses a timer library created by Simon Monk and Jack Christensen.
 You can find it here:
 https://github.com/JChristensen/Timer
 
 There is an out-of date page about it on the Arduino website here:
 http://playground.arduino.cc/Code/Timer
 
 Follow the instructions at the github site about unzipping the library in your
 Arduino library folder, and if necessary, from inside this project, select the 
 menu Sketch->Import Library and import the timer library.
