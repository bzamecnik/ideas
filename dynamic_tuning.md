# Dynamic tuning

The goal: allow polyphonic instruments with controllable amount of dissonance. Ie. more crips consonant chords or more out-of-tune chords.

This could be done by dynamically varying both the fundamental frequencies of tones and the relative frequencies of their partials.

## The problem

The harmonic profile (set of partials) of an instrument determines the tunings at which the instrument can produce reasonable (quite consonant) polyphonic sounds.

Tones produced by most natural instruments have a static harmonic profile. Thus the set of matching tunings is limited. 

In some instruments the fundamental frequency can be varied arbitrarily (eg. voice), while in others they are more rigid (eg. piano), it is not practical to change the fundamentals while playing. Thus the set of good sounding tones is even more limited.

As an example a tone with harmonic partials (integer multiples of the fundamental) induces the just intonation tuning over some root tone. In case of an instrument with fixed strings this results in a single diatonic key which sounds best. In order to play in multiple keys a compromise tuning, the equal temperament, is used. It introduces a small error uniformly in all keys.

If we compare it to singing it also has harmonic tones but the fundamental frequencies can be varied. Still, the relative frequencies of the partials are fixed. This enables less dissonant chords. Listen to some "barbershop music".

## Solution

We can control two separate parameters:

- fundamental frequencies of each tone
    - which affect all the partials
- the relative frequencies of each partial within each tone

By modifying these parameters we change some overall metric of dissonance. We can optimize the parameters towards some value of the dissonance metric (either to minimize it, maximize it or keep it at some constant).

This could be performed either for completely synthesised sounds or by modifying existing sounds produced by normal instruments.

In all cases dissonance can be measured from the output synthesized or modified sound. For pure synthesis it could be also measured directly from the mutual configuration of all partials.

It is desirable the overall tuning does not diverge and rather stays around some constant reference frequency.

### Implementation

The simplest case is off-line synthesis of sound. It assumes that we can control the harmonic profile of synthesized tones.

- input: symbolic description of polyphonic melody and the instrument
- process:
    - for each time frame determine the optimal set of partials for each tone
    - this can be done in a single step before synthesis
- output: synthesized sound

In another case we can just control the fundamental frequencies in the synthesied sound. Thus for optimization we need a feedback loop. It can either run off-line (synthesize a single frame multiple times to get a good result), or in real-time (synthesize continuously, produce results and analyze jsut the results).

- input: symbolic description of polyphonic melody
- process
    - loop until a the result is good enough:
        - synthesize a time frame using a current set of fundamentals
        - analyze the produced sound
        - compute better set of fundamentals
    - output the synthesized frame

Much more interesting result could be obtained by modifying sound produced by existing real instruments. This could be at least done off-line. The process is similar to the first case, however, there is a difference. We need to analyze the input sound, convert it to come symbolic representation, modify it and resynthesize it.

The "holy grail" would be modifying existing sounds in real-time.

### Notes

Since a set of chords is used over and over during a song the results of optimization for given inputs could be remembered and used to initialize the optimization algorithm on further occurences of the inputs.

## Expressive tools

Since we could optimize the tones for more or less dissonance this optimization goal could be varied in time and used as an expressive tool for musicians.

Eg. the same input chord played on some set of instruments could be made either very consonant or very dissonant.

Thus the dynamic range of musical expressions could be enlarged. One could either make a stable chord more stable by decreasing dissonance, or less stable by increasing dissonance. In the first case the effect of both expressions would be aligned, in the latter conflicting.
