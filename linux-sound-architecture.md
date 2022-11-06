# Linux Sound Architecture

## Summaries

### Audio on Linux: The End of a Golden Age? [1]

[1] is an excelent explanations about the motivations of having audio servers like PulseAudio or Jack. The video
explains what ALSA is, and what other software PulseAudio, Jack and Pipepewire are.

### Fabian Renn-Giles (Independent) - The Linux Audio API: A Different Way To Do Audio [2]

[2] Information about the low level communication between ALSA and programs. There are some interesting questions at the end of the video (starting at 1:02:45)

The information presented in this video is too low level to be useful for someone who wants to configure the audio on linux.

###  USB Audio Part 1: What is USB Audio? [3]

Explains what USB Audio is.

### Audio on Linux: The End of a Golden Age? [4]

3:48 Starts with the history of sound

4:22 Explains what you can find in the first computers as sound devices.

6:18 Mentions Soundblaster in 1989

  Explains that the possiblities of the first soundcards were different than
  the posisiblities of the current soundcards.

  - First cards: it was possible to program them to generate some kind of sound effect.
  - Current soundcards: the current soundcards are able to play a wav stream of data.

In the near future sound boards evoluted becaus the people wanted to play music and to
heare more sound at at time (so it was necessary to add mixers)

8:22 Part allocated to OSS (Open Sound system) (approx. year 2000)

The major drawback of OSS was 1 card per system but there were others.

10:16 ALSA

  - begins with the history of ALSA

19:37 Reducing costs

   - The sound hardware was simplified (no mixers, no sinthesizers). These
     features are emulated in software.

20:30 Talks about the standardization of Audio Interfaces like AC97 and
the addition of USB to ALSA

25:39 The concept of sound servers (The sound servers war; before 2004)

   - artsd: KDE
   - ESD

   Mentions *interesting* aspects about sound servers and about the data
   stream supported by a sound card.

27:00 PulseAudio

30:17 Embedded (Alsa for System on a Chip - ASoC)

33:33 Modern Hardware

   High Definition Audio (HDA)

   - Introduced in 2004, it is the successor of AC97;

   Mobiles
   
36:37 Present (2017)
  
  - EXCELENT: Starts with an image about the Linux Audio Stack
  - A slide mentions that all new hardware has on board HDA !
  - PulseAudio is HDA or USB aware
  - PulseAudio and Jack are able to comunicate with each other and to negotiate the access to the hardware.
  - Manetions changes in the embedded world
    
41:14 Future
 
  - Because the hardware got cheaper to produce, the hardware is not implementing synthesizers, mixers, etc.
  - There are new technologies to handle these changes (this type of harware): 
    - Usecase Manager (UCM): Because of the multitude of features available, these
      features cannot be described in the hardware and next used by sound server.
      The technology allows tto describe these features in profies to be used by
      a sound server ! INTERSTING  !
      
      Usecase Manager is part of ALSA and Pulseaudio has its own Usecase Manager and other
      soundservers have their own Usecase Manager.
      
    - Topology (@ 44:00)

45:25 Time for a major Overhaul?



      
      
      

     
## References


- [1] Linux Audio Explained (ALSA vs PulseAudio vs JACK vs Pipewire Explained) , https://www.youtube.com/watch?v=HxEXMHcwtlI
- [2] Fabian Renn-Giles (Independent) - The Linux Audio API: A Different Way To Do Audio, https://www.youtube.com/watch?v=-wDVPreDNjE
- [3] USB Audio Part 1: What is USB Audio?, https://www.youtube.com/watch?v=PZ9vEisSgw0
- [4] Audio on Linux: The End of a Golden Age? https://www.youtube.com/watch?v=6oQF2TzCYtQ



