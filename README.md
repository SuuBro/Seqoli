<div align="center">
  <img align="center" src="https://raw.githubusercontent.com/SuuBro/Seqoli/master/site/static/images/logo.png" alt="Seqoli">
  <br>
  <strong>A tactile, open-source MIDI sequencer for ROLI lightpad blocks</strong>
</div>

<div align="center">
  <sub>Written by 
  <a href="https://www.linkedin.com/in/jsubramaniam/">Joshua Subramaniam</a> and
  <a href="https://github.com/SuuBro/Seqoli/graphs/contributors">
    contributors
  </a>
</div>

## Table of Contents
- [Summary](#summary)
- [Installation](#installation)
- [User Guide](#user-guide)

## Summary
Seqoli is a 'DAW-less' midi sequencer interface designed to run on one or more ROLI Lightpad BLOCKS. Drawing inspiration from Monome grid, Seqoli is great for creating polyrhythms on the fly or sequencing an entire track. Snap together multiple Lightpad BLOCKS to extend your sequencer length and/or track count.


## Installation

1.  Ensure you have installed ROLI Dashboard from https://roli.com/.
1.  Download the Seqoli.littlefoot file from [here](https://gumroad.com/l/seqoli) or GitHub.
1.  Open the ROLI Dashboard and connect your lightpad block(s).
1.  Go to File -> Open... and select the downloaded Seqoli.littlefoot file.
1.  Confirm if you prefer to one-time-load the app or install it into the dashboard list.
1.  Upload to your ROLI Lightpad block(s).


## User Guide

### Interface

Seqoli has up to 5 tracks on each BLOCK, with up to 5 positions each, as shown below:

<img width="350px" src="https://raw.githubusercontent.com/SuuBro/Seqoli/master/site/static/images/Layout.png" alt="Seqoli">

Multiple blocks can be combined to increase either or both the track length and the number of tracks.


Each track has it's own current position. This will advance one place to the right with each beat, according to the BPM. 

To send MIDI notes to your instrument, you can press each position within a track to enable it. Pressing an enabled note will disable it again.

<img width="350px" src="https://raw.githubusercontent.com/SuuBro/Seqoli/master/site/static/images/Track.png" alt="Seqoli">

When the current position encounters an enabled-note, a MIDI meesage is emmitted to play the note.

<img width="350px" src="https://raw.githubusercontent.com/SuuBro/Seqoli/master/site/static/images/PlayedNote.png" alt="Seqoli">

When the position reaches the track-end marker it will loop back to the beginning. The track-end marker can be moved by pressing and sliding it. Alternatively you can press-and-hold it, and use another finger to press somewhere else on the same track.


The midi channels and note values for each track can be configured in the ROLI Dashboard. Note that the left-most block for a given track is responsible for defining the midi channel and note for the entire track, regardless of how many BLOCKS are in the row.

<img width="350px" src="https://raw.githubusercontent.com/SuuBro/Seqoli/master/site/static/images/Dashboard.png" alt="Seqoli">

The BPM is always controlled by the top-most, left-most BLOCK. 

There is currently a limit of a 5x5 BLOCKS- though it hasn't been tested with more than a 3x2 configuration.







