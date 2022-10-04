# U-Net_road_detection

Automatic road extraction from remote-sensing imagery plays a critical role in many applications. However, accurate and efficient extraction from high-resolution images remains hard because of the image size, spatial diversity for road targets and disturbances (e.g., trees and buildings), etc. The goal of this project is to use U-Net architecture together with data augmentation to execute the fast acquisition of weak road information while avoiding noise.   

## Data
All the images and masks used in the project are downloaded from DeepGlobe (http://deepglobe.org). Each image covers roughly 16 acres of land with a size of 512 by 512. For the boolean masks, the road pixels are labeled as one, and non-road pixels are labeled as zero. Some example images are in the example_data folder.

Training set:
- Input: ten thousand satellite images
- Output: ten thousand corresponding boolean masks

Test set:
- Input: two thousand satellite images

## Data preprocessing:
- Resize the image: 
The original images and boolean masks are of size 512 x 512. They are resized to 128 x 128 to improve the computational efficiency.
