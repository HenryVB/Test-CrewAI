# Test-CrewAI

Test-CrewAI is a sample Java RESTful API web service project that allows to manage users data. It provides endpoints to create, read and update.

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the Application](#running-the-application)
- [API Endpoints](#api-endpoints)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## About the Project

Test-CrewAI is designed to be a simple and scalable service for managing users data. It uses Spring Boot to provide a robust and easy-to-use interface for interacting with user data. The API supports basic CRUD operations and is designed to be easily extendable for additional features.

## Features

- Create a new user
- Retrieve a list of all users
- Retrieve a specific user by its ID
- Update data of an existing user

## Getting Started

Follow these instructions to set up and run the Test-CrewAI project on your local machine.

### Prerequisites

List any prerequisites for your project, such as:

- [Java JDK 17]
- [Maven]
- [MySQL 8.X]

### Installation

Provide a step-by-step series of examples that tell how to get a development environment running:

1. Clone the repository:
   git clone https://github.com/yourusername/projectname.git

2. Navigate to the project directory:
	cd Test-CrewAI

3. Install the dependencies using maven:
	mvn install

4. Configure the database in application.properties :
	spring.datasource.url=jdbc:mysql://localhost:3306/<yourdatabasename>
	spring.datasource.username=<your database user name>
	spring.datasource.password=<your database user password>
	spring.jpa.hibernate.ddl-auto=update
	spring.jpa.show-sql=true
	
### Running the Application

To run the Test-CrewAI project locally:
1. Start the application:
	mvn spring-boot:run

2. The API will be accessible at http://localhost:8080


### API Endpoints
- GET /api/books
	Retrieves a list of all books.
- GET /api/books/{id}
	Retrieves a specific book by ID.
- POST /api/books
	Creates a new book entry.
- PUT /api/books/{id}
	Updates an existing book's details.

### Project Structure
	Test-CrewAI/
	│
	├── src/
	│   ├── main/
	│   │   ├── java/
	│   │   │   └── com/
	│   │   │       └── example/
	│   │   │       	└── demo/	
	│   │   │           	├── DemoApplication.java
	│   │   │           	├── controller/
	│   │   │           	│   └── UserController.java
	│   │   │           	├── model/
	│   │   │           	│   └── User.java
	│   │   │           	└── repository/
	│   │   │               	└── UserRepository.java
	│   │   └── resources/
	│   │       ├── application.properties
	│   └── test/
	│       └── java/
	├── target/
	├── pom.xml
	└── README.md

## Contributing
Contributions are welcome! If you want to contribute to the BookStore API, follow these steps:

1. Fork the repository.
2. Create a feature branch (Example: git checkout -b feature/AmazingFeature).
3. Commit your changes (Example: git commit -m 'Add some AmazingFeature').
4. Push to the branch (Example: git push origin feature/AmazingFeature).
5. Open a Pull Request.

## License
TBD
## Contact

- Henry Valdivia - hvaldivia@soaint.com
- Project Link: https://github.com/HenryVB/Test-CrewAI


