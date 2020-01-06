# goban_data_set

In this repo you'll find a data set of 494 photos of go boards (1000x1000 rgb) with corresponding labels in xml format for the corners coordinates of both board and field corners, 
and 3240 segments (20x20 gray) with corresponding labels in xml format for 'empty', 'white' or 'black' field.

Moreover I'm sharing my jupyter notebooks and trained models I intend to improve [Goban-to-SGF](https://github.com/irglbriz/goban_to_sgf) with. 

Especially ['CornerSegmentationUNet.ipynb'](https://github.com/irglbriz/goban_data_set/blob/master/CornerSegmentationUNet.ipynb) could be interesting to play around with. It showcases how to build a custom data generator with random data augmentation outputting automatically generated masks in order to train a segmentation model based on the u-net architecture. This enables classic contour detection to precisely find the corners and warp the image into a clean top-down view. 
