# Time-series browser

## Goal

Have a software to interactively visualize time-series.

Examples:

- financial time-series - discrete events with scalar or vector values
  - eg. stocks, FX, etc.
- time-frequency distribution - 2D distribution
  - eg. music spectrogram

## Motivation

### Financial data

In finance there underlying events representing trades that happpened at some time, price and volume. Since there's a vast amount of such events and the raw data are quite valuable a standard aggregation is to provide statistics for time blocks (days, minutes, seconds) - open-high-low-close (OHLC) price and sum of volume. The OHLC stats on one hand encode all events within a block into constant space but provide just a bounding box of the actual events - outliers. Another way to represent a vast amount of events in a limited way but using all the information is to compute a quantized distribution - a 2D histogram. Integrate the volume into blocks of time and price.

A nice visualization should be able to:

- zoom into a specified region
- pan (move around)
- compute marginal distributions for a selection (in one or another axis)

When visualizing the data it would be great to aggregate the events into histograms for each (pan-zoom) view and depending on the window and screen resolution.

On the very high zoom level the original event values could be seen.

### Audio TF data

In time-frequency analysis (not limited to audio) we're interested in distribution of energy over two domains (time and frequency). We'd like to be able to explore the data in a similar way as described above. This thing is still how to integrate the energy so it is displayed well.

For musical data there might be additional useful features:

- synchronous playback with an audio track
- various y domains (linear frequency, log frequency, pitch, pitch class, etc.)
- various x domains (seconds, beats, etc.)

### Other notes

- the input might be lists or sparse matrices
- multiple data sources could be overlaid
  - full distribution as a histogram + line plots of median and some quantiles
