# Emitter Backend API
This is a Spring Boot application that provides a RESTful API for fetching questions based on difficulty and language ID, and checking if an answer is correct.
Swagger link = http://localhost:8080/swagger-ui/index.html#
## Prerequisites
- Java 8 or higher
- Maven
- IntelliJ IDEA 2023.3.2 or any other IDE that supports Spring Boot

## Setup
1. Clone the repository to your local machine.
2. Open the project in your IDE.
3. Update the `application.properties` file with your database credentials.

## Running the Application
1. Navigate to the root directory of the project in your terminal.
2. Run the command `mvn spring-boot:run` to start the application.

## API Usage
The application runs on `http://localhost:8080` by default. Replace `localhost` with your IP address if you're accessing the API from a different machine.

### Fetch Questions
To fetch questions based on difficulty and language ID, send a GET request to `/api/questions` with the `difficulty` and `languageId` parameters.
Example: `http://localhost:8080/api/questions?difficulty=1&languageId=1`

### Check Answer
To check if an answer is correct, send a GET request to `/api/questions/check-answer` with the `languageId`, `questionId`, and `selectedOption` parameters.
Example: `http://localhost:8080/api/questions/check-answer?languageId=1&questionId=1&selectedOption=A`

## Contributing
Please read [CONTRIBUTING.md](./CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
## License
This project is licensed under the MIT License - see the [LICENSE.md](./LICENSE.md) file for details
