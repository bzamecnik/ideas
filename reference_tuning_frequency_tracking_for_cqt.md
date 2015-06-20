# Reference Tuning Frequency Tracking for CQT

The CQT bins depend on the reference frequency. It it changes the CQT kernels would need to be recomputed.

We could use the same fixed bins all the time and compute the precise tone frequencies using the high-precistion method. Then we could compute the most likely offset to the canonical reference frequency (using e.g..the least squares method).

If the computed current reference frequency differs from the canonical one ( with which the CQT bins were computed the CQT bins would no longer correspond to the tones in the new tuning. Thus we need to shift the intervals for tones in current tuning with respect to the cQT bins. Here interpolation could be quite useful.

Care must be taken for slide tones. There should be some time-domain averaging.

The interpolation could be useful firstly for resampling of the data from the original bins, secondly to obtain approximate data between bins (eg. resampling not restricted to the shifted bins).

Note that the pass is wrapped (unless we track the wraps).
