# Docker Compose - WordPress + MySQL

This project demonstrates how to deploy a **multi-container application using Docker Compose**.

The application consists of:

- WordPress
- MySQL 8.0
- Docker Compose Network
- Docker Named Volumes

WordPress connects to MySQL using the Docker Compose service name.

---

## Architecture

```text
                    Browser
                       |
                       | Port 8080
                       v
              +----------------+
              |   WordPress    |
              |   Container    |
              |     wPRES      |
              +-------+--------+
                      |
                      | db:3306
                      v
              +----------------+
              |     MySQL      |
              |     8.0        |
              |  wordpres-db   |
              +-------+--------+
                      |
                      v
                 db_data
              Named Volume


-----------------------------------------------------------

Technologies Used
Docker
Docker Compose
WordPress
MySQL 8.0
Docker Networking
Docker Named Volumes
