---
layout: post
title:  Big Idea 4 Blog
permalink: /BI/
toc: true
comments: true
---
# Big Idea 4: The Internet - Networking Stack in a GitHub Pages → AWS EC2 Interaction

## Introduction
When a frontend hosted on GitHub Pages interacts with a backend Python web application on AWS EC2, multiple layers of the networking stack come into play. This blog will explore these layers in depth and provide code snippets demonstrating how the interaction works.

## Connection to AP CSP Big Idea 4:
In AP Computer Science Principles (CSP), Big Idea 4 focuses on the importance of the internet and networking in computing systems. Understanding the layers of the networking stack is essential for students to comprehend how data moves across the internet, from end-users (clients) to servers, and how systems communicate in a distributed environment. This blog provides a practical understanding of these layers in a real-world scenario, highlighting the importance of secure and efficient data transmission in web development.

## 1. HTTP/DNS (Application Layer)

### Frontend (GitHub Pages):
- The frontend makes HTTP(S) requests using JavaScript’s `fetch` API.
- The domain name of the AWS EC2 backend is resolved via DNS.
- The request includes method, headers, and optional body (e.g., JSON payload for CRUD operations).

#### Example: Making an HTTP GET Request in JavaScript
```javascript
fetch("https://api.example.com/data", {
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
    app.run(host="0.0.0.0", port=5000)
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
        proxy_pass http://localhost:5000;
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

## Tools in Use

| **Tool**              | **Purpose**                                                                                                                                                               |
|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Docker**            | Containerizes the backend Python application, ensuring consistent deployment across environments. It simplifies the setup process and allows for isolated, reproducible environments. |
| **Nginx**             | Acts as a reverse proxy, handling incoming HTTP(S) requests. It routes traffic to the appropriate Docker container, balancing the load and ensuring efficient request handling.  |
| **Certbot**           | A free, automated tool for managing SSL/TLS certificates. It ensures secure HTTPS connections by obtaining and renewing certificates, maintaining a secure communication channel between frontend and backend. |
| **SQL Database**      | Stores and retrieves data for CRUD operations. The backend interacts with the database to fetch, update, or delete data, typically using SQL queries.                        |
| **JavaScript Fetch API** | Allows the frontend to make asynchronous HTTP requests to the backend. It simplifies communication between the browser and the server, enabling dynamic data fetching and interaction. |
| **Python Flask API**  | A lightweight web framework used to build the backend. Flask handles HTTP requests, processes data, interacts with the database, and sends responses back to the client.         |


## Conclusion
Understanding the networking stack from GitHub Pages to AWS EC2 is crucial for deploying scalable web applications. Each layer—Application, Transport, Network, and Physical—plays a role in ensuring secure and efficient communication between the frontend and backend.





