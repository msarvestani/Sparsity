# Sparsity

We look at the sparsity of neuronal responses to natural images and static gratings.

The data is 2P calcium imaging flourescence in mouse V1, made available by the Allen Institute (Allen Brain Observatory).

Sparse response distribution can be thought of as deviation from the normal gaussian response distribution. i.e. sparse distributions have most of the variance due to a few responses. One way to determine the sparsity of a response distribution is to look at the deviation of its fourth moment (kurtosis) from the known kurtosis of a normal distribution (3). Another is to use essentially a coefficient of viaration (mean/standard deviation).

We define two sparsity  metrics:

1) Lifetime sparseness: is the sparseness of the response of ONE CELL to many images. High lifetime sparsity means the cell only responds well to a few images. e.g. it is very selective.

2) Population sparseness: is the sparseness of the response of MANY CELLs to one image. High population sparsity means only a few cells from the population respond to a particular image.

The two metrics aren't necessarily related, and serve different purposes. We calculate both here.

Files in this repo:

1) sparsity_test_natural_scenes.ipynb: a jupyter notebook that downloads data from the Allen Observatory dataset and calculates sparseness of responses during natural scenes.

2) sparsity_test_static_gratings.ipynb: same as 1), but for responses during static gratings.

3) plot_sparsity_natscenes_vs_staticgratings.ipynb: a notebook that plots the mean sparsity across 16 mice, for both stimulus conditions

4) sweep_response_test.ipynb: a notebook that checks to make sure the calculated trial averages are correct
