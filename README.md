concatenate wav files and put a cue point at each boundary.

targeted for use with the dirtywave M8. note that M8 only supports up to 32 slice markers in a file.

`cuecat.js input1.wav input2.wav ... inputN.wav output.wav` to stitch the input wavs together (in order), and set
a cue point at the end of each one

expects mono or stereo WAV input, output is 16 bit 44.1khz stereo WAV, or mono if all inputs are mono.

You can also list the cue points in a wav: `cuecat.js file.wav`

`batch.sh` is an example for how I'd run this on a bunch of dirs full of wav files
