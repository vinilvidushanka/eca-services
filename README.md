# ITS 2130 ECA Project Submission - Business Services

Polyrepo architecture with Git submodules, implemented with Spring Cloud and deployed on Google Cloud Platform.

## 1. Student Information

| Field | Value |
| :--- | :--- |
| **Module** | ITS 2130 Enterprise Cloud Application |
| **Program** | HDSE @ IJSE |
| **Student Name** | Vinil Vidushanka |
| **Student ID** | 2301692013 |
| **Submission Date** | 2026-03-31 |
| **Main Submission Repository** | https://github.com/vinilvidushanka/eca-services.git |

## 2. Project Overview

This repository contains the core business microservices for the **GoDrive** application.
* Each microservice is implemented using Spring Boot and Spring Cloud.
* Database requirements are met using both SQL and NoSQL solutions.
* All services are registered with the central Eureka discovery service.

## 3. Repository Structure (Polyrepo + Submodules)

### 3.1 Nested Submodules in Services

| Path | Repository | Purpose |
| :--- | :--- | :--- |
| Services/booking-service | https://github.com/vinilvidushanka/Booking-Service-GoDrive.git | Booking microservice |
| Services/customer-service | https://github.com/vinilvidushanka/Customer-Service-GoDrive.git | Customer microservice |
| Services/vehicle-service | https://github.com/vinilvidushanka/Vehicle-Service-GoDrive.git | Vehicle microservice |
| Services/config-repo | https://github.com/vinilvidushanka/GoDrive-Config-Repo.git | Externalized Configurations |

## 4. Spring Cloud Components Implemented

* Spring Cloud Config Client
* Spring Cloud Netflix Eureka Client

## 5. Database & Cloud Storage Requirements (Mandatory)

* **Relational Database**: MySQL/PostgreSQL for transactional data.
* **Non-Relational Database**: MongoDB for flexible data storage.
* **Cloud Storage**: Integrated with Google Cloud Storage Buckets for file persistence.

## 6. High Availability and Auto Scaling (Mandatory)

### 6.1 Microservice Auto Scaling

| Check | Value |
| :--- | :--- |
| Horizontal scaling supported | YES |
| Autoscaler configuration | YES |
| Instance group details | YES |

## 7. PM2 Process Management and Auto Restart (Mandatory)

All microservices are managed by PM2 to ensure high availability and automatic recovery as per the project guidelines.

### 7.1 PM2 Compliance Checklist

| Requirement | Status |
| :--- | :--- |
| Applications started and managed by PM2 | YES |
| Auto restart on failure | YES |
| PM2 starts on VM reboot | YES |

## 8. Screen Recording Submission (Mandatory)

* **Recording URL**: https://drive.google.com/file/d/12L4fkenJXVYBrzwBsfufipEPKwNqd9bQ/view?usp=sharing

## 9. How to Clone This Repository

```bash
git clone --recurse-submodules [https://github.com/vinilvidushanka/eca-services.git](https://github.com/vinilvidushanka/eca-services.git)
```
