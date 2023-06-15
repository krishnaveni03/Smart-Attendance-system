# Smart-Attendance-system
METHODOLOGY
 

1.	Data Collection: 
In this step, images of student faces are captured and stored in a database. This can be done using a camera or webcam, and the images should be captured under different lighting conditions and angles to ensure accuracy in recognition.

2.	Face Detection:
 OpenCV is used to detect faces in the captured images. This is done using the Haar Cascade classifier, which is trained to detect faces based on specific features such as the presence of eyes, nose, and mouth.

3.	Face Alignment:
 After detecting the face, the next step is to align it to a standard position. This is done to reduce variations in pose and facial expression that can affect the accuracy of recognition. The PIL (Python Imaging Library) package is used to perform this task.

4.	Feature Extraction: 
Once the face is aligned, the next step is to extract the features that will be used for recognition. LBPH (Local Binary Patterns Histograms) is a face recognition algorithm that is used to extract features from the aligned face images. This algorithm calculates a histogram of local binary patterns in different regions of the face, which are then combined to create a feature vector.

5.	Face Recognition: 
The final step is to match the extracted features to those in the database. This is done by calculating the similarity between the feature vectors using a distance metric such as Euclidean distance or cosine similarity. If the similarity score is above a certain threshold, the system will consider the face a match and record attendance.

  6. Attendance storing:
	Once attendance is recorded the system stores the information in an Excel sheet.The openpyxl package is used to create and modify the excel sheets for each day and records the attendance of each student in a row along with the date and time

TECHNOLOGY
PYTHON:
1.tkinter
2.openCV
3.csv,numpy,pandas,date and time
