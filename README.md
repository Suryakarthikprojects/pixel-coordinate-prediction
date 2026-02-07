# pixel-coordinate-prediction

Approach For Dataset : This code generates a synthetic dataset of 50×50 grayscale images by creating random snake-shaped paths of different lengths (1 to 1200) and placing one fruit pixel (value 255) at a random empty location. For deep learning training, it also creates a fruit-only binary image where only the fruit pixel is 1 and all others are 0. Finally, it saves all images and stores the fruit coordinates (x, y) and other details in a JSON label file.
