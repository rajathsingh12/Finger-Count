# Finger-Count
This is a program that detects a hand, segments the hand, and counts the number of fingers that are held up in the red square box.

## Strategy used.

- Grabbing an ROI (Region of Interest).
- Calculating Running Average Background value for 60 FPS.
- Once when the Average Value is found, we enter our hand into the ROI region.
- After the hand enters the ROI, we can detect it and find changes and apply thresholding. 
- To detect the fingers we use Convex Hull to draw polygon around our hand.
- By some math we can detect the center of hand and apply it against to the outer angle to match finger count.  


## Libraries Used.

- Numpy
- Scikit Learn (Pairwise)
- OpenCV


