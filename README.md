# Spring-Boot-Microservices-Basic-Project1
A basic Spring Boot Microservices project that includes User-Service, Contact-Service, Eureka-Server and API-Gateway.
  - User MicroService includes User Details like Id, Name.
  - Contact MicroService includes Contact details like contactId, email, phone.
  - Eureke Server is a service registry that helps manage microservices in a distributed system and allows services to register themselves and discover other services
     without hardcoding their addresses., here used to register User and Contact Microservices.
  - API gateway acts as an intermediary between clients and backend services, managing and routing API requests, here routing User and Contact Microservices.

Steps to open the Project in IntelliJ:
  - Download and Install 7-Zip: Go to the 7-Zip website and download the latest version. Install 7-Zip on your computer.
  - Download all the splitted raw files from Github for each Microservice one by one.
  - Open 7-Zip Application and select all the splitted 7-Zip files(1-4/1-5) for each Microservice and click on the Extract Icon to Extract the file.
  - Extract all the raw files for each Microservice one by one.
  - Once all the 4 Microservices are extracted, use IntelliJ to open each Microservice and Run Maven-clean & install.
  - Run the Eureka-Server Microservice first, followed by User, Contact and API Gateway Microservices.
  - Open Edge Browser and hit the URIs to fetch the User and Contact details.

URIs in EDGE to see User and Contact Results:
  - for Eureka Server Microservice: http://localhost:8761/
  - for User Microservice: http://localhost:9001/user/{UserId}, http://localhost:9001/user/1213
  - for Contact Microservice: http://localhost:9002/contact/user/{UserId}, http://localhost:9002/contact/user/1214
  - Through API Gateway Microservice:
     - for User Microservice: http://localhost:8999/user/{UserId}, http://localhost:8999/user/1211
     - for Contact Microservice: http://localhost:8999/contact/user/{UserID}, http://localhost:8999/contact/user/1211
  - Check Eureka Server Microservice if the User, Contact and API Gateway Microservices are up and running.

Reference: (https://www.youtube.com/watch?v=_PQd6aZ-ANk)
