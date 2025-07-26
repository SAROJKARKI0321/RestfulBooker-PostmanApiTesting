# 📬 Postman Collection – Restful Booker API

This repository contains a **Postman collection** to test the public **Restful Booker API**, which simulates a hotel booking system.  
You can use this collection to run automated or manual CRUD operations for learning, testing, or demonstration purposes.

---

## 📁 Files Included

- `restful-booker.postman_collection.json` – The main Postman collection with all endpoints.
- *(Optional)* `restful-booker_environment.json` – Pre-configured environment variables for base URL, tokens, etc.

---

## 🔗 API Reference

API Documentation: [https://restful-booker.herokuapp.com/apidoc/index.html](https://restful-booker.herokuapp.com/apidoc/index.html)

---

## 🚀 How to Use This Collection

### 1. Import into Postman

- Open Postman
- Click **Import**
- Choose the file: `restful-booker.postman_collection.json`

### 2. Set Up Environment (optional)

If you’re using variables:

- Import `restful-booker_environment.json` (if available)
- Select it from the environment dropdown in Postman

### 3. Run Requests

- Use the **collection runner** or run individual requests manually.
- Explore all CRUD operations:  
  - `GET /booking`  
  - `POST /booking`  
  - `PUT /booking/:id`  
  - `DELETE /booking/:id`  

---

## ✅ Requirements

- Postman v10+  
- Internet connection (API is hosted online)

---

## 📌 Notes

⚠️ This API is **public** and resets frequently. Don't expect data to persist.  
🔄 You may need to regenerate authentication tokens before using protected routes.

---

## 📃 License

This collection is for learning, testing, and demo purposes only.
