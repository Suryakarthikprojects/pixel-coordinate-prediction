# pixel-coordinate-prediction

Approach For Dataset : This code generates a synthetic dataset of 5960 grayscale (50×50) images by creating random snake-shaped paths with varying intensity values and placing a single fruit pixel (value 255) at a random unoccupied location. For each grayscale image, it also generates a corresponding binary fruit-only image, where the fruit pixel is set to 1 and all other pixels are 0.

The binary fruit-only image is used as the input for the deep learning model, while the fruit coordinates (x, y) serve as the target labels for supervised learning. Finally, all images are saved, and the fruit coordinates, snake length, and file paths are stored in a JSON label file for training and evaluation.
