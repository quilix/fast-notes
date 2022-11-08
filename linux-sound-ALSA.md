# Comenzi ALSA

## Cum sa restartezi ALSA:

   $ sudo alsa force-reload 
   
   ref [1]
  
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
- [3] https://tldp.org/LDP/lpg/lpg.html
