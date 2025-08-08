# Alloy Wheel Visualizer App 🚗🛠️

A full-stack Android application that allows customers to visualize alloy wheels on their car by uploading an image and selecting compatible designs. Dealers can upload alloy designs and manage their stock. The app leverages ML for alloy overlay and includes role-based access, real-time data from MongoDb, Amazon S3 and Spring Boot as the backend.

Now available on Google Play (Closed Testing)

---

## 📱 Features

### For Customers:
- Upload side-view photo of car.
- Select car company and model.
- View list of dealers with compatible alloy designs.
- Visualize alloy designs overlaid on the uploaded car image using AI/ML model.
- Filter alloys by size or width.
- Secure login using phone number authentication.
  
### For Dealers:
- Register and log in via phone OTP.
- Upload alloy designs with metadata (size, width, compatibility, etc.).
- Manage stock and view customer interest.

---

## 🧠 ML Integration
- Trained a custom YOLO segmentation model to detect wheels in the car image.
- Overlay selected alloy design on detected wheel regions.
- Model served via Python backend or integrated into Android.

---

## 🛠️ Tech Stack

### 🔙 Backend (Spring Boot)
- Spring Boot + Spring Security (JWT-based authentication)
- MongoDB for data persistence
- AWS S3 for image storage
- REST APIs for all operations
- Role-based access control (Customer and Dealer)

### 📱 Frontend (Android)
- Jetpack Compose UI
- Coil + Retrofit + Coroutines
- Camera & File Picker integration
- Role-based navigation
- ML overlay visualization

---

## 🔒 Security
- JWT-based authentication system.
- Endpoints secured using role-based access.
- Dealers and customers have isolated access to respective features.

---

## 🔗 Repositories

- **Backend (Spring Boot)**: [GitHub - Alloy Visualizer Backend](  https://github.com/Krish-Virani/Personal-Project  )  
- **Frontend (Android)**: [GitHub - Alloy Visualizer Android App](  https://github.com/Krish-Virani/Personal-Project-Android  )

---

## 📱 App Screenshots

<p align="center">
  <img src="https://github.com/user-attachments/assets/d5787ea2-b8dd-4ea2-9454-6c6794dc5209" alt="Screen 1" width="250"/>
  <img src="https://github.com/user-attachments/assets/cc02f2ea-b13d-4f11-9585-b101dfa1f0a2" alt="Screen 2" width="250"/>
  <img src="https://github.com/user-attachments/assets/d522ef95-69b5-4082-9ee2-de6d006e2459" alt="Screen 3" width="250"/>
  <img src="https://github.com/user-attachments/assets/6b4c110a-a865-4d43-9fac-ec2181ceb2ab" alt="Screen 4" width="250"/>
  <img src="https://github.com/user-attachments/assets/b2563f0e-3a69-40cb-be38-dd296688210e" alt="Screen 5" width="250"/>
  <img src="https://github.com/user-attachments/assets/aa0cf498-8e21-4c94-b82c-5c461dc8c176" alt="Screen 6" width="250"/>
  <img src="https://github.com/user-attachments/assets/3bb03393-f416-4efd-801b-3fbb8e5b577d" alt="Screen 7" width="250"/>
</p>



