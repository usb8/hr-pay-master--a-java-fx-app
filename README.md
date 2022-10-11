# HR Pay Master

HR Pay Master is a simple Java application for managing company staff, calculating salaries, and listing employees with long-term seniority. The project includes both a console-based version and a JavaFX GUI version.

## Features

- Manage staff information: name, email, year of starting work.
- Two staff types:
  - **Worker**: Main salary = product quantity × 10.
  - **Officer**: Main salary = fixed salary − days off × 100.
- Each employee receives a compensation of 100, increasing by 20 for each year of service.
- Add and list company employees.
- Calculate the total salary the company must pay each month.
- List employees with more than 10 years of service.
- JavaFX GUI for interactive usage.

## Project Structure

```
2_company/                # Console version (pure Java)
    Main.java
    Company.java
    Staff.java
    Worker.java
    Officer.java
    README.md
companyfx/                # JavaFX GUI version (Maven project)
    src/
        main/
            java/com/example/companyfx/
                MainApplication.java
                MainController.java
                Company.java
                Staff.java
                Worker.java
                Officer.java
            resources/com/example/companyfx/
                hello-view.fxml
    pom.xml
```

## Getting Started

### Console Version (`2_company`)

1. Open a terminal in the `2_company` directory.
2. Compile and run:
    ```sh
    javac Main.java
    java Main
    ```

### JavaFX Version (`companyfx`)

1. Ensure you have Java 16+ and Maven installed.
2. Open a terminal in the `companyfx` directory.
3. Run the application:
    ```sh
    mvn clean javafx:run
    ```
4. The GUI will display total salary and seniority information.

## Requirements

- Java 16 or higher
- Maven (for JavaFX version)

## Notes

- The console and JavaFX versions share similar logic but are implemented separately.
- The JavaFX version uses static variables to share data between the application and controller.

## License

This project is for educational purposes.