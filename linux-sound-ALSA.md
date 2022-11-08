# Comenzi ALSA

## Cum sa restartezi ALSA:

   $ sudo alsa force-reload 
   
   ref [1]
   
# Playing with soundcards

Playing with sound cards is more complicated that playing with disks.

With disks everything works just form the start and this is due to the fact that they are essential components of every computer.
Besides this aspect of "fast working" from the physical point of view they work very simplisitcally
from the logical point of view: under linux a special file is provided to the user to work with the
disk. If the user writes to this file, it writes the disk. If the user reads from this file, it reads
the disk. There are not other things that you can do with a disk. Any other operation the user knows
about disks (like partitionaing and formatting) takes place by using the special device file provided
by the linux kernel to manipulate the disk and it consists from a sequence of reading and writing data
from and to the disk.

With sound cards the things are much more complicated. Here are some diferences:

- A sound card can receive a digital signal and can output an analogical signal;
- The sound can go to a speaker or to headephones;
- The sound can be captured from a microhpone or from a digital instrument;
- Digital sound is not a simple array of bytes. A digtal signal has a organisation: a sample rate, the
  number of chanels. etc.
- The output can be in frequency modulation;
- Soundcards can provide mixers being capable of mixing more source of data.
- Soundcards have volume, balance and bass controls;

Due to all these features, the access to soundcards through a single special file is not
enough. As you can see in [3, sec 7.2] more special files canb be provided for a single
soundcard: (as of 1995) "Each of these features have their own device driver interface. For digital
samples it is /dev/dsp, for the frequency modulation it is /dev/sequencer and for the
midi interface it is /dev/midi. The sound settings (like volume, balance or bass) can
be controlled via the /dev/mixer interface. For compatibility reasons a /dev/audio
device exists which can read SUN data."

As you can see, there are many thing to know about soundcards: you must know what the device files
are. Why you need many device files for a sound card. You must know the capabilities of your sound
card (does it support MIDI? dors it support a mixer?, etc). And you must know  stuff about digital
sound.

So be prepared with patiens. There is along way you habe to walk in order to understand how sound
is processed. In 2022 there we have ALSA that takes the responsability of providing special device
files to the user.


# Playing with sounds
  
## How to play a sound?

  An old Howto [2; sec 6.2] said that it is possible to send a file to the
  soundcard with cat. While this may not be very obvious how to do it (in 2022) because you must know which is the
  device file the same howto said that sending a file to the soundcard may not provide good results. 
  
  By using a program to play a sound is better because the program sets the soundcard to the correct sampling rate.

## How to record a sound?

  An old Howto [2; sec 6.3] says that it is possible to record a sound by reading the device file coorespinding to the card.
  This may not be very obvious how to do it (in 2022) because you must know which is the device file. However,  the same howto
  says that this tecnique may not provide the best results because the sampling rate is not set 
  
  Using a dedicated program provides better results because it is possible to set the sampling rate.

# Open questions

1. How can I use a sound card to replace the system consol beep? And vice versa.

   
# References

- [1] https://wiki.ubuntu-it.org/Hardware/Audio/HdaIntel
- [2] https://tldp.org/HOWTO/Sound-HOWTO/x504.html
- [3] *Sven Goldt*, *Sven van der Meer*, *Scott Burkett*, *Matt Welsh*, The Linux Programmer's Guide, 1995, https://tldp.org/LDP/lpg/lpg.html
