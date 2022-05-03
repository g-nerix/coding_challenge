# coding_challenge
## Note: 
I am an amature in this field, I have previously not taken any coures in AI/ML, I do stuff because these things Interuige me. Please forgive me I do some thing wrong here.

## Approach (use CNN+LSTM (Convolutional Neural Network + Long Short Term Memory Deep learning Model)):
Seeing the dataset provided, it was clear that standard CNN won't do the work here since we can only extract features from the video, which won't be sufficient here since we are given a time-varying dataset. We would have to use something different. 
Upon reading several articles and looking through some previously published papers, I figured out we can use CNN + LSTM in a hybrid manner.

## Why it is the most appropriate solution here?
 - We already have several pretty good models which can extract landmarks from the face, and from here, we can feed these points to another model to classify them into different emotions.
 - Since we have fewer data points to train our model, the training and testing process would be orders of magnitude faster than a trivial approach. (THIS IS THE USP OF THIS APPROACH)
 - I find this approach to be efficient and well-suited for this kind of work.

## Now let's talk about some numbers:
I planned on using mediapipe library to get landmarks from on the dataset. It returns a list of 468 3-D points on the face. This is far less than 1280X720 (921,600) points in the original dataset

# I was not able to give enough time to this project and thereby this in incomplete
