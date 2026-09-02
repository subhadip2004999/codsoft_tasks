# CODSOFT_TASKS

Internship at CodSoft.in in the Java Programming.

This repository contains small Java projects completed during an internship at CodSoft. The projects are intended as learning exercises and demonstrate basic Java concepts such as console I/O, control flow, object-oriented programming, and simple data processing.

## Repository language

- Java (100%)

## Projects in this repository

- CODSOFT_ATM_Interface — A console-based ATM simulator with PIN authentication, balance inquiry, deposits, and withdrawals. See `CODSOFT_ATM_Interface/README.md` for details and run instructions.
- CODSOFT_Number_Game — A number-guessing game implemented in Java. See the `CODSOFT_Number_Game` folder for source files and instructions.
- CODSOFT_Student_Grade_Calculator — A simple grade calculator that reads student marks and computes totals, averages, and grades. See `CODSOFT_Student_Grade_Calculator/README.md`.

## How to build and run

Each project in this repository is a small console application with one or more `.java` files. The general steps to compile and run any project are:

1. Ensure you have Java (JDK) 8 or later installed.
2. Open a terminal and change into the project folder, for example:

   cd CODSOFT_ATM_Interface

3. Compile the Java files in that folder:

   javac *.java

4. Run the main class. Replace `<MainClass>` with the actual class name containing `public static void main(String[] args)`:

   java <MainClass>

Note: Some projects may declare a package at the top of their .java files. If so, compile/run from the repository root and include the package path when running the class (or use an IDE).

## Project-specific notes

- If you are unsure which class has the `main` method, inspect the Java files for `public static void main` or open the subfolder README.md files which include usage examples.
- For convenience and reproducible builds, you can add a simple `build.gradle` or `pom.xml` later to compile and package these projects.

## Contributing

This repository is primarily for learning. If you'd like to contribute improvements, consider:

- Adding input validation and error handling where missing
- Adding unit tests (JUnit) for logic-heavy classes
- Adding a build system (Maven/Gradle) and a runnable JAR
- Providing more examples and sample inputs in each project README

To contribute: fork the repo, create a branch, make changes, and open a pull request.

## License

No license file is included. By default, all rights are reserved by the author. If you want to allow others to use or contribute, consider adding an open-source license such as the MIT License.

## Author

Subhadip (GitHub: @subhadip2004999)

---

If you want a more detailed top-level README (badges, CI, how to run each project with exact main class names, or a table of contents), tell me which details you want and I will update the file.