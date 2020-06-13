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

Seqoli has up to 5 tracks on each block, with up to 5 positions each, as shown below:

<img align="center" width="350px" src="https://raw.githubusercontent.com/SuuBro/Seqoli/master/site/static/images/Layout.png" alt="Seqoli">


Each track has it's own current position. This will advance one place to the right with each beat, according to the BPM. 

To send MIDI notes to your instrument, you can press each position within a track to enable it. 

<img align="center" width="350px" src="https://raw.githubusercontent.com/SuuBro/Seqoli/master/site/static/images/Track.png" alt="Seqoli">

When the current position encounters an enabled-note, a MIDI meesage is emmitted to play the note.

<img align="center" width="350px" src="https://raw.githubusercontent.com/SuuBro/Seqoli/master/site/static/images/PlayedNote.png" alt="Seqoli">

When the position reaches the track-end marker it will loop back to the beginning. The track-end marker can be moved by pressing and sliding it. Alternatively you can press-and-hold it, and use another finger to press somewhere else on the same track.





