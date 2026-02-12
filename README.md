# pixel-coordinate-prediction
 Dataset Rationale and Application :

In this work, we generated a synthetic dataset by dividing a 50×50 pixel board into circular regions based on the distance from the center. The primary purpose of this dataset is to predict the (x, y) coordinates of the target hit on the board. By knowing the exact location of the hit pixel, we can train a deep learning model to map the board image to the coordinates of the hit.

This approach is particularly useful in scenarios such as:

1.Target practice systems, where the aim is to identify which part of a board was hit.

2.Game-based training applications, where scoring depends on the precise location of hits.

3.Human-computer interaction tasks, where understanding user actions on a 2D interface is required.

By dividing the board into clearly defined regions with distinct color coding, the dataset provides structured spatial information that facilitates accurate coordinate prediction. The inclusion of boundary regions further helps the model handle edge cases, where a hit falls near the border of two rings.

Image Pixels Framing into Regions :

The code divides a 50×50 image into circular regions based on the distance from the center. First, it calculates the center of the image. Then, for every pixel, it computes its distance from the center. Based on this distance, each pixel is assigned to a circular region (R1, R2, R3, R4, R5, R6).

If a pixel lies exactly on the boundary between two circles (for example, between R1 and R2), it is assigned to a special boundary region, such as R1-R2. As a result, the image is divided into six main circular rings and five boundary rings, making a total of eleven regions. The boundary regions — R1-R2, R2-R3, R3-R4, R4-R5, and R5-R6 — ensure that pixels partially overlapping two rings are represented accurately.
