Here are some basic and commonly used Gradle commands when working with the `./gradlew` wrapper in a Spring Boot project:

---

### **Build Commands**
1. **Build the Project**
   ```bash
   ./gradlew build
   ```
   - Compiles the code, runs the tests, and builds the application JAR file in the `build/libs/` directory.

2. **Clean the Project**
   ```bash
   ./gradlew clean
   ```
   - Deletes all build artifacts (e.g., compiled classes, JAR files).

3. **Rebuild the Project**
   ```bash
   ./gradlew clean build
   ```
   - Cleans the project and then builds it again.

---

### **Running the Application**
1. **Run the Application**
   ```bash
   ./gradlew bootRun
   ```
   - Starts your Spring Boot application.

---

### **Testing**
1. **Run Tests**
   ```bash
   ./gradlew test
   ```
   - Executes all the unit tests in your project.

2. **Run a Specific Test**
   ```bash
   ./gradlew test --tests "com.example.demo.SomeTest"
   ```
   - Runs a specific test class or method.

---

### **Dependency Management**
1. **Show Dependencies**
   ```bash
   ./gradlew dependencies
   ```
   - Lists all dependencies, including transitive ones.

2. **Show Dependency Tree**
   ```bash
   ./gradlew dependencies --configuration runtimeClasspath
   ```
   - Displays the dependency tree for the runtime classpath.

---

### **Other Useful Commands**
1. **Check the Gradle Version**
   ```bash
   ./gradlew --version
   ```
   - Displays the Gradle version and environment information.

2. **View Available Tasks**
   ```bash
   ./gradlew tasks
   ```
   - Lists all available tasks in the project.

3. **Show Build Information**
   ```bash
   ./gradlew buildEnvironment
   ```
   - Displays the build environment, including JVM and dependency information.

---

### **Debugging and Logs**
1. **Run with Debug Logs**
   ```bash
   ./gradlew build --debug
   ```
   - Provides detailed debugging information.

2. **Run with Stacktrace**
   ```bash
   ./gradlew build --stacktrace
   ```
   - Prints the full stack trace if an error occurs.

3. **Run with Info Level Logging**
   ```bash
   ./gradlew build --info
   ```
   - Shows more detailed logging than the default output.

---

### **Creating a JAR File**
1. **Build a Runnable JAR**
   ```bash
   ./gradlew bootJar
   ```
   - Creates an executable JAR file for your Spring Boot application in the `build/libs/` directory.

2. **Build a Plain JAR**
   ```bash
   ./gradlew jar
   ```
   - Creates a regular JAR file (not executable).

---

### **Updating Gradle Wrapper**
1. **Update Gradle Wrapper Version**
   ```bash
   ./gradlew wrapper --gradle-version <version>
   ```
   - Updates the Gradle wrapper to a specific version (e.g., `8.3`):
     ```bash
     ./gradlew wrapper --gradle-version 8.3
     ```

---

### **Run Custom Tasks**
1. **Run a Specific Task**
   ```bash
   ./gradlew <task-name>
   ```
   - Replace `<task-name>` with the task you want to execute (e.g., `test`, `bootRun`).

2. **Run Multiple Tasks**
   ```bash
   ./gradlew clean build test
   ```
   - Runs multiple tasks in sequence.

---

These commands should cover most of your needs when using `./gradlew`. Let me know if you want details on any specific command!