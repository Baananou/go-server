# Simple Web Server with Form Handling

This is a simple Go application that sets up a web server capable of handling static files, processing form submissions, and responding to basic HTTP requests. The application uses the standard `net/http` package to create the server and define handlers for different routes.

## Features

1. **Static File Serving:** The server serves static files (e.g., HTML, CSS, JavaScript) from the `./static` directory. Accessing the root URL ("/") will serve the static files located in this directory.

2. **Form Handling:** The server handles HTTP POST requests to the "/form" endpoint. When a POST request is made, the server extracts form data from the request body and responds with a success message along with the values of the submitted "name" and "address" fields.

3. **Hello Endpoint:** The server responds with a "hello!" message to GET requests made to the "/hello" endpoint.

## How to Use

1. **Clone the Repository:** Clone this repository to your local machine.

2. **Navigate to the Directory:** Open a terminal and navigate to the directory where you cloned the repository.

3. **Run the Application:** Execute the following command to run the application:

   ```bash
   go run main.go

4. **Access the Web Pages:**

- Open your web browser and navigate to [http://localhost:8080](http://localhost:8080) to access the static files served from the `./static` directory.
- To submit a form, visit [http://localhost:8080/form](http://localhost:8080/form). Enter your name and address in the provided fields and submit the form to see the submitted data displayed.
- Access [http://localhost:8080/hello](http://localhost:8080/hello) to receive a "hello!" message.
  
**Stopping the Server:**

To stop the server, press `Ctrl+C` in the terminal where the server is running.

**Requirements:**

- Go (Golang) must be installed on your machine to run this application.

**Disclaimer:**

This application is intended for educational and illustrative purposes only. It demonstrates basic web server functionalities and may not be suitable for production use without further enhancements and security considerations.
