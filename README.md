Computer Vision (CV) plays a crucial role in various domains, with one significant application being the detection of facial expressions. Understanding facial expressions is fundamental in human communication, as they convey emotions and intentions. CV-based facial expression detection enables machines to interpret and respond to human emotions, facilitating more natural and intuitive human-computer interaction.
This Python script uses OpenCV for real-time facial expression detection using a trained model (facialemotionmodel.h5).
The script loads the trained model and defines a list of emotion labels corresponding to the expressions it can detect: "Angry", "Disgust", "Fear", "Happy", "Neutral", "Sad", "Surprise".

It initializes OpenCV's face detector using the Haar cascade classifier.
The extract_features function takes a frame (image) captured from the camera, detects faces, extracts the face region, and predicts the emotion using the model. It then draws a rectangle around the face and displays the predicted emotion label on the frame.
The main function captures frames from the camera in a loop, calls the extract_features function on each frame, and displays the resulting frame with emotion labels.
The script runs indefinitely until the user presses the 'q' key to quit.
