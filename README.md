## Setup

In a promp or Terminal window, type:  
 
```shell
conda install --file requirements.txt 
```
I'm using Anaconda as a package manager.

This will help you in installing all the libraries required for the project. Bear in mind, at the time of development, Python 3.6.8 and OpenCV 4.1.1.26, Keras 2.2.4 and tensorflow 1.12.0 was used.

## Process

- Run `1-set-hand-histogram.py` to set the hand histogram for creating gestures. 
- Once you get a good histogram, save it in the same directory as the python files.
- Add gestures and label them using OpenCV which uses webcam feed. by running `2-create-gestures.py` and stores them in a database file.
- Add different variations to the captured gestures by flipping all the images by using `3-rotate-images.py`.
- Run `4-load-images.py` to split all the captured gestures into training, validation and test set. 
- To view all the gestures, run `5-display-gestures.py`.
- Train the model using Keras by running `6-cnn-model-train.py`.
- Run `7-final.py`. This will open up the gesture recognition window which will use your webcam to interpret the trained Sign Language gestures.  

## Note

This is my Final Year Project (FYP) for my Computer Engineering degree.