# Face-Recognition

  > The Face-Recognition Software is done using the [face_recognition](https://pypi.org/project/face_recognition/) library which requires [dlib](http://dlib.net), the C++ based machine learning and deep learning module.

## Installation  
  - The Software is written in Python 3.6
  - All the required modules are in the requirement text file   
  `pip install requirement.txt`
  - or Execute the following **Command** to install the modules.   
  `pip install pickle numpy Pillow Click tox flake8 dlib==19.7.0 sklearn face_recognition_models opencv-contrib-python`
  
## Working Procedure  
  - Upload the face data (Images) in **Folders** at the `Data/Train` Path. The Folder Names will be the labels of the Person in the images.  
  - Run `Train.py` for training the classifier which uses [KNN](https://scikit-learn.org/stable/modules/neighbors.html) (K- Nearest Neighbors Algorithm).
  - The Classifier is saved in `Model/` directory in `.clf` format.
  - By running `Video_Capture.py`, the video starts to stream from the choosen camera and labels the faces in the live stream.
  - If it finds an unknown face, it takes a snap and store it in the `\Noobie` directory.  
  
## Conclusion
> The Face_Recognition Software can be used for many applications. Personally in use it for **Attendence System Based on Face Recognition**, for getting staff attendance. It can also be used as **Security** purpose.  
