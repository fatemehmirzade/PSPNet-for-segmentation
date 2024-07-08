# PSPNet-for-segmentation

Implementation of Pyramid Scene Parsing Network: PSP-Net has been made for the segmentation of objects in underwater scenes on the SUIM dataset. One of the cornerstones of semantic segmentation in underwater visual data is the SUIM dataset. It consists of different categories of objects, each with different symbols and RGB color codes, which are:

Background (waterbody) - BW - RGB: 000 (black) Human divers - HD - RGB: 001 (blue) Aquatic plants and sea-grass - PF - RGB: 010 (green) Wrecks and ruins - WR - RGB: 011 (sky) Robots (AUVs/ROVs/instruments) - RO - RGB: 100 (red) Reefs and invertebrates - RI - RGB: 101 (pink) Fish and vertebrates - FV - RGB: 110 (yellow) Sea-floor and rocks - SR - RGB: 111 (white) The directory structure is organized as follows:

train_val/: encompasses 1525 paired samples designated for training and validation:

images/: contains RGB images portraying underwater scenes masks/: stores segmentation labels wherein each RGB color signifies a distinct object category Further elucidation can be found in the paper (Section III) TEST/: comprises 110 paired samples for benchmark evaluation:

images/: houses RGB test images masks/: accommodates ground truth labels Combined RGB masks are available Individual binary masks are also provided in separate directories Benchmark_Evaluation/: hosts all experimental data pertinent to the state-of-the-art (SOTA) models. The network's performance is assessed utilizing the Mean Intersection over Union (mIoU) metric and the Cross Entropy loss function. Among the globe's latest and most leading-edge methodology in scene understanding and image parsing would be PSP-Net, and other deep neural networking. Such networks bear deep, complexly engineered architectures that enable robust segmentation and recognition of objects and various elements of an image.

PSP-Net facilitates a meticulous analysis of scenes depicted within an image by leveraging convolutional layers and complementary layers to extract multifaceted information from the image. This extracted information is instrumental in segmentation and comprehensive analysis, encompassing insights derived from the image's surroundings. In the area of semantic segmentation, PSP-Net applies to the segmentation of objects and identification of the various elements that exist within a scene. Allowing networks such as PSP-Net, through which objects within an image can be identified and categorized automatically, opens the way for applications across very disparate domains, from medical image processing to driverless vehicles.

The mIoU metric serves as a pivotal measure of model efficacy in object detection and segmentation within images, representing an accuracy metric tailored for models operating with pixel-labeled data. It is computed by assessing the intersection area between the predicted model and ground truth labels relative to their union area, subsequently averaging across all categories.

Ultimately, the code retrieves and showcases images of input data alongside network predictions.
![image](https://github.com/fmirzadeh99/PSPNet-for-segmentation/assets/169579231/8c815fd5-b052-4d7e-a278-20c06977ba8e)



