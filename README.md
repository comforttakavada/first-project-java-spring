This project is a Spring Boot, It demonstrates the basics of web development using the Spring Framework, specifically the MVC (Model-View-Controller)

Project Configuration
This project uses:
Build Tool: Maven
Language:Java
Framework:Spring Boot


Features

Controller Functionality (`HelloController.java`)
The application includes a controller that handles three types of HTTP requests:

GET /`**: Returns a raw text response: `"Hello Vistula, in my first Spring controller."`
GET /hello: Returns a raw text response: `"Hello from Spring!"`
GET /greeting: Uses an MVC approach. It accepts an optional `name` parameter (default: "World"), binds it to the model, and renders the `greeting.html` template.

 2. View Layer (`greeting.html`)
The view layer utilizes Thymeleaf for dynamic content rendering:
Dynamic Greeting: Displays a personalized message based on the URL parameter (`/greeting?name=YourName`).
Static Content: Includes a placeholder image (`vistula.png`) sourced from the `src/main/resources/static` directory.

How to Run
Import: Ensure the project is imported into your IDE as a Maven project.
Dependencies: If the IDE shows errors, right-click the project, select Maven, and then Reload project.
Execute: Run the main application class.
Access:
http://localhost:8080/` for the root message.
http://localhost:8080/greeting?name=Vistula` to see the rendered HTML template with the Vistula logo.
 Project Structure
src/main/java/`: Contains the HelloController.
src/main/resources/templates/`: Contains greeting.html (Thymeleaf template).
src/main/resources/static/`: contain vistula.png .
