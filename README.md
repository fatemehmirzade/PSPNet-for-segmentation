# PSPNet-for-segmentation

The implementation of the Pyramid Scene Parsing Network (PSP-Net) has been executed to facilitate object segmentation within underwater environments, specifically on the SUIM dataset.

The SUIM dataset serves as a cornerstone for semantic segmentation of underwater visual data. It encompasses various object categories, each associated with distinct symbols and RGB color codes:

Background (waterbody) - BW - RGB: 000 (black)
Human divers - HD - RGB: 001 (blue)
Aquatic plants and sea-grass - PF - RGB: 010 (green)
Wrecks and ruins - WR - RGB: 011 (sky)
Robots (AUVs/ROVs/instruments) - RO - RGB: 100 (red)
Reefs and invertebrates - RI - RGB: 101 (pink)
Fish and vertebrates - FV - RGB: 110 (yellow)
Sea-floor and rocks - SR - RGB: 111 (white)
The directory structure is organized as follows:

train_val/: encompasses 1525 paired samples designated for training and validation:

images/: contains RGB images portraying underwater scenes
masks/: stores segmentation labels wherein each RGB color signifies a distinct object category
Further elucidation can be found in the paper (Section III)
TEST/: comprises 110 paired samples for benchmark evaluation:

images/: houses RGB test images
masks/: accommodates ground truth labels
Combined RGB masks are available
Individual binary masks are also provided in separate directories
Benchmark_Evaluation/: hosts all experimental data pertinent to the state-of-the-art (SOTA) models.

The network's performance is assessed utilizing the Mean Intersection over Union (mIoU) metric and the Cross Entropy loss function.

PSP-Net, alongside other deep neural networks, represents an advanced methodology for comprehending scenes and parsing images. These networks are characterized by architectures endowed with deep and intricate layers, enabling robust segmentation and recognition of objects and diverse image components.

PSP-Net facilitates a meticulous analysis of scenes depicted within an image by leveraging convolutional layers and complementary layers to extract multifaceted information from the image. This extracted information is instrumental in segmentation and comprehensive analysis, encompassing insights derived from the image's surroundings.

Concerning the application of PSP-Net for semantic segmentation, it entails the segmentation of objects and identification of various elements within a scene. Leveraging networks like PSP-Net facilitates the automated identification and categorization of objects within an image, rendering it applicable across diverse domains such as medical image processing and autonomous vehicles.

The mIoU metric serves as a pivotal measure of model efficacy in object detection and segmentation within images, representing an accuracy metric tailored for models operating with pixel-labeled data. It is computed by assessing the intersection area between the predicted model and ground truth labels relative to their union area, subsequently averaging across all categories.

The Cross Entropy loss function stands as a ubiquitous metric for classification problems, employed to gauge the disparity between the model's predicted distribution and actual labels. This function computes the average loss across all samples, with 'y' representing the ground truth labels and 'y^' denoting the predicted labels by the model.

Leveraging these concepts enables the evaluation of model quality in object detection and image segmentation, alongside the enhancement of model performance through optimized loss function calibration.
