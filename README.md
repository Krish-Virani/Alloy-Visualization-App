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
