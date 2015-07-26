# Bell classification

- find/record a dataset of bells
- train a ML model
- classify bells
  - sounds from the same bell should have the same label
  - good features could be the profile of sinusoids

## Notes

- bells sounds typically consist of a set of non-harmonic sinusoids

## Bell app

It could be used in a mobile app / web service:

- a user records a bell sound via a smartphone
- the original sound or its features are sent to the cloud part of the app
- a similarity query is performed against a database of known bells
- a description is returned for a known bell
  - name, location, age, etc.
- the user could add bell info in case the bell is not known, or fix it
