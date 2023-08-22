# Algorithmic-Interactive-Music-on-the-Web-Browser
Web-app for automatic generation and computer-assisted manipulation of melodic and rhythmic musical patterns, with built-in synthesisers, transport and BPM controls.

Mainly built with Angular 7, Tone.js and Chance.js.

Inspired by Laurie Spiegel's Manipulations of Musical Patterns
[L. Spiegel. (Oct. 1981). “Manipulations of Musical patterns”, ​Proceedings of the Symposium on Small Computers and the Arts,​ No. 393, pp.19 - 22]

DESIGNED TO FOSTER MUSICAL CREATIVITY AND INSPIRATION

For (much) further detail, please read 'Final Project Report.pdf' and watch some demo videos inside the folder 'Video recordings'.

The code is in 'Angular App.zip'.

## Introduction
Algorithmic Interactive Music is not yet very common, and the Web Browser is the media which can best help it in becoming mainstream. The project consists in a Web Music Application dedicated to the generation and manipulation of Musical structures in real time, to be used in the context of an Improvisation or Live Performance. The Application is meant to foster the Musical creativity of the user by allowing low and abstracted level of control over creation and manipulation of Musical patterns. The Generative Algorithms produce plausible and engaging melodies; nevertheless, the focus of the Application is on how the user can actively and creatively manipulate them.

## Events
An event can be either a note or a rest, depending on the notes likelihood percentage (higher the notes likelihood percentage, higher the probability of the event being a note and not a rest).

## Patterns
Musical patterns are sequences of events, that is, groups of subsequent notes and/or rests.

## Phrases
Phrases are sequences of patterns.

## GUI and controls over musical manipulations
Each synth has its own GUI, but all of them (all the synthesiser types) have the following controls.

<img src="Screenshots/Main GUI.png"/>

### Global data 
They apply to everything played by the relative synth.
Numbers for pitches ranges represent pitch classes in terms of the relative distance to the selected tonic (Anglosaxon notation, A = 440 hZ), that is, 0 is the tonic, 4 is the fourth, 8 is its octave, ecc.
Rhythmic vertical and horizontal ranges represents a matrix of symbolic figures durations, where each row is half the duration of the row above, and viceversa, and each column contains the rhythmic durations of the column at its left multiplied by 3, 5 and 7 (the multiplied durations are, in the case of columns, the ones in the first column from the left).

<img src="Screenshots/Rhythmic horizontal and vertical subdivisions.png"/>

Phrases arrangement represents the series of phrases to be played by the synth, where each phrase is represented by a number. For each time we want a phrase to be played, its number (aka its name) must be specified in this field.

### Phrases

<img src="Screenshots/Phrase controls view.png"/>

### Patterns

<img src="Screenshots/Pattern controls view.png"/>

#### Cloning
Phrases and patterns can be copied.