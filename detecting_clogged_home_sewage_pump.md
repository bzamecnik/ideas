# Detecting clogged home sewage pump

A practical home ML application.

![](http://inspectapedia.com/septic/SepticTankPumpout38DF.jpg)

## Motivation

Consider a house with sewage water collected in a cesspit. After years it has been connected to the public sewer system. Each year the shit in the cesspit needs to be manually pumped into the sewers though an underground pipe.

The problem is the pump often clogs and needs to be cleaned. The only place to figure this out is the sewage manhole located at some distance from the pump (let's call it the sink). Typically one person operates the pump and the other monitors the sewers and makes an alert when the water stops to flow or start to flow again. Without a mobile phone or radio it might be hard to communicate efficiently on the distance. And this is a quite boring job. So why not to leave it to machines?

## Possible solutions

### Video stream

One possibility is just to put a camera with microphone into the sink and stream it to a display next to the pump. This is quite easy to set up but still leaves the decision on the pump operator. This might not be practical since the pump can be noisy, the pump operator might not be able to see or hear the video stream while being submerged into the cesspit. It is not so cool.

### Clog detection via ML

We can do more since. This problem can be formulated as a machine learning problem. The input is a time series of features and the output is just a binary classification of each time frame. Upon this we might then report any significant state change (clogged, running). The actual message can be provided via text-to-speach or a sound signal played from another mini-computer or mobile phone near the pump operator. It can be loud enough to be perceived even under noise.

We can monitor the sewers sink by various mean. A simple to obtain signal is audio taked by a microphone. Also we can take a video stream. Both can be taked via a mobile phone or a mini-computer and do not need contact with the sewage water.

#### Data collection

This year I have managed to collected some data - both audio and video - and I plan to analyze it, label it and publish it. Basically any recording of running water should be close enough but at least this could be useful for testing the system.

#### Features

For the audio data at least the spectrogram could be a good start.

For the video data some kind of motion detection could be helpful (optical flow?). Basically there should be some flow in one direction and also some diagonal patterns from the edges to the center. Image registration might be unnecessary in case we're able to fix the camera in a stable tripod.

#### Training the model

Try any favorite method...

## Conclusion

Good luck with the shit. :)
