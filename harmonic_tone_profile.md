# Harmonic tone profile

In practice tones (stationary sounds) are composed of multiple frequences (partials). Many musical instruments produce tones where the partial frequencies are (precisely or approximately) integer multiples of the fundamental frequency. Such partials are called harmonic partials (or harmonics) and such a tone is called a harmonic tone.

What we might be interested is the profile of the partials, ie. a set of frequencies, their amplitudes and phases. All usually constant, but possibly time-varying (ie. non-stationary).

- detect the fundamental frequency
- compute the ideal harmonic frequencies
- detect the actual partials
- match the actual partials to the ideal ones
- compute how they differ in frequency
- find out the amplitudes of each partial
- find out relative phases
- compute this for multiple frames in time
    - explore the [non-]stationarity
- visualize
    - find out how

This might be a useful feature eg. for classification of musical instruments.

