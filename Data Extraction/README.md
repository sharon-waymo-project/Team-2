# Data Extraction

This directory contains the python code for extracting the data from the tfrecord files.
The extracted features are [vx, vy, vz, dx, dy, vfx, vfy, vfz, afx, afy, afz], and the labels are [ax, ay, az]

## Input
For running the code in this file, we need 1 inputs:

1) The list of names of the tfrecord files.

### Running the model:
Running this model is very easy as you just need to provide the path  of the inputs mentioned above, and the script can be run as it is.

### Runtime of the model:
The runtime of this script varies on the amount of tfrecord files to be processed.

### Dependencies:
There are multiple Python libraries that are necessary to run this model. They are:
1) TensorFlow
2) Numpy
3) waymo_open_dataset
4) shapely

### Outputs:
After running the code, CSV file containing the features of all the tfrecord files will be generated

