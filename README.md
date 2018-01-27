[XXXX](#jump)

## Initial Estimation (#R1)
![Image](https://farm5.staticflickr.com/4721/26045732858_1133701b2c_b.jpg)
> Fig. 1: The bias distribution on MIT intrinsic dataset and our MIID dataset.

From the figure above, we can see that the biases between the reflectance image and the input image follow a heavy-tailed distribution with zero mean, which validate our assumption that the reflectance image has small deviation from the input image.

## PCA vs. 'Best' 8 bands (#R2)
![Image](https://farm5.staticflickr.com/4701/26047528898_29a16acf4f_h.jpg)
> Fig. 2 The comparison between PCA and selected 8 bands. We use LMSE to evaluate the performance.

## <span id="mit">On MIT Intrinsic Dataset</span>
![Image](https://farm5.staticflickr.com/4714/26047185008_06ce9cf270_k.jpg)
> Fig. 3: Comparison of visual results, where GT denotes Ground Truth and CR denotes Color Retinex.

![Image](https://farm5.staticflickr.com/4714/25049103807_9b4d41bcf9_h.jpg)
> Fig. 4: The quantitative performance of our method.

## MIID Dataset
![Image](https://farm5.staticflickr.com/4704/39918684321_42faa1c719_k.jpg)
![Image](https://farm5.staticflickr.com/4761/39019998775_fa2a84c34a_k.jpg)
> Fig. 5: The first subfigure is 12 groups that we provided in the paper. The second one is newly-captured 10 groups to validate the performance of our algorithm.

### Objective evaluation
![img](https://farm5.staticflickr.com/4743/39022043025_103a809018_b.jpg)
> Fig. 6: LMSE performance on our newly-captured dataset. Our algorithm achieve better results on every group of 10.

### Subjective evaluation
![img](https://farm5.staticflickr.com/4604/39890672712_98326ccd3d_k.jpg)
> Fig. 7: Visual results of our algorithm on newly captured dataset. Noted that we use 2 different spectral imagers, so there may be a little color difference caused by different white balance methods.

## Performance on SIID dataset.
### Objective evaluation
![Image](https://farm5.staticflickr.com/4611/28140381309_f9179756b9_b.jpg)
> Fig. 8: the performance of our algorithm on SIID dataset. *SIID dataset and Error rate is proposed by Chen et al. _Intrinsic decomposition from a single spectral image._ Applied optics 56.20 (2017): 5676-5684.

<!--### Subjective evaluation>
