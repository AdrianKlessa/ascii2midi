# ascii2midi
Encodes an ASCII string to a midi audio file and back

1 byte (1 ASCII character) is 1 note in the MIDI file

First two bits are encoded as the note_on velocity (strength of the piano keypress)

Next two bits are encoded as the note_off velocity (strength with which the key was released)

Last 4 bits are encoded by the piano key that was pressed (selected from 16 keys in a given musical scale)

Includes code to generate list of keys for a major/minor scale based on a given note / tonic (provided as a MIDI note number)
