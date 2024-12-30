---

# Attendance Management System Using Face Recognition

## Summary

This **Attendance Management System** tracks who is present by automatically using facial recognition technology. It is made with Python and uses tools like OpenCV to detect and recognize faces, ensuring accuracy, security, and efficiency. The system is great for schools, workplaces, and events because it provides real-time attendance logging and reporting.

---

## Important Parts

- **Facial Recognition**: Can authenticate users through webcam.
- **Automated Attendance**: Immediately records attendance and stores it in a database.
- **Graphical Reports**: Shows attendance trends with charts.
- **User-Friendly GUI**: An easy interface for smooth interaction.
- **Database Integration**: Maintains safe attendance records and user information.
- **Manual Attendance**: Option Allows fallback for unrecognized faces.
---

## Technologies Used

- **OpenCV**: Detect and recognize faces.

- **NumPy & Pandas**: Data processing and handling.
- **Pillow**: Image resizing and manipulation.
- **Matplotlib**: Graphics data visualization.
- **Dlib**: Facial landmark detection.
- **Tkinter**: Graphical User Interface.
- **MySQL**: A database that keeps records safe.
- **PyCharm**: IDE for development and debugging.
---

## Here's a Complete Guide of How It Works

1. **Enrollment**: Users register their name, ID, and facial images.

   

   
   **Run the AMS_Run.py file**: It shows an interface like this. Now enter the enrollmont number and name in the following.




  
   ![Interface of the FAMS](https://github.com/user-attachments/assets/e733c3e3-7745-44d7-8168-198cc201be83)



   
   **Click on Take Images**: It takes several images in grayscale to train the model.



  
   ![Taking Images of the Student](https://github.com/user-attachments/assets/5a981da8-7546-4af9-811d-0e28e5385fee)


   


2. **Model Training**: Facial data is applied to train the recognition model.

   

   **Click on train images**: It will train the model with tthe several pictures that were taken before.

   

   
   ![Training the model](https://github.com/user-attachments/assets/c6a10f6e-e4e9-4cae-8002-33e831e7fd5b)

   

   

   
3. **Automatic Attendance Marking**: The system recognizes faces automatically and starts marking attendance on its own.



   * To give automatic atttendance click on automatic attendance ,then it will open another window
  


   * Enter the sectiion or subject details in the box and click on fill button
  


    ![Attendance Marked](https://github.com/user-attachments/assets/ba0f08cd-4673-4f40-9666-a34be3b4092e)



   * **Note**:**The attendance is filled** will show after capturing your face
  



   * It identifies the face and checks the database for the face base on the image trained.
  


   * Once it identifies , then the attendance is marked 
   

   ![Taking Attendance based on the Trained Model](https://github.com/user-attachments/assets/2cbb33b9-b61a-4866-85e4-142ae7c7fbb7)




   



   

4. **Manual Attendance**: Users can take attendance manually if required.

   

   **To do this**: follow the following steps :
   
    1.click on manual attendance and enter the details i.e., subject name 

   
   
    2. Then enter your Details such as Enrollment Number and name and then  click on enter data and then click on convert to csv

   

   ![Manual Attendance](https://github.com/user-attachments/assets/2e10ef6e-d20b-455a-88b9-186c11ffd92a)


   

   ![Manual Attendance(1)](https://github.com/user-attachments/assets/2e2001b4-4e8f-496d-954a-27968e28d30a)



5. **Check the Registered Students** : we can check the students who are registered on the system through their face data


   * To check this we have to go to check registered students and click it , it will redirect us to another window
  
     
   * There it will ask for the name and password , enter it accordingly and click login
  
     
     ![Entering username and password for checking registered faces](https://github.com/user-attachments/assets/f71334de-7de5-4e5d-b405-d7f25a2dabe8)


   * Then we can see all the students who have registered their faces at what time and exact details
  
     ![List Of Registered Faces and their details](https://github.com/user-attachments/assets/f976eade-daab-467b-aea7-ad5649b27b4a)



   * **Note**: The list of students who have not registered their faces or who gave their attendance manually will not be shown here in the list 



6. **To check the attendance complete details** : To check complete details, open StudentDetails.csv file from the StudentDetails Folder


---

## Installation and Setup

1. **Clone the Repository**:  
   ```bash
   git clone https://github.com/Sreekar529/Face-Recognition-Attendance-System.git
   cd Attendance-Management-System-using-Face-Recognition
   ```

2. **Install Dependencies**:  
   ```bash
   pip install -r requirements.txt
   ```

3. **Setup MySQL Database**:  
   - Create a database:  
     ```sql
     CREATE DATABASE attendance_system;
     ```  
   - Update `db_connector.py` with your database credentials.

4. **Run the App**:  
   Execute `AMS_Run.py` to start the system.

---

## Uses

- **Schools**: Automatically tracks student attendance.  
- **Corporate Offices**: Monitors employee attendance efficiently.  
- **Events**: Tracks attendee participation.  
- **Access Control**: Enhances security with face-based entry systems.

---

## Future Improvement

- Mobile app integration.  
- Improved recognition in diverse lighting conditions.  
- Support for multiple camera feeds.

---

## License

Licensed under the MIT License. See `LICENSE` for more details.

---

This format enhances readability while keeping the content intact. Let me know if you'd like further adjustments!
