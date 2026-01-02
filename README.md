# 2026 Flutter Engineer Test

![Bitroot Org](https://avatars.githubusercontent.com/u/63720760?s=100&v=4)

![Internship - Flutter](https://img.shields.io/badge/Internship-Flutter-blue)
![Android Studio](https://img.shields.io/badge/Android-Studio-green?style=flat-square&logo=flutter)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github)

---

## 📋 What We Expect

- Proficient knowledge of the **Dart** programming language and the **Flutter** framework
- Understanding of **Backend REST APIs** (to communicate with team members)
- Ability to manage **Material Design**, including database handling and scaling applications to handle load changes
- Knowledge of **accessibility** and **security compliance**
- Experience with **version control**, such as Git
- **Native app experience** will be an add-on (Optional)

---

## 📱 Project Overview

### Create a Payment Management App using Local Database

**Core Requirements:**

- Create UI based on the given screenshots (You need to create the auth UI)
- Make models as per design UI and bind with UI
- Following points need to be considered while making the designs:

1. Use **Slivers** as much as possible
2. Make user experience **smooth**
3. Page navigation should be **Shimmer-based**
4. Search should be in **full screen**
5. ListView should be **animated** based on user gestures

---

## 🛠️ Frameworks to be Used

- **MVP / MVVM / Others** (Architecture Pattern)
- **Repository Architecture** (Optional)
- **Bloc Pattern / Provider / GetX** (any works)

---

## 🔐 Authentication Implementation

Implement **Login** and **Register** functionality using the APIs provided below.

### Register API
```http
POST https://api.rapaap.com/api/v1/mobile/registerUser
Content-Type: application/json

{
  "mobile": 8454883226,
  "email": "c2905y@gmail.com",
  "password": "123456",
  "name": "Chandan Yadav"
}
```

### Login API
```http
POST https://api.rapsap.com/api/v1/mobile/loginUser
Content-Type: application/json

{
  "username": "rapsap@gmail.com",
  "password": "123456"
}
```

---

## 🧩 Authentication Implementation Guidelines

- Add **Login** and **Register** screens
- UI design is open but must include:
  - Clean **Material UI**
  - Smooth transitions
  - **Shimmer / Loader** during API calls
- Existing screens, navigation, and logic **must not break**

---

## ✅ Validation Requirements

### Register Screen

- **Name**: Required
- **Mobile**:
  - Exactly 10 digits
  - Numbers only
- **Email**:
  - Valid email format
- **Password**:
  - Minimum 6 characters
- **Confirm Password**:
  - Must match password

### Login Screen

- **Username / Email**: Required
- **Password**: Required

> **Note:** All validations must be handled **before making API calls**.  
> API error messages must be displayed clearly using **Snackbar / Dialog**.

---

## 💾 Login State Persistence (Mandatory)

After successful login, use **one** of the following to store session data:

- `SharedPreferences`
- `GetX Storage` (preferred if using GetX)

### Store at least:

- `isLoggedIn` flag
- User identifier (email / username / id if available)

---

## 🚀 App Launch Behavior

On app launch:

- If user is **logged in** → Navigate directly to **Payment Dashboard**
- If user is **not logged in** → Show **Login Screen**
- Avoid unnecessary re-login API calls once session exists

---

## ⭐ Additional Points

Bonus points for:

- Using **local database**
- Simplified **3rd party integrations** enhancing the app's functionalities and keeping the app size minimal

---

## 📸 UI Reference

![App UI Reference](https://user-images.githubusercontent.com/9571732/184913399-858128bd-3f58-41b8-abb3-0afa5f9d1afc.png)

---

## 📝 Submission Guidelines

- Ensure clean, readable, and well-documented code
- Follow Flutter best practices
- Include a proper `README.md` with setup instructions
- Push your code to a GitHub repository
- Share the repository link for evaluation

---

**Good luck! 🚀**

---

*Prepared by Bitroot Org.*
