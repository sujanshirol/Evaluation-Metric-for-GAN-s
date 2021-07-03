# Evaluation Metric for GAN's
The evaluation of supervised image classification is simple. The projected output must be compared to the actual production. To get this fake(generated) image, though, you use a GAN and some random noise. This created image should appear as authentic as possible. So, how do you measure the reality of this computer-generated image? Or, to put it another way, how can you assess GAN?

## Frechet Inception Distance(FID) Score
One of the most widely used measures for determining the feature distance between real and produced images is Frechet Inception Distance (FID). Frechet Distance is a measure of similarity between curves that takes the placement and ordering of points along the curves into account. It can also be used to calculate the difference between two distributions.

![image](https://user-images.githubusercontent.com/71747522/124357677-7095a000-dc3a-11eb-9d0d-ac1768510ae7.png)

Where μ and σ are the mean and standard deviation of the normal distributions, X, and Y are two normal distributions.

Inception V3 model is employ, which has been pre-trained on the Imagenet dataset, for GAN evaluation. The score is called "Frechet Inception Distance" because it uses activations from the Inception V3 model to summarise each image.

The Frechet Inception Distance for "multivariate", normal distribution, that is GAN, is given by

![image](https://user-images.githubusercontent.com/71747522/124357804-07625c80-dc3b-11eb-8eef-5c9e3203fffc.png)

where X and Y are the real and fake embeddings. μX  and μY are the magnitudes of the vector X and Y. Tr is the trace of the matrix.










Credits [Ayush Thakur](https://wandb.ai/ayush-thakur/gan-evaluation/reports/How-to-Evaluate-GANs-using-Frechet-Inception-Distance-FID---Vmlldzo0MTAxOTI)
