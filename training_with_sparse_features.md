# How to train with sparse features?

How to train a machine learning model when the features have the following properties?

- are sparse - a few non-zero values
- the range of values is large and possibly unbounded
- eg. a histogram - discretized distribution of some random variable

Typically ML algorithms accept a fixed-size set of features. However for many application a distribution of some variable might be a good feature.

Possible approaches:

- feature hashing
