## Harris Corner Kps and Descriptors Extraction

This Harris Corner Kps extraction codes based on the calculation of Heissen matrix of the Gaussian Kernel windows, estimating the corner points by det(M)/trace(M)

## R function (Harris response)

- Images after gaussian filters
![Pic](Test Result1.png)
- Second derivatives in x->x direction, x->y direction, y->y directions
- M is the 2*2 matrix computed from image derivatives:
![Pic](Test Result2.png)
- R response = det(M)/trace(M)

## Candidate corner points and threshold

- get coordinates of candidates and their values (the R response point value > threshold)
- sort candidates
- set a min_distance and choose the candidates with the minimum distances

![Pic](Test Result.png)
