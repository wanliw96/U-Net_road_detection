# U-Net_road_detection

Automatic road extraction from remote-sensing imagery plays a critical role in many applications. However, accurate and efficient extraction from high-resolution images remains hard because of the image size, spatial diversity for road targets and disturbances (e.g., trees and buildings), etc. The goal of this project is to use U-Net architecture together with data augmentation to execute the fast acquisition of weak road information while avoiding noise.   

## Data
Training set:
- Input: ten thousand satellite images
- Output: ten thousand corresponding boolean masks

Test set:
- Input: two thousand satellite images

All the images and masks used in the project is downloaded from DeepGlobe (http://deepglobe.org). Each image covers roughly 16 acres of land in a 256 m by 256 m cube. Each image is of size 512 by 512 resulting in a pixel resolution of 50 cm. For the boolean masks, the road pixels are labeled as one, and non-road pixels are labeled as zero.
