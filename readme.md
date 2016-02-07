# speaker_pcm

## Convert audio to the right format

We need 8000 Hz data rate and unsigned 8bit, this should do it:

* With xxd:

    xxd --include sound.wav

Sources:

    http://linux.die.net/man/1/xxd
    http://smackerelofopinion.blogspot.fr/2015/12/incorporating-and-accesses-binary-data.html

* With sox

    sox -V exterminate.wav -r 8000 -u sound.wav

Sources:

    http://playground.arduino.cc/Code/PCMAudio
    https://github.com/olleolleolle/wav2c

## Generate header file from audio file

    ./wav2c sound.wav ../sound.h sound
