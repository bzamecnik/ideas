# Multi-focal time-frequency analysis

Standard time-frequency analysis, such as [STFT](https://en.wikipedia.org/wiki/Short-time_Fourier_transform) or [reassigned STFT](https://en.wikipedia.org/wiki/Reassignment_method) impose a trade-off between time and frequency resolution driven by the window size parameter. A shorter window allows better time resolution and worse frequency resolution and vice versa.

It looks analogously to focusing a camera back and forth to a plane at some distance. With a single shot it is not possible to focus at the whole range of distances. Some areas are in focus while other are blurred.

However, it is possible to combine multiple images and take just the focused part from each image. This is studied as [Multi-focus image fusion](https://scholar.google.cz/scholar?q=Multi-Focus+Image+Fusion) and is already used in the image-processing domain.

It would be interesting to apply the multi-focal methods also to the domain of time-frequency analysis of 1D signal such as sound.
