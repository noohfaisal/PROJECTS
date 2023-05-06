## Real-Time Face Cartoonification using OpenCV

This project demonstrates real-time face mask detection using OpenCV and Haar Cascades. The program uses a Haar Cascade Classifier to detect faces in each frame captured from a video feed. Once the face is detected, a mask is applied to the face region using a PNG image of a cartoon charecter. The masked image is then overlaid onto the original frame using bitwise-and. Finally, the output video is saved to a file named "output.avi".

### Installation

This project requires Python 3 and the following libraries:

- OpenCV (cv2)
- NumPy

You can install the required libraries using pip by running:

```
pip install opencv-python numpy
```

### Usage

To run the program, open the `face_mask_detection.ipynb` notebook file in Jupyter Notebook or any other compatible environment. Then, execute all the cells in the notebook. The program will start capturing video from the default camera (0) and display the output in a window named "Face Video". The output video will also be saved to a file named "output.avi" in the same directory as the notebook. To stop the program, press the 'q' key.

### Credits

This project is based on the following resources:

- [Real-time Face Mask Detection with Python, OpenCV, and MobileNet](https://www.pyimagesearch.com/2020/05/04/covid-19-face-mask-detector-with-opencv-keras-tensorflow-and-deep-learning/)
- [OpenCV documentation](https://opencv.org/)
- [NumPy documentation](https://numpy.org/)
