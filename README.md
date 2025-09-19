# Real-Time Chat Application

A scalable real-time chat application that enables users to send and receive messages instantly.  
Built with **Spring Boot (WebSockets)** and **SQL database** to ensure persistence, reliability, and scalability.


## Features
- Real-time messaging between multiple clients using WebSockets  
- User authentication (login/register)  
- Message persistence in SQL database  
- Reliable delivery with publish–subscribe model  
- Scalable architecture with message queue integration  


##  Tech Stack
- **Backend:** Java, Spring Boot, WebSockets  
- **Database:** MySQL / PostgreSQL  
- **Architecture:** Message Queue + SQL DB for persistence  
- **Build Tool:** Maven / Gradle  


## System Design

```mermaid
graph TD
A[Client 1] -- WebSocket --> B[Spring Boot Server]
C[Client 2] -- WebSocket --> B
B --> D[(SQL DB)]
B --> E[Message Queue]
E --> B
