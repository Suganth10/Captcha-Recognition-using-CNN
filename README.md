# Captcha-Recognition-using-CNN
Automatic Captcha recognition using Convolutional Neural Networks

Problem Statement:
There are several websites today which still use the traditional Captchas which is a combination of Letters and Numbers. These websites end up being at risk of their data getting updated automatically by bots. The goal of this project is not only to accurately identify the captchas but also to understand what characteristics a captcha should have in order to be effective.

Background:
Captchas have defeated machines, but things are changing rapidly as technology improves. Hence research into Optical Character Recognition (OCR) is required to strengthen Captchas against machine-based attacks.

Scenario and Approach:
For instance, let us look at a captcha of length 4 there are 36x36x36x36 combinations that is 1,679,616 unique combinations. Increasing captcha length increases combinations.
To train captchas directly with Neural networks would require us to generate huge amount of data and computing resources to train the model.
So, what is the alternate solution?
Alternative approach is to make the model identify characters rather than mapping entire captcha. So, the idea is to take the captcha images and identify and create images of individual characters as training data. Then this data can be used to train the model and detect captchas using divide and conquer approach.

Implementation:
The CNN model is implemented using Keras. For detailed implementation procedure kindly go through attached python notebook.
Insights from the project:
1. The applications containing Captchas with no ‘noise’ included are at the highest risk of being automated.
2. The Captchas with noise such as lines across the text are at a medium risk of a breach.
3. Observing the different captchas and its history we can find that there is always a space separating the letters in a captcha which makes these captchas vulnerable for machines to break them.
4. If the intensity of the noise is less than the actual text and if not converging on the text, the noise can be removed by thresholding or binarizing 
5. Captchas with Images or a combination of Images and text with varying intensity of noises is an efficient way to be used in applications and would be difficult for machines to learn the pattern.

Note: Refer the slides and program for complete understanding of the implementation.
