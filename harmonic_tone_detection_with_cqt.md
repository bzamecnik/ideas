# Harmonic Tone Detection with CQT

Now we detect fundamental frequencies of harmonic tones among their harmonics using a correlation with a harmonic comb with the CQT spectrum. Tones with harmonics get higher weight that tones without them.

One of the problems is that the harmonics are not precisely aligned with the equally tempered CQT bins. Also the fundamental might be off. Also the harmonics might be off the ideas integral multiples.

We can use interpolation of the CQT bins to get approximate values "in between" bin centers. Also we can use the frequency estimation from phase difference to get better frequency estimate of harmonics.

[image - errors]
- for each bin:
    - if the bin's amplitude is high enough
        - make high-precision estimate
    - using the comb pattern
        - find the amplitudes for each harmonic (using interpolation of bins)
            - is it possible?
        - compute the for product
    - use this product weight and fundamental's amplitude to construct a compound weight (also use total amplitude)
    - threshold the tones by this weight
