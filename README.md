# Employee Attendance Management System (EAMS)

![image](https://github.com/user-attachments/assets/8f717713-06a3-490c-8a80-da19b2dce587)

![image](https://github.com/user-attachments/assets/64bd328b-d7a2-47e3-84bd-98ff395fda99)

![image](https://github.com/user-attachments/assets/ebc3425a-a8d9-4bf7-86e5-3f7ad1886d9f)

![image](https://github.com/user-attachments/assets/d800a36b-5861-43cf-ae6d-839407dfceaa)

![image](https://github.com/user-attachments/assets/c3ed15b4-a625-4469-8525-213f337da712)

![image](https://github.com/user-attachments/assets/46b6d7b3-eaa9-455d-94aa-11e37ae6e4ce)

![image](https://github.com/user-attachments/assets/b650b02a-1e35-418d-859c-88be470ff8e4)






## Overview

In today’s fast-paced corporate environment, efficient employee attendance management is essential for productivity and accurate administrative records. Traditional methods of attendance tracking, which rely on manual input or outdated systems, are prone to errors and inefficiencies. 

To address this, **Employee Attendance Management System (EAMS)** introduces an innovative solution that integrates **Internet of Things (IoT)** technologies, specifically leveraging **Raspberry Pi**, **Facial Recognition**, and **Deep Learning** to automate attendance tracking, improve accuracy, and streamline processes.

### Key Features
- **Image Capture**: Employees are photographed using a **Raspberry Pi Camera Module**, with images sent to the backend via a **Flask** application.
- **Image Processing**: The backend, powered by **Django**, processes these images and verifies attendance through facial recognition.
- **Facial Recognition**: Deep learning algorithms are used to identify employees based on facial recognition technology, ensuring accurate identification.
- **Attendance Recording**: Attendance data including check-in and check-out times is stored securely in the database.
- **Real-time Feedback**: **Buzzer** and **Speaker** provide instant feedback on attendance status (e.g., "Check-in Successful" or "Access Denied").
- **Dataset Management**: New employees can be added to the recognition dataset. If an unknown person is detected, their photo is captured along with their time and date information.
- **Work Time Monitoring**: Employees can view their work hours and daily routines through a **Next.js**-based frontend interface.

## Technologies Used
- **Raspberry Pi** with Camera Module
- **Flask** (Web Framework for Image Transmission)
- **Django** (Backend and Image Processing)
- **Deep Learning Algorithms** for Facial Recognition (using libraries like OpenCV and TensorFlow)
- **Next.js** (Frontend for Work Time and Routine Monitoring)
- **Buzzer** and **Speaker** (For real-time feedback)

## Project Architecture
1. **Image Capture**: 
   - Raspberry Pi Camera captures images of employees.
   - Flask application sends video feed to Django backend.
   
2. **Image Processing**: 
   - Django backend processes the captured image to verify employee presence.
   
3. **Facial Recognition**: 
   - Deep learning models are applied to recognize employee faces.
   - Matches are compared to the stored dataset for verification.
   
4. **Attendance Recording**: 
   - Verified attendance is stored, including check-in and check-out times.
   
5. **Feedback**: 
   - The system provides immediate feedback through a buzzer and speaker.
   
6. **Dataset Management**: 
   - Employees can be added to the system for recognition.
   - If an unknown face is detected, it is logged with additional information such as date and time.

7. **Work Time and Routine Monitoring**:
   - Employees can track their attendance and work hours via a web interface built with **Next.js**.

## Installation and Setup

### Prerequisites
- Raspberry Pi with **Raspberry Pi OS** installed
- **Python** 3.x installed
- **Flask** and **Django** installed
- **TensorFlow** and **OpenCV** for facial recognition
- **Node.js** and **Next.js** for the frontend

### Steps:
1. **Set up Raspberry Pi**:
   - Connect the **Raspberry Pi Camera Module** and ensure it is working.
   - Install necessary dependencies for Flask and Raspberry Pi integration.

2. **Backend Setup**:
   - Clone this repository and install the required Python libraries for Django, Flask, OpenCV, and TensorFlow.
   - Configure the Django backend for image processing and facial recognition.
   - Set up a database to store attendance data and employee details.

3. **Frontend Setup**:
   - Install **Node.js** and **Next.js**.
   - Set up the **Next.js** app to display employee work hours and attendance records.

4. **Facial Recognition Dataset**:
   - Add employee photos to the dataset for recognition.
   - The system will automatically store new employees when their faces are captured.

5. **Run the System**:
   - Start the Flask application to stream video from the Raspberry Pi camera.
   - Launch the Django backend to handle image processing and facial recognition.
   - Access the frontend via the Next.js application to monitor employee work times.

## Usage
1. **Employee Check-in/Check-out**:
   - When an employee approaches the system, their face is captured.
   - The system verifies the face and records their attendance, providing real-time feedback via the buzzer and speaker.

2. **Monitoring Attendance**:
   - Administrators can view employee attendance logs and work hours via the frontend application.

3. **Dataset Management**:
   - New employees can be added to the dataset through the admin panel.
   - If an unknown face is detected, their photo, along with date and time, is stored in the database for future reference.

## Future Enhancements
- Integrate additional IoT devices for better security and accuracy.
- Improve facial recognition models for even more accurate identification.
- Add features for remote access and monitoring of attendance data.

## Contributing
Feel free to contribute to this project by submitting pull requests or reporting any issues you encounter. Your contributions are always welcome!

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


