## Presentation View Link

https://canva.link/4bbyr8zu5sj5gf2

## Video Link

https://o365coloradoedu-my.sharepoint.com/:v:/g/personal/ablu2313_colorado_edu/IQCrtuBbCr9JTLpslE7XFqNIAQNbiNbMafE_VG7p9RgiE7o?e=3CAHaw

**Abstract**

This presentation introduces the idea of the Non-Uniform Fast Fourier Transform (NUFFT) by building an intuition with its parent algorithms,
the Discrete Fourier Transform (DFT) and the original Fast-Fourier transform. (FFT)
We'll find that the NUFFT is unique only that in it adds a convolution and de-convolution step in order to handle data points that are not sampled at equispaced intervals.
The Flatirons Institute NUFFT library (FINUFFT) chooses to implement the NUFFT with the smoothing kernel 'expoenntial of semicircle'.
We run 1D experiments comparing the FINUFFT library to the O(NM) sum. We find that FINUFFT overtakes the direct sum beyond a few hundred points, that tightening the tolerance reduces error with diminishing gains, and that it remains accurate for typical inputs even with tightly clustered points.
For inputs whose true output nearly cancels, the relative error grows large, revealing the ill-conditioning of the question being asked rather than a flaw in the FINUFFT implementation of the algorithm.
A more interesting study of the library would likely center on its choice of smoothing kernel, compared to alternative choices, as well as testing the inverse operations of the higher dimension transforms.