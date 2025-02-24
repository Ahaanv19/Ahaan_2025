---
layout: post
title: Big Idea 4 Blog
permalink: /BI/
toc: true
comments: true
---

# Big Idea 4: The Internet - Networking Stack in a GitHub Pages → AWS EC2 Interaction, Personal Features

## Introduction
When a frontend hosted on GitHub Pages interacts with a backend Python web application on AWS EC2, multiple layers of the networking stack come into play. This blog explores these layers in depth and provides code snippets demonstrating how the interaction works. Additionally, we will analyze how this project aligns with AP Computer Science Principles (AP CSP) Big Ideas and the College Board’s Create Performance Task (CPT) requirements.

## Connection to AP CSP Big Ideas
### **Big Idea 1: Creative Development**
- The development of this project required designing and implementing a structured approach to handling frontend-backend communication.
- Using GitHub Pages and AWS EC2 demonstrates creativity in deploying a scalable system.
- The dynamic genre table allows users to add, edit, and delete sections, showcasing problem-solving skills in designing a functional feature.

### **Big Idea 2: Data**
- The genre table stores and retrieves user-generated data using a database.
- Data persistence is handled via an SQL-based backend.
- JSON responses facilitate seamless data transmission between frontend and backend.

#### **Example: Fetching Data from the Database**
```python
@app.route("/sections", methods=["GET"])
def get_sections():
    sections = Section.query.all()
    return jsonify([{ "id": sec.id, "name": sec.name, "theme": sec.theme } for sec in sections])
```

### **Big Idea 3: Algorithms and Programming**
- The frontend dynamically generates and manipulates the table using JavaScript.
- The backend follows structured API endpoints to handle CRUD operations.

#### **Example: Dynamic JavaScript Table Rendering**
```javascript
fetch("https://api.example.com/sections")
    .then(response => response.json())
    .then(data => {
        const tableBody = document.getElementById("sectionsTable");
        tableBody.innerHTML = "";
        data.forEach(section => {
            const row = `<tr>
                <td>${section.id}</td>
                <td>${section.name}</td>
                <td>${section.theme || ''}</td>
                <td>
                    <button onclick="editSection(${section.id}, '${section.name}', '${section.theme || ''}')">Edit</button>
                    <button onclick="deleteSection(${section.id})">Delete</button>
                </td>
            </tr>`;
            tableBody.innerHTML += row;
        });
    })
    .catch(error => console.error("Error:", error));
```

### **Big Idea 4: Computer Systems and Networks**
- This project showcases how HTTP, TCP, and IP protocols enable communication between the frontend and backend.
- The networking stack ensures secure and efficient data transfer.
- Hosting the backend on AWS EC2 demonstrates cloud computing concepts.

#### **Example: Flask API Running on AWS EC2**
```python
if __name__ == "__main__":
    app.run(host="0.0.0.0", port=8103)
```

### **Big Idea 5: Impact of Computing**
- The ability to dynamically manage genres enhances user experience.
- Ensuring secure communication using HTTPS prevents unauthorized data access.

## Connection to CPT Requirements
1. **Program Purpose & Function:**
   - The purpose is to enable users to manage and categorize book genres efficiently.
   - Users can perform CRUD operations via a user-friendly interface.

2. **Data Usage:**
   - Data is stored in an SQL database and retrieved using REST API calls.
   - JSON formatting ensures data consistency and readability.

3. **Algorithms & Abstraction:**
   - The project abstracts complex backend processes by exposing RESTful API endpoints.
   - JavaScript event handlers dynamically update the UI based on user input.

4. **Testing & Debugging:**
   - Unit tests verify backend functionality.
   - Console logs and network monitoring debug frontend issues.

#### **Example: Backend Testing Using Pytest**
```python
def test_get_sections():
    response = app.test_client().get("/sections")
    assert response.status_code == 200
```


## Connection to AP CSP Create Performance Task (CPT)
### Code Development Process
The Create Performance Task (CPT) requires students to develop a program that:
- Performs data collection, storage, and manipulation.
- Utilizes an abstraction to simplify a complex process.
- Implements an algorithm that achieves a specific outcome.

### How This Project Meets CPT Requirements  

| Requirement              | Implementation                            |
|-------------------------|-----------------------------------------|
| **Data Collection**      | Stores section data in an SQL database |
| **Procedural Abstraction** | Uses functions like `get_sections()` to handle data retrieval |
| **Algorithm Implementation** | Implements authentication using JWT tokens |


#### Example: Creating and Using a JWT Token for Authentication
```python
@app.route("/login", methods=["POST"])
def login():
    username = request.json.get("username")
    password = request.json.get("password")
    if username == "admin" and password == "password123":
        access_token = create_access_token(identity=username)
        return jsonify(access_token=access_token)
    return jsonify({"error": "Invalid credentials"}), 401
```



## Tools in Use
| **Tool** | **Purpose** |
|----------|------------|
| **Docker** | Containerizes the backend for consistent deployment. |
| **Nginx** | Manages HTTP traffic and serves as a reverse proxy. |
| **Certbot** | Enables HTTPS for secure communication. |
| **SQL Database** | Stores section data for retrieval and updates. |
| **JavaScript Fetch API** | Enables frontend-to-backend communication. |
| **Flask API** | Handles backend logic and database interactions. |



## Conclusion
This project exemplifies AP CSP Big Ideas in action, demonstrating real-world applications of computer systems and networks. By integrating frontend-backend communication, database management, and secure networking principles, this project serves as a model CPT submission aligning with AP CSP’s key learning objectives.
