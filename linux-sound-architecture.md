# Linux Sound Architecture

## Summaries

### Audio on Linux: The End of a Golden Age? [1]

[1] is an excelent explanations about the motivations of having audio servers like PulseAudio or Jack. The video
explains what ALSA is, and what other software PulseAudio, Jack and Pipepewire are.

### Fabian Renn-Giles (Independent) - The Linux Audio API: A Different Way To Do Audio [2]

[2] Information about the low level communication between ALSA and programs. There are some interesting questions at the end of the video (starting at 1:02:45)

The information presented in this video is too low level to be useful for someone who wants to configure the audio on linux.

### Audio on Linux: The End of a Golden Age? [3]

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












## References


- [1] Linux Audio Explained (ALSA vs PulseAudio vs JACK vs Pipewire Explained) , https://www.youtube.com/watch?v=HxEXMHcwtlI
- [2] Fabian Renn-Giles (Independent) - The Linux Audio API: A Different Way To Do Audio, https://www.youtube.com/watch?v=-wDVPreDNjE
- [3] Audio on Linux: The End of a Golden Age? https://www.youtube.com/watch?v=6oQF2TzCYtQ



