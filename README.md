# Dogs vs Cats 

The "Dogs vs. Cats" dataset is a popular benchmark for image classification tasks, particularly for learning Convolutional Neural Networks (CNNs). It involves training a model to distinguish between images of dogs and cats, often using a subset (in this case: 3,750 cats and 3,750 dogs) of a larger dataset. The larger dataset contains 17,500 images (8,750 cats and 8,750 dogs). Ultimately, creating a function or dataset that has an image name (or an image) that recognizes if image is cat or dog. 

This project makes use of 
 - ### **NumPy** (for data preprocessing) 
 - ### **TensorFlow/Keras** (for model architecture modeling)
 - ### **VGG-16** (pre-trained deep CNN model - for feature extraction and transfer learning) 

Accuracy is measured via AUC/ROC Scores and Confusion Matrix 

## The Asirra data set
Web services are often protected with a challenge that's supposed to be easy for people to solve, but difficult for computers. Such a challenge is often called a CAPTCHA (Completely Automated Public Turing test to tell Computers and Humans Apart) or HIP (Human Interactive Proof). HIPs are used for many purposes, such as to reduce email and blog spam and prevent brute-force attacks on web site passwords.

Asirra (Animal Species Image Recognition for Restricting Access) is a HIP that works by asking users to identify photographs of cats and dogs. This task is difficult for computers, but studies have shown that people can accomplish it quickly and accurately. Many even think it's fun! Here is an example of the Asirra interface:

Asirra is unique because of its partnership with Petfinder.com, the world's largest site devoted to finding homes for homeless pets. They've provided Microsoft Research with over three million images of cats and dogs, manually classified by people at thousands of animal shelters across the United States. Kaggle is fortunate to offer a subset of this data for fun and research. 

## Image recognition attacks
While random guessing is the easiest form of attack, various forms of image recognition can allow an attacker to make guesses that are better than random. There is enormous diversity in the photo database (a wide variety of backgrounds, angles, poses, lighting, etc.), making accurate automatic classification difficult. In an informal poll conducted many years ago, computer vision experts posited that a classifier with better than 60% accuracy would be difficult without a major advance in the state of the art. For reference, a 60% classifier improves the guessing probability of a 12-image HIP from 1/4096 to 1/459.

## State of the art
The current literature suggests machine classifiers can score above 80% accuracy on this task. Therfore, Asirra is no longer considered safe from attack.  This project benchmarks the latest computer vision and deep learning approaches to this problem.

## VGG-16 Architecture & Mammalian Visual Cortex
VGG (Visual Geometry Group) modules and the mammalian visual cortex share similarities in their hierarchical processing of visual information. Both systems process visual data through multiple layers, progressively extracting more complex features as the signal moves deeper. Early layers in VGG resemble simple processing stages similar to those in the primary visual cortex (V1), which respond to basic features like edges and textures. Higher layers in VGG correspond to more abstract and complex feature representations akin to higher visual cortical areas, which integrate and interpret more detailed aspects of visual stimuli.

Studies comparing VGG16 with the mouse visual cortex show that the intermediate layers of VGG correspond roughly to mid-level visual processing in the brain, indicating the representations are higher-order than simple edge detection. Also, unlike the strictly hierarchical feedforward nature of VGG, the mammalian visual cortex may exhibit a more parallel and broader organization beyond early visual areas.

In essence, VGG networks are designed inspired by and functionally analogous to the mammalian visual cortex, with layered feature hierarchies mirroring the brain's progression from simple to complex visual processing stages.

### Acknowledgements

 - Special thanks to Professor Zia Khan & Frank Fletcher for their mentorship and code reviews. Thanks to the Microsoft Research team for providing the photographic data. The conceptual inspiration derives from the following publication:

   Jeremy Elson, John R. Douceur, Jon Howell, Jared Saul, Asirra: A CAPTCHA that Exploits Interest-Aligned Manual Image Categorization, in Proceedings of 14th ACM Conference on Computer and Communications Security (CCS), Association for Computing Machinery, Inc., Oct. 2007.

 - Thanks also to the LearningFuze and the open source community for continuous support and helpful discussions.
