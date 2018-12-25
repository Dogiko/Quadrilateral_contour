# Quadrilateral contour

For given data points in 2-D Euclidean space, getting suitable quadrilateral boundary by gradient descent.

1. Use PCA to normalized data points.
2. Generate fake points uniformlly between -4 to +4 standard deviation.
3. Train a NN-Discriminator to verify data points, with layer 2-4-1 and sigmoid function.
4. Treat the weight of first linear transformation in NN as quadrilateral boundary.

The concept can be Considered as simple GAN with single adversarial round.