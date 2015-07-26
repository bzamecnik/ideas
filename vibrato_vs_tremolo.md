# Vibrato vs. tremolo

In the music terminology these two terms are use ambiguously. However, the typical distinction is as follows:

- vibrato - modulation of the tone's fundamental frequency
- tremolo - modulation of tones amplitude

## Hypothesis

On the first sight the two phenomena are completely different. Nevertheless, they might be connected quite well, which would explain the chaos in terminology.

Consider a common situation when music is performed in a place with some reverb. If we play a FM modulated (vibrato) tone the reverb echoes the sound with some delay back and multiple copies of the original sound can be heard at the same time. Since the fundamental frequency varies this might cause interferences (dissonances) resulting in varying amplitude (tremolo).

## Experiment

- add delay or reverb to a vibrato tone
  - delay - convolution with a kernel consisting of some delta spikes
  - reverb - convolution with a continuous kernel
- analyze the interferences - changes in the volume

Is it possible to construct such conditions where the resulting sound is very close to tremolo sound (amplitude-modulated with a sinusoid)?
