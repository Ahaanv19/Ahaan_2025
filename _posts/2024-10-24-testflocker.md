---
layout: post
title: Personal Feature Database Blog
permalink: /BI/
toc: true
comments: true
---

</table>
<p1 style="font-size:70%; color: purple; font: bold 14px Open Sans;"> Final Exam Review Blogs Linked Here.  &#128513;</p1>
<table>
    <tr>
        <td><img src="{{site.baseurl}}/images/notebook.png" height="60" title="Home" alt=""></td>
        <td><a href="{{site.baseurl}}/retrospective/">Personal Retrospective</a></td>
        <td><a href="{{site.baseurl}}/exam/">Final Exam Homepage</a></td>
        <td><a href="{{site.baseurl}}/dm/">Performance Task Demo Video & N@tM</a></td>
        <td><a href="{{site.baseurl}}/mcq/">MCQ Blog</a></td>   
        <td><a href="{{site.baseurl}}/BI/">Personal Feature Blog</a></td> 
    </tr>

</table>

  <a href="https://github.com/Ahaanv19/LitConnect/issues/10" class="button-link">Feedback</a>



# Personal Full Stack Feature: College Board Performance Task Blog

## Introduction
When a frontend hosted on GitHub Pages interacts with a backend Python web application on AWS EC2, multiple layers of the networking stack come into play. This blog explores these layers in depth and provides code snippets demonstrating how the interaction works. Additionally, we will analyze how this features aligns with AP Computer Science Principles (AP CSP) Big Ideas and the College Board’s Create Performance Task (CPT) requirements.

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
fetch("https://litconnect.stu.nighthawkcodingsociety.com//sections")
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

## **Detailed Connection to CPT Requirements**

### **1. Program Purpose & Function**
- The program allows users to categorize and manage book genres efficiently.
- CRUD operations enable users to create, read, update, and delete genres.
- The interface provides an interactive experience while maintaining data integrity.
- The use of RESTful APIs allows scalable and modular architecture, aligning with CPT’s requirement for well-structured and purposeful development.

### **2. Data Usage**
- Data is persistently stored in an SQL database, ensuring availability across sessions.
- JSON-based REST API responses facilitate structured and machine-readable data.
- Query optimization ensures performance efficiency, addressing CPT’s emphasis on effective data handling.
- Error handling mechanisms ensure data consistency, preventing corruption due to failed operations.

#### **Example: Backend Testing Using Pytest**
```python
def test_get_sections():
    response = app.test_client().get("/sections")
    assert response.status_code == 200
```

### **3. Algorithms & Abstraction**
- The backend leverages RESTful API abstractions to handle user requests efficiently.
- The frontend dynamically processes and renders data to the UI, simplifying the user experience.
- JWT authentication abstracts security measures, ensuring secure access to user data.
- The program meets CPT’s requirement for implementing abstraction in code through modular function design.

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

### **4. Testing & Debugging**
- Unit tests validate API functionality, ensuring consistent behavior.
- Logging mechanisms help debug errors and improve system reliability.
- Automated test scripts enable regression testing to maintain performance integrity.
- These practices align with CPT’s emphasis on testing and debugging throughout development.


### How This Project Meets CPT Requirements  

| Requirement              | Implementation                            |
|-------------------------|-----------------------------------------|
| **Data Collection**      | Stores section data in an SQL database |
| **Procedural Abstraction** | Uses functions like `get_sections()` to handle data retrieval |
| **Algorithm Implementation** | Implements authentication using JWT tokens |


## How My Feature Meets CPT Requirements

### **1. Instructions for Input**
My project allows user input through an interactive web interface. Users can:
- Add, edit, and delete genres dynamically using buttons in the frontend.
- Submit HTTP requests via JavaScript `fetch()` to interact with the backend API.
- The Flask API processes user input and modifies the SQL database accordingly.

#### **Example: Handling User Input in JavaScript**
```javascript
function addSection() {
    const name = document.getElementById("sectionName").value;
    fetch("https://api.example.com/sections", {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        body: JSON.stringify({ name: name })
    })
    .then(response => response.json())
    .then(data => console.log("Added section:", data))
    .catch(error => console.error("Error:", error));
}
```

### **2. Use of Lists or Collections**
The project uses a database table to manage genres. Data is stored and retrieved using SQL queries and represented as a JSON collection in the backend.

#### **Example: Retrieving Data from SQL and Converting to JSON**
```python
@app.route("/sections", methods=["GET"])
def get_sections():
    sections = Section.query.all()
    return jsonify([{ "id": sec.id, "name": sec.name, "theme": sec.theme } for sec in sections])
```

