# Simple Web Quiz example on java

This project serves as a simple and demonstrative example for creating a web-based quiz application, utilizing Java Servlets and JSP (JavaServer Pages) technologies. Its primary purpose is to illustrate the structure and workflow required for an interactive question-and-answer application.

The application presents a set of questions to the user, records their answers, and, at the end, offers the option to restart the quiz. It is designed to be a starting point for more complex quiz-based applications.

## Key Features
* **Web Interface:** Uses JSP for displaying questions and managing user interactions.
* **Server-Side Logic (Servlets):** The `QuestionServlet` class handles the logic for displaying questions, processing answers, and navigating between pages.
* **Modular Structure:** The project is divided into logical packages (controller, entity, repository) for better organization.

## Project Structure
The project follows standard Maven conventions.
* **`QuestionServlet.java`**: The central control point of the application. It processes HTTP requests, manages quiz logic (next question, answer validation), and redirects to the appropriate JSP pages.
* **`Question.java`**: Defines the structure of a single question in the quiz. It should include attributes such as the question text, answer options, and the correct answer.
* **`DataBase.java`**: **This class is a *demonstrative* and *simplified* implementation to simulate question storage.** **For a real application, it is imperative to replace it with logic that accesses a persistent database (SQL, NoSQL, etc.) and implements an appropriate data management strategy (CRUD - Create, Read, Update, Delete).**
* **`index.jsp`**: The welcome or introductory page for the quiz.
* **`questionPage.jsp`**: The page where the user interacts with the questions. It likely contains forms for submitting answers.
* **`restart.jsp`**: The final page of the quiz, which might display a score or an end message and offers the option to restart.
* **`styles.css`**: The styling file for the visual appearance of the application.

## Requirements
* Java Development Kit (JDK) 8 or newer
* Apache Maven (for building the project)
* A Servlet API and JSP compatible application server (e.g., Apache Tomcat 8 or newer)
* Docker (optional, for containerized execution)

