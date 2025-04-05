# 📚 Rest Assured API Testing - API-WORKBOOK

This project demonstrates how to perform **API testing using Rest Assured and TestNG** against a public read-only REST API.

> 🚫 Note: This public API does **not support** POST/PUT/DELETE operations. Only GET methods will work.

---

## 🔗 API Under Test

**Base URL:**
https://fakerestapi.azurewebsites.net/api/v1


---

## ✅ What’s Covered

- Get All Books
- Get Book by ID
- Get Non-Existing Book by ID (Negative Scenario)

---

## 📁 Project Structure

RestAssuredBookAPI/ ├── src/ │ ├── com.base/ │ │ └── BaseTest.java │ ├── com.tests/ │ │ └── BookCRUDTest.java ├── config.properties ├── pom.xml └── README.md

yaml
Copy
Edit

---

## ⚙️ Technologies Used

- Java
- Maven
- Rest Assured
- TestNG

---

---

## 🧪 What We’re Testing

| Test Name               | Status    | Description                                      |
|------------------------|-----------|--------------------------------------------------|
| `testGetAllBooks()`     | ✅ Pass    | Retrieve all books                              |
| `testGetBookById()`     | ✅ Pass    | Get a book by valid ID                          |
| `testGetNonExistingBook()` | ✅ Pass | Check 404 for non-existent book ID             |

> ❗ POST/PUT/DELETE requests are **not supported** by this public API, and will result in `405`/`501` errors.

---

## 🚀 How to Run

1. 🔁 Clone this repository
2. 📂 Open it in **Eclipse** or **IntelliJ**
3. 🔨 Run `mvn clean install` or right-click → **Run as TestNG Suite**
4. 🔍 Results appear in your console or TestNG tab

> `config.properties` contains the correct URL:
```properties
base_url=https://fakerestapi.azurewebsites.net/api/v1







