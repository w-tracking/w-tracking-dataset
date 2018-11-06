# w-tracking dataset
This dataset contains 3 clips shot synchronously by 3 cameras, and 3600 continuous frames for each clip. Challenging situations for visual tracking, such as occlusion, visual ambiguity, apperance variations, etc. will be present as time goes on.

## annotation
Currently, annotations(including positions of bounding box, 3D trajectory) for one of four persons has been given at [./annotations](./annotations), more annotations will be published soon.

## image sequences
The published images sequences are derived from rectifying original images with the distortion coefficients([./cameras parameters](./camera_parameters)), and the upper 24 rows of pixels have been removed for aesthetics, so it needs to project the points in world coordinate with only rotation matrix and translation vetor, and minus 24 in y-axis while finding the correspongding pixels in image coordinate.   
