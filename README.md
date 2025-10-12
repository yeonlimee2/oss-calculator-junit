# Calculator — Maven + JUnit 5 (OSS Lecture 6)

A minimal Java project showing **Apache Maven** for build automation and **JUnit 5** for unit testing.

## Requirements
- Java 17+
- Maven 3.9+
- (Optional) VS Code + “Extension Pack for Java”

## Project Layout
- `src/main/java/...` application code  
- `src/test/java/...` test code  
- `pom.xml` Maven config

## Quick Start (CLI)
```bash
# compile sources
mvn compile

# run unit tests
mvn test

# package JAR into /target
mvn package

# clean build artifacts
mvn clean
```

## Test Report (HTML)
```bash
mvn surefire-report:report
# open target/site/surefire-report.html
```

## VS Code (Testing UI)
1. Open the folder in VS Code.  
2. Go to the **Testing** view (beaker icon) → **Run All Tests**.  
3. If tests don’t appear: `Ctrl+Shift+P` → **Java: Clean Java Language Server Workspace**.

## Troubleshooting
- Ensure package names match folders.
- Confirm JUnit 5 dependencies are in `pom.xml`.
- Java version in `pom.xml` matches your installed JDK.
