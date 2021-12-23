# Face_Swapping_Application
### Used OpenCV and DLIB to develop a Face Swapping Application. The application extracts a face of a human-being from a given image using a pre-trained model. Obtained the pre-trained model from a Github Repository and it can be downloaded [here](https://github.com/tzutalin/dlib-android/raw/master/data/shape_predictor_68_face_landmarks.dat). Hence, the whole application can be summarized as follows:
- Given a source image and a destination image, the application has to replace the face of the destination image with the face of the source image and vice-versa.
## Steps taken to solve this problem were as follows:
- Downloaded a pre-trained model that enabled the extraction of a face from an image
- A function was then created that enabled extracting the index
- The source and destination images were then loaded from the internet
- The images then had to be converted into a numpy array so that the model could be applied to them
- The images also had to be converted to greyscale for better results
- DLIB was then used to load the face detector and face landmarks predictor
- The process of triangulation was then performed on the images so that the faces could be cut out
- Empty masks were then created for the images
- Swapping the face of the destination image with the face of the source image, and vice-versa was the next step
- Seamless cone was then used to adjust the color scheme

# Results
### Source Image:
<img width="305" alt="Screen Shot 2021-12-23 at 10 05 45 PM" src="https://user-images.githubusercontent.com/18570056/147287250-af75f512-0e7d-4250-9cee-2b165ea9b5fd.png">

### Destination Image: 
<img width="302" alt="Screen Shot 2021-12-23 at 10 07 35 PM" src="https://user-images.githubusercontent.com/18570056/147287380-054ccc8d-5f73-4e94-a75b-c69b97741cb0.png">

### Source Image Swapped With The Destination Image:
<img width="304" alt="Screen Shot 2021-12-23 at 10 09 11 PM" src="https://user-images.githubusercontent.com/18570056/147287492-e165e858-3aee-4149-92c5-fe758efd6d29.png">
