```markdown
# AGENTS.md File Guidelines

These guidelines outline best practices for all development efforts within the AGENTS repository. Adherence to these principles is crucial for maintaining a maintainable, scalable, and reliable codebase.

## 1. DRY (Don't Repeat Yourself)

*   All logic, data models, and API definitions must be encapsulated within dedicated files and functions.
*   Avoid duplicating code.  If a functionality needs to be reused, create a reusable component or function.
*   Refactor code to eliminate redundant sections.
*   Use interfaces and abstract classes to define common contracts.

## 2. KISS (Keep It Simple, Stupid)

*   Strive for maximum simplicity in code design.
*   Prioritize readability and clarity.
*   Avoid unnecessary complexity.
*   Keep functions and classes focused on a single task.
*   Favor explicit over implicit.  State should be managed explicitly rather than relying on hidden assumptions.

## 3. SOLID Principles

*   **Single Responsibility Principle:** Each class should have one and only one reason to change.
*   **Open/Closed Principle:**  The system should be extensible without modifying the existing code.
*   **Liskov Substitution Principle:**  Subclasses must be substitutable for their base classes without altering the correctness of the program.
*   **Interface Segregation Principle:** Client code should not be forced to depend on implementation details.
*   **Dependency Inversion Principle:**  High-level modules (classes) should not depend on low-level modules (classes). Interfaces should govern interaction.

## 4. YAGNI (You Aren't Gonna Need It)

*   Implement only what is absolutely necessary for the current functionality.
*   Avoid adding features or code that is not currently required.
*   Focus on delivering value incrementally.
*   Don't over-engineer solutions.

## 5. Development Process & Code Quality

*   **Code Comments:**  Provide clear and concise comments explaining the *why* behind the code, not just the *what*.  Comments should be focused on algorithm, reasoning, and edge cases.
*   **Naming Conventions:**  Follow a consistent naming convention (e.g., camelCase, snake_case).
*   **Error Handling:** Implement robust error handling with informative error messages. Avoid exceptions where possible; use well-defined return values and error conditions.
*   **Testing:**  All development *must* be productive, requiring a minimum of 80% test coverage using established testing frameworks.  Tests should be designed to isolate and verify specific functionality.
*   **Code Formatting:**  Adhere to a consistent code formatting style (e.g., using a linter).
*   **Version Control:** Use Git for version control and adhere to established branching strategies.
*   **Code Review:** All code changes should be reviewed by another developer before merging.

## 6. File Structure & File Size

*   Each file should be no more than 180 lines of code.
*   Files should be organized logically.
*   Consider using a directory structure to reflect the module/component hierarchy.

## 7. Specific File Considerations

*   **`Agent.py`:**  Contains core agent logic, data models, and API definitions.  Should be well-documented and easily testable.
*   **`DataModel.py`:**  Defines the data structures used by the agents.
*   **`Network.py`:**  Implements the networking layer for communication between agents.
*   **`StateManagement.py`:**  Handles agent state management.
*   **`AgentService.py`:**  Contains service logic for interacting with other systems.
*   **`Configuration.py`:** Stores configuration data.

## 8. Testing Requirements

*   Unit tests should cover all significant functions and classes.
*   Integration tests should validate interactions between components.
*   End-to-end tests should simulate real-world scenarios.

## 9. Documentation

*   Provide brief README files for each file explaining its purpose and usage.

## 10. Automation

*   Utilize a continuous integration (CI) system to automate testing and build processes.

By adhering to these guidelines, the AGENTS repository will be a consistently high-quality and maintainable system.  Any deviation from these rules will be addressed and require discussion and revision.
```