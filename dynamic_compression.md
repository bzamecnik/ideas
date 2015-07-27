# Dynamic compression

Consider the [soundscape sensor](soundscape_sensors.md) problem, ie. recording a continuous stream of sound from one location. The data might be very sparse and could be compressed well. However with having more data we can compress better.

The interesting possibility is to change the compressed representation over time as the compression models learns from more data. The assumption is that the model can improve and achieve higher compression ratio. The other requirement is to loose no or minimum information.

How to do it?
