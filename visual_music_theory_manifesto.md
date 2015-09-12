# The Manifesto of Visual Music Theory

## The goal

> Be able to understand the structure in human music well in order to percieve and perform music better.

![And I Hove Her](http://i.visualmusictheory.com/manifesto/and-i-love-her.png)

## About this document

This document tries to outline an educational process of learning music theory.

Is a result of my more than 20-years old  frustration (since 1st grade) with classical music theory and it's education and finding other exciting ways of comprehending the structure in music. After taking the exams at the [Fundamental of Music Theory](https://www.coursera.org/course/musictheory) course at Coursera on 2015-09-12 the cup has poured over.

This is a work in progress, feel free to disscuss it or post pull request.

- twitter: [@bzamecnik](https://twitter.com/bzamecnik)
- [my blog with a few basic articles already written](http://www.visualmusictheory.com/)

## TL;DR

- classical music theory is unnecessarily complex
- it is very hard to learn and think about by humans
- many people thus get dissapointed by learning music instead of enjoying it
- the structure in music is much simple without the burden of ages
- music theory it can be refactored to the bare minimum
- we can use very powerful concepts distilled from science (mathematics, physics, machine learning, signal processing, neurology, etc.)
- we can use powerful visual representations
- we can learn about human perception
- we can use the comprehensible concepts to learn music and perform it better
- by understanding the concepts classical music theory makes more sense
- we can learn it more easily as a "foreign language” to communicate with other people since it still is the lingua franca
- this is not meant to completely erase classical theory and replace it with something else, but to make more sense to the concepts in the classical theory
- also this is not something completely green-grass new, rather a synthesis of existing research from various fields into something practically useful

## Preface

Music is beautiful. It is a language humans use to can communicate emotions via sound. Along with other forms of languages it evolves spontaneously for ages  through practice. However, it is not a chaos, it has some very interesting structure to which it converges.

This structure can be unconsciously comprehended by people exposed to music. It is joy for mind to explore the structure in music as well as to feel the emotions carried by music. Even though other animals also communicate using sound, it is beyond this scope and we will focus on human music.

Many people have tried to better understand the various parts of the structure in music and created a lot of theories trying to explain them. Also in order to clearly record and communicate musical ideas people stared to describe musical pieces visually.

Since music as we know it originates in how humans treat sound, the two vital sources of structure in music are acoustics and human perception. We can describe it with various interesting more or less abstract models. But the models are worthless without actual music.

There is a broad range of aspects of music, thus a music theory needs to deal with:

- time
- frequency
- intensity
- timbre
- tuning
- sections
- ornaments
- visual representation
- etc.

## The Problems in Classical Music Theory

![Classical notation](http://i.visualmusictheory.com/manifesto/classical-notation.png)

Classical music theory carry a lot of unnecessay complexity and inconsistency beyond the inherent complexity in the music - mostly in terminology and visual representation. It stems from the long evolution, progresses in understanding and  maintaining backwards compatibility. It’s not that our ancestors were idiots. Any disruptive changes in terminology and visual representation are typically so painful that they have hard time to catch on.

- too focused on notation
- symbolic notation is good for print but bad for understanding
- insane terminology
- accidentals
- key signatures
- chord names
- scales
- scales names
- note duration names
- rhythm names
- (the list goes on...)

# Visual Music Theory

![Tone circle - clock analogy](http://i.visualmusictheory.com/tone-circle/alarm_clock_pitch_classes_d_800.jpg)

- Keep concepts simple.
- Be visual.
    - People are trained more for visual perception. It carries bigger stream of information. People can easily find patterns visually.
- Be interactive.
    - With the advent of computers we are no longer limited by pen and paper. Create beautiful visualizations, merge music with animations and go interactive.
- Be practical. Allow people fiddle themselves and use the concepts in their own music instead of just plain memorizing.
- Start with the important things, leave details for later. But do not hide them completely.
    - Try following the 80/20 rule in education. Like learn 80% useful concepts in 20% time.
- Show the big-picture path. Draw the attention to the next leture by showing the results.
    - Don’t be narrowly focused and bring useful ideas from other fields.
- Go by small well-conencted steps.
- Build the theory from small concepts - with a range of abstactions from low-level high-level.
- Take concepts from software engineering/machine learning:
    - DRY - each concept should do one thing and do it well (factorization)
    - KISS - prefer simpler concepts over more complex (regularization)
    - be bold and do refactoring if it helps
- Simultaneously translate the concepts to the classical terminology to avoid a “shock".
- Do not punish for being unconvential.
    - some thigns not always bad, they're just unexpected and bring too much attention
        - beats off the rhythm
        - tones outside the key
        - dissonant tones
        - tones out of tuning

## An appetizer

It's not just words of hate without any actions...

[![Penny Lane chords visualized](http://i.visualmusictheory.com/manifesto/penny-lane.png)](https://vid.me/is5)

- [Penny Lane chords visualized](https://vid.me/is5)
- [The beauty of music's getting visual](https://vid.me/Wat)
- [Tone circle](https://play.google.com/store/apps/details?id=com.harmoneye.tonecircle)
- [HarmonEye](http://harmoneye.com/)
- [Music Theory Toolbox](http://bzamecnik.github.io/music-theory-toolbox/)
- [Tuner](https://www.youtube.com/watch?v=8y6L9HwdeAA)

## The journey

- kinds of sound
    - 2D visualization: time-frequency place
    - intensity
    - percussive sounds
        - focused more in time
    - harmonic sounds
        - focused more in frequency
    - noisy sound
        - focused neither in time or frequency
- dissecting a song / a zoom into a song
    - time - sections, verses, bars, beats, percussions
    - frequency - keys, chords progressions, chords, tones, embelishments
    - intensity - variation in loudness, dynamics
    - timbre - the spectral shape of sounds
    - feeling/perception - stable/boring/resolved/expected, unstable/excited/tension/unexpected
        - the structure of antic drama / stories
            - set the landscape (stable) so that the listener can orient
            - rise the tension until a maximum so that it is not boring
            - resolve the tension and finish stable so that the end is expected
    - prosody - correspondence in feeling stable/unstable across various features
    - lyrics
- basic of rhythm - time
    - periodicity
    - speed
    - [hierarchical] time division
    - patterns on the grid
    - from periodic percussive sounds to harmonic sounds -> more speed
- tones - frequency
    - “height” - continuous
    - harmonic
        - voice, strings, wind instruments, etc.
    - not harmonic
        - bell, xylophone
    - discrete tones - based on harmonic tones
    - octave equivalence
    - linear model -> helix model
- 12-tone circle
    - clock analogy
    - structure: 5+2+5 = (5+2)+5 = 5+(2+5)
    - ordering
        - by 1, by 7
    - subsets, shifting (rotation)
    - distances between tones
    - examples of chaos and structure
    - examples of consonance and dissonance
- go to the 5-tone pentatonic circle
    - simple melodies that always sound good
- go to the 7-tone diatonic circle
    - add 2 more tones to the 5-tone circle
    - more simple melodies
    - intervals - relationship between two tones
    - chords
        - even-odd skipping
    - chord quality
        - intervals within the chords
    - the structure
        - three major chords - I, IV, V
        - three minor chords - VIm, IIm, IIIm
        - one diminished chord - VIImb5
    - the two pendula
    - the relation between major and parallel minor chords
        - I-VIm, IV-IIm, V-IIIm
        - IIm-VIImb5-V
    - distance from a tone to a key
    - various keys
        - relationship via the circle of fifths
- how to train ears?
    - for rhytms
    - for harmony - intervals, chord qualities, functions
    - how to find the key?
    - how to improvise on some music in a key?
    - how to find section in a song?
- practical analyzing songs for keys, chords, etc.
    - take some chords from the next, get aware of the key, chord functions, etc.
- chord progressions
    - common patterns in chord usage
    - dominant seventh in minor pendulum
- voice leading
    - connection between tones inside chords when chords change
    - small movements
- mirror scale - rabbit hole behing the mirror
    - tritone substitution
    - sixth chords
- going outside of a key - back to 12-tone circle
    - other scales
    - taking tones or chords from outside
    - modulation between keys
- a little miracle - why diatonic scale is so special?
    - connection between harmonic tones and diatonic scale
    - highest richness for melody and chords
    - continuous in the circle of fifths
    - the fifth of each tones excepts on points to a another tone inside the set
- tuning
    - general connection between harmonic profile and scales through dissonance
    - just intonation vs. equal temperament vs. others
    - more generalized tunings
    - how to tune a guitar? - it a tuner or ear better?
- blues
    - just a different kind of pendulum
    - back to natural tuning
- why vibrato? why it is just another face of tremolo?
- (the list goes on...)
