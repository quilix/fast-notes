# Comenzi ALSA

## Cum sa restartezi ALSA:

   $ sudo alsa force-reload 
   
   ref [1]
  
# Playing with sounds
  
## How to play a sound?

  An old Howto (6.2 in https://tldp.org/HOWTO/Sound-HOWTO/x504.html) said that it is possible to send a file to the
  soundcard with cat. While this may not be very obvious how to do it (in 2022) because you must know which is the
  device file the same howto said that sending a file to the soundcard may not provide good results. 
  
  By using a program to play a sound is better because the program sets the soundcard to the correct sample rate.
  
  


   
# References

[1] https://wiki.ubuntu-it.org/Hardware/Audio/HdaIntel

