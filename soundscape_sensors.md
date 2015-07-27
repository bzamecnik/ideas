# Soundscape sensors

We might be interested in recording sound from a audio sensor located at a single place continuously, ie. 24/7. This might be useful eg. for gathering data for some exploratory analysis, building a training dataset for machine learning, and performing an actual ML task.

## Examples of usage

- car traffic activity
- presence and activity of bird species
- monitoring weather - wind, rain, ...
- human activity in cities

Consider a small Raspberry Pi mini-computer act as the sensor.

## What technical problems we would need to solve?

- how and where to store the data?
  - raw mono PCM sampled at 44kHz take ~3.5 GB per day
- how to deliver the data to the storage?
  - connectivity
- how to compress the data?
  - we might assume a typical soundscape might be quite boring (ie. sparse) and could be compressed well
  - see [dynamic compression](dynamic_compression.md)
- how to deal with outages?
  - power outage, upgrade, ...
- how to explore the data?
  - how to find typical patterns?
  - how to find interesting anomalies?
- how to precisely timestamp the data?
  - NTP?
- how to combine recordings from multiple sensors?
- how to combine the data with other modalities?
