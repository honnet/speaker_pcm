# speaker_pcm

## Sources

    http://playground.arduino.cc/Code/PCMAudio
    https://github.com/olleolleolle/wav2c

## Need 8000 Hz data rate (-r) and unsigned 8bit (-u)

    sox -V exterminate.wav -r 8000 -u sound.wav

## Generate header file from sound file

    ./wav2c sound.wav ../sound.h sound

