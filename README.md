# Image Classification for a City Dog Show

## Project Overview

This project is designed to improve your Python programming skills while working with a pre-built image classifier. Your task is to help classify images of dogs submitted for a citywide dog show. Specifically, you'll ensure that only images of actual dogs are registered by using a provided image classifier.

## Project Goal

You will apply Python tools to:
- **Identify dog breeds** using an existing image classifier.
- **Determine which classifier architecture** (AlexNet, VGG, or ResNet) works best for identifying dog images.
- **Measure performance** in terms of accuracy and runtime for each classifier architecture.

## Problem Context

The city dog show requires every participant to submit an image of their dog. However, some participants may attempt to register pets that aren’t dogs. Your job is to use a pre-developed classifier to determine whether the submitted image depicts a dog. If it does, the system will further classify the dog's breed.

This project does not require you to create an image classifier from scratch. Instead, you'll use a provided function to evaluate and analyze various CNN architectures for their ability to classify images correctly and efficiently.

## How It Works

The provided classifier function utilizes convolutional neural networks (CNNs) trained on the **ImageNet** dataset, which contains 1.2 million images across various categories. The classifier function supports three CNN architectures:
1. **AlexNet**
2. **VGG**
3. **ResNet**

These architectures have different structures, strengths, and trade-offs in terms of accuracy and speed. Your task will be to experiment with each architecture to identify which performs best in classifying dog images and determining specific breeds.

## Your Tasks

1. **Classify Images**:
   Use the classifier to categorize images as either “dog” or “not dog.”

2. **Identify the Best Classifier**:
   - Test the three CNN architectures (AlexNet, VGG, ResNet).
   - Compare their performance in correctly identifying images of dogs.

3. **Evaluate Dog Breed Classification**:
   - Once a dog is identified, evaluate the algorithm's ability to correctly classify the breed.

4. **Measure Runtime**:
   - Track the amount of time each architecture takes to complete the classification.
   - Consider the trade-off between classification accuracy and runtime.

## Instructions

1. **Setup**:
   - Clone this repository to your local machine.
   - Ensure you have Python 3.x installed along with any required dependencies (see the [Requirements](#requirements) section below).
   
2. **Classifier Function**:
   - The classifier function is located in `classifier.py`. This function loads one of the CNN architectures and classifies the input image.
   
3. **Example Code**:
   - Review the `test_classifier.py` file for a demonstration of how to use the classifier function. You can modify this script to implement your own classification tests.
   
4. **Run Your Tests**:
   - Classify a variety of images using the different architectures and measure both accuracy and runtime.

5. **Performance Analysis**:
   - After running your tests, compare the results of each classifier and determine the best performer based on your criteria (e.g., accuracy, speed).

## Requirements

To run this project, you will need:
- Python 3.x
- `classifier.py` (pre-developed classifier function)
- Basic understanding of Python, CNNs, and image classification
- Necessary Python libraries: `torch`, `torchvision`, and `PIL` (Install them with `pip install -r requirements.txt`)

## Similar Breeds Challenge

Certain breeds of dogs may be difficult for the classifier to differentiate due to their physical similarities. Pay close attention to the following dog breed pairs, which the classifier might struggle with:
- **Great Pyrenees** and **Kuvasz**
- **German Shepherd** and **Malinois**
- **Beagle** and **Walker Hound**

These similar-looking breeds pose additional challenges for image classification algorithms, making it harder for the model to distinguish between them accurately. Your task includes evaluating how well each architecture handles these challenging cases.

## Expected Outcomes

By the end of this project, you should be able to:
- Compare the effectiveness of different CNN architectures (AlexNet, VGG, and ResNet) in classifying dog images.
- Understand the trade-offs between accuracy and runtime for image classifiers.
- Improve your Python programming skills by applying them to a real-world image classification problem.

## FAQs and Additional Resources

For further clarifications on the project and CNN architectures, check the [FAQs](#) or explore additional resources provided in the links.

---