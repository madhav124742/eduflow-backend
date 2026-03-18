# EduFlow Pro Portal

A simple and modern Student ERP web application built with Spring Boot and Vanilla HTML/CSS/JS.

## Features

- **Student Management:** Add new students and view them in a clean table with search functionality.
- **Dashboard Overview:** See total students and top 3 performers at a glance.
- **Attendance Tracking:** Mark students as present or absent and track their percentage.
- **Marks & Grading:** Input marks for 5 subjects, automatically calculates total, percentage, grade, and pass/fail result.
- **Performance Insights:** View student progress on their detail card, with visual indicators distinguishing Pass and Fail results.
- **Dark/Light Theme:** Built with a modern dark theme and an easy toggle for light mode.

## Tech Stack

- **Backend:** Java 17, Spring Boot 3
- **Data Storage:** In-Memory (cleared on restart)
- **Frontend:** Vanilla HTML5, CSS3, JavaScript (Fetch API)

## Prerequisites

- Java Development Kit (JDK) 17 or higher
- Maven (optional if you have an IDE, but required for command line build)
- An internet connection when running for the first time (to download Maven dependencies and load google font 'Inter')

## Project Structure

```
c:\Users\madha\Desktop\JAVA\New folder\
 │
 ├── pom.xml                                   # Maven dependencies
 ├── src/main/java/com/eduflow/                # Backend Source Code
 │    ├── EduFlowApplication.java              # Main Application Class
 │    ├── controller/StudentController.java    # REST API endpoints
 │    ├── service/StudentService.java          # Business Logic & Data Store
 │    └── model/                               # Data Models (Student, Attendance, Marks)
 │
 └── src/main/resources/
      ├── application.properties                 # App configuration
      └── static/                                # Frontend Assets (Served automatically)
           ├── index.html                        # Main UI layout
           ├── css/style.css                     # Custom Styling (Dark/Light themes)
           └── js/app.js                         # Application Logic (API calls & DOM)
```

## How to Run Locally

### Option 1: Using an IDE (Recommended)
1. Open up **IntelliJ IDEA**, **Eclipse**, or **VS Code**.
2. Select **Open** or **Import Project** and choose the `c:\Users\madha\Desktop\JAVA\New folder` directory.
3. Wait for Maven to download the dependencies.
4. Locate the `EduFlowApplication.java` file in `src/main/java/com/eduflow/`.
5. Right-click the file and select **Run 'EduFlowApplication.main()'**.
6. Open your browser and go to: [http://localhost:8080](http://localhost:8080)

### Option 2: Using Terminal / Command Prompt
1. Open a terminal or command prompt inside `c:\Users\madha\Desktop\JAVA\New folder`.
2. Run the following command to compile and start the app:
   ```bash
   mvn spring-boot:run
   ```
3. Open your browser and go to: [http://localhost:8080](http://localhost:8080)

## Usage Guide
1. By default, 3 dummy students are loaded with some sample attendance and marks data.
2. Go to the **Students** tab on the left sidebar.
3. Use the **+ Add Student** button to register a new student.
4. Click **View** on any student to open their Detail Card / Report Card.
5. In the Report Card, use the buttons to **Mark Attendance** or **Add Marks**.
6. Switch back to the **Dashboard** to see the Top Performers based on the latest entered percentages.
7. Click the **☀️ Toggle Theme** button to switch between light and dark modes.
