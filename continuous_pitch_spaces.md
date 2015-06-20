# Continuous pitch spaces

Tuning deals with an abstract model of tones and their relation to actual frequencies. In literature typically discrete pitches or pitch classes (relative to some tuning) are utilized. We can generalize them to be continuous and be less dependent on the actual tuning. The remaining parameter is the base frequency.

- unit pitch space
  - continous, unbounded
  - 1.0 ~ one octave
- step pitch space
  - continous, unbounded
  - N steps ~ one octave
  - `unit pitch space * N`
- unit pitch class space
  - continous, bounded [0, 1.0)
  - `unit pitch space % 1.0`
- step pitch class space
  - continous, bounded [0, N)
  - `unit step pitch space % N`
- integer step pitch space
  - discrete, unbounded
  - `floor(step pitch space)`
- integer step pitch class space
  - discrete, bounded {0, 1, .. N - 1}
  - `floor(step pitch class space)`
