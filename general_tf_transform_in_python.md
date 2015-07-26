# Implement general parametrized time-frequency transform in Python

Make a Python port of an existing MATLAB implementation of GPTFT: http://tfd.sourceforge.net/

The point of this family of transforms is to adapt to the data. Short-time Fourier/chirplet/wavelet transforms integrate the TF plane on a (ir)regular (possibly rotated) rectangular grid regardless of the data. However it is possible to adaptively choose kernels fitted for the actual data that can provide more accurate information about the TF energy distribution.

There's an existing MATLAB implementation, but it is not too actively maintained. It would be beneficial to have the same tools available in Python via a nice pythonic interface.

We could then eg. extract more accurate features for visualization or machine learning.

## References:

- Yang Y., Peng Z.K., Dong X.J., Zhang W.M., General parameterized time-frequency transform, IEEE Transactions on Signal Processing, 62(11), pp 2751-2764, 2014.