### **3. Custom Procedure with Parameters**
A key procedure in my backend is `get_sections()`, which retrieves genre data. It demonstrates abstraction by handling SQL queries and formatting responses.

#### **Example: Defining and Using a Procedure in Python**
```python
def get_sections_data():
    return Section.query.all()

@app.route("/sections", methods=["GET"])
def get_sections():
    sections = get_sections_data()
    return jsonify([{ "id": sec.id, "name": sec.name, "theme": sec.theme } for sec in sections])
```

### **4. Algorithm with Sequencing, Selection, and Iteration**
The program includes algorithms that:
- Sequence: Execute SQL queries and return JSON responses.
- Selection: Use conditional logic to handle user authentication.
- Iteration: Loop through database records to generate API responses.

#### **Example: Using Conditional Logic in User Authentication**
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

### **5. Calls to Student-Developed Procedure**
The frontend calls backend functions via API requests, which then execute the student-developed procedures.

#### **Example: Fetching Sections from the Backend**
```javascript
fetch("https://api.example.com/sections")
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(error => console.error("Error:", error));
```

### **6. Output Based on Input and Functionality**
The project provides textual and visual output through:
- Console logs for debugging.
- Dynamic table updates displaying stored data.
- JSON responses from the API.

#### **Example: Displaying API Data in a Table**
```javascript
function displaySections(data) {
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
}
```

This detailed breakdown demonstrates how my feature aligns with the College Board’s CPT requirements while integrating fundamental computing principles from AP CSP.




## Full Stack Connection to AP CSP Big Idea 4:
In AP Computer Science Principles (CSP), Big Idea 4 focuses on the importance of the internet and networking in computing systems. Understanding the layers of the networking stack is essential for students to comprehend how data moves across the internet, from end-users (clients) to servers, and how systems communicate in a distributed environment. This blog provides a practical understanding of these layers in a real-world scenario, highlighting the importance of secure and efficient data transmission in web development.

### **Big Idea 4: Computer Systems and Networks**
- This project showcases how HTTP, TCP, and IP protocols enable communication between the frontend and backend.
- The networking stack ensures secure and efficient data transfer.
- Hosting the backend on AWS EC2 demonstrates cloud computing concepts.


## 1. HTTP/DNS (Application Layer)

### Frontend (GitHub Pages):
- The frontend makes HTTP(S) requests using JavaScript’s `fetch` API.
- The domain name of the AWS EC2 backend is resolved via DNS.
- The request includes method, headers, and optional body (e.g., JSON payload for CRUD operations).

#### Example: Making an HTTP GET Request in JavaScript
```javascript
fetch("https://api.example.com/sections", {
    method: "GET",
    headers: {
        "Content-Type": "application/json"
    }
})
.then(response => response.json())
.then(data => console.log(data))
.catch(error => console.error("Error:", error));
```

### Backend (AWS EC2 with Docker):
- The backend processes the request inside a Docker container.
- Handles CRUD operations on an SQL database.
- Constructs an HTTP response.
- Uses Certbot for HTTPS security.

#### Example: Python Flask API Handling a Request
```python
from flask import Flask, request, jsonify

app = Flask(__name__)

@app.route("/data", methods=["GET"])
def get_data():
    return jsonify({"message": "Hello from AWS EC2"})

if __name__ == "__main__":
    app.run(host="0.0.0.0", port=8103)
```

## 2. TCP/UDP (Transport Layer)
### Request:
- HTTP(S) requests are transmitted using TCP.
- Nginx manages TCP traffic and routes it to the correct container.
- TCP handshake ensures a reliable connection.

### Response:
- The server sends an HTTP response over the same TCP connection.
- TCP guarantees in-order and complete delivery.

#### Example: Configuring Nginx for Reverse Proxy
```nginx
server {
    listen 80;
    server_name api.example.com;
    location / {
        proxy_pass http://localhost:8103;
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
    }
}
```

## 3. IP (Network Layer)
### Request:
- TCP segments are encapsulated into IP packets.
- Packets are routed to AWS EC2 via routers.

### Response:
- The AWS EC2 server sends packets back to the client.
- AWS handles routing and load balancing.

#### Example: Checking Network Traffic with `tcpdump`
```sh
sudo tcpdump -i eth0 port 80 or port 443
```

## 4. Physical Layer
### Request & Response:
- IP packets are converted into physical signals (Ethernet, Wi-Fi, fiber optics).
- Signals travel through routers, cables, and wireless networks.


#### Tools in Use

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
