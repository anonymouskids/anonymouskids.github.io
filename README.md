# Rebuttal material: Multispectral Image Intrinsic Decomposition via Low Rank Constraint

[Inital Estimation (#R1)](#init)

[PCA vs. 'Best' Bands (#R2)](#lr)

[Experiments (#R3)](#mit)
* [on MIT intrinsic benchmark](#mit)
* [on MIID, our newly-captured dataset](#miid)
* [on SIID dataset](#siid)

[Contributions (#R3)](#contri)

## <span id="init">Initial Estimation (#R1)</span>
![Image](https://farm5.staticflickr.com/4721/26045732858_1133701b2c_b.jpg)
> Fig. 1: The bias distribution on MIT intrinsic dataset and our MIID dataset.

From the figure above, we can see that the biases between the reflectance image and the input image follow a heavy-tailed distribution with zero mean, which validate our assumption that the reflectance image has small deviation from the input image.

## <span id="lr">PCA vs. 'Best' 8 bands (#R2)</span>
![Image](https://farm5.staticflickr.com/4701/26047528898_29a16acf4f_h.jpg)
> Fig. 2 The comparison between PCA and selected 8 bands on our MIID dataset. We use LMSE to evaluate the performance. With PCA, our algorithm outperforms best-band method by 38% on average.

## <span id="mit">Experiments (#R3)</span>


### <span id="mit">On MIT Intrinsic benchmark</span>
![Image](https://farm5.staticflickr.com/4714/26047185008_06ce9cf270_k.jpg)
> Fig. 3: Comparison of visual results on MIT intrinsic benchmark (first row: reflectance; second row: shading), where GT denotes Ground Truth and CR denotes Color Retinex. Our shadings are more uniform and reflectances are more 'flat' visually.

![Image](https://farm5.staticflickr.com/4714/25049103807_9b4d41bcf9_h.jpg)
> Fig. 4: The quantitative performance of our method. 

To better illustrate our algorithm, we test our algorithm on MIT intrinsic benchmark. In Fig. 3, we display some results on MIT dataset. Compared with CR, our algorihtm on RGB cases would also achieve great visual results. In Fig. 4, we evaluate our algorithm quantitatively. Since we directly operate on image domain, the performance would elavate a little, from 0.030 to 0.028 on average.

### <span id="miid">On MIID Dataset</span>
![Image](https://farm5.staticflickr.com/4704/39918684321_42faa1c719_k.jpg)
![Image](https://farm5.staticflickr.com/4761/39019998775_fa2a84c34a_k.jpg)
> Fig. 5: The first subfigure is 12 groups that we provided in the paper. The second one is newly-captured 10 groups which validate the performance of our algorithm.

Apart from 12 groups MIID dataset provided in the paper, we add 10 groups in order to demonstrate the contribution of our algorithm. We mainly compare our algorithm with SIID*, the latest algorithm on MIID problem.

> *Chen et al. _Intrinsic decomposition from a single spectral image._ Applied optics 56.20 (2017): 5676-5684.

#### Objective evaluation
![img](https://farm5.staticflickr.com/4743/39022043025_103a809018_b.jpg)
> Fig. 6: LMSE performance on our newly-captured dataset. Our algorithm achieve better results on every group of 10.

In Fig. 6, we show LSME performance of our algorithm. This time our algorithm outperform SIID on each group of images, which validate the effectiveness of our algorithm.

#### Subjective evaluation
![img](https://farm5.staticflickr.com/4651/39214501674_088371962d_k.jpg)
> Fig. 7: some visual results of our algorithm on newly captured dataset. Captured by two different spectral imagers, colors of the images are slightly different from each other because of different white balance methods.

SIID introduced super-pixel based method to handle MIID problem in order to reduce the complexity of multispectral information. Their results would cause the mosaic effect, in other words, the loss of details. In Fig. 7, we demonstrate that our algorithm can better maintain the detailed information. And our shadings tend to be uniform and reflectances are more 'flat'.

Noted that in the group 'cap' our results appear to be worse, but our algorithm maintains high frequency information on shading image, so our performance are better.

### <span id="siid">On SIID dataset</span>
![Image](https://farm5.staticflickr.com/4611/28140381309_f9179756b9_b.jpg)
> Fig. 8: the performance of our algorithm on SIID dataset. *SIID dataset and Error rate is proposed by Chen et al. _Intrinsic decomposition from a single spectral image._ Applied optics 56.20 (2017): 5676-5684.

Also, we do another experiment on SIID dataset. Using the error evaluation term defined in Chen et al.'s paper, we achieve better results quantitatively.

## <span id='contri'>Contributions (#R3)</span>
In sum, our LRIID algorithm outperforms state-of-the-art algorithms on various kinds of databases. And MIID dataset we provide with the ground truth would play an important role in following MIID research.

<!--### Subjective evaluation>
