# CODSOFT Number Game

A simple console-based number-guessing game written in Java as part of the CodSoft internship exercises. The player tries to guess a randomly chosen integer and receives feedback whether their guess is too high or too low. A score starts at 50 and is reduced with each incorrect guess.

## Features

- Console menu to start or exit the game
- Random target number (1–99 as implemented)
- Hints after each wrong guess (too high / too low)
- Simple scoring that decreases with wrong guesses

## Requirements

- Java Development Kit (JDK) 8 or later is recommended for compiling and running Java programs.

Note: The implementation uses Random.nextInt(1, 100) which requires Java 17+. If you use an older JDK, either upgrade to Java 17+ or modify the code to use `random.nextInt(100) + 1` instead.

## Files

- NumberGame.java — main source file containing `NumberGameApplication` with the `main` method and game logic.

## How to build and run

1. Clone or download this repository and open a terminal.
2. Change into the project directory:

```bash
cd CODSOFT_Number_Game
```

3. Compile the Java file:

```bash
javac NumberGame.java
```

4. Run the application:

```bash
java NumberGameApplication
```

If you prefer to compile from the repository root without changing directories, compile with the relative path and run with the classpath set to the project directory:

```bash
javac CODSOFT_Number_Game/NumberGame.java
java -cp CODSOFT_Number_Game NumberGameApplication
```

## Gameplay

- Choose `1` to start the game, or `2` to exit.
- The program prompts: "Guess the number:". Enter an integer and press Enter.
- If your guess is too high or too low, you'll be prompted to guess again until you find the correct number.
- When you guess correctly, the correct number and your score are shown.

## Example session

```
||---------------------------||
|| CAN YOU GUESS THE NUMBER? ||
||---------------------------||
1. Start the game
2. Exit the game
Enter your choice (1/2): 1

||--------------------------------||
|| GAME STARTED. GUESS THE NUMBER ||
||--------------------------------||

Guess the number: 50
Your number is too high

Guess again: 25
Your number is too low

Guess again: 37

Congratulations. Your guess is right the number is: 37
Your Score is: 48 out of 50
```

(Note: Exact score behavior depends on the implementation details in the code.)

## Known issues and suggestions

- Random API: `random.nextInt(1, 100)` (two-argument form) requires Java 17+. Consider replacing with `random.nextInt(100) + 1` for Java 8+ compatibility.
- Input validation: The program assumes numeric input; entering non-integer input will throw an exception. Add try/catch and input validation to handle invalid input gracefully.
- Scoring logic: The score update currently uses `score = points --;` which is confusing and may not behave as intended. Consider tracking attempts and computing score from attempts (for example: `score = Math.max(0, 50 - attempts)`).
- Resource handling: Multiple Scanner instances are created; prefer creating one Scanner and reusing it or closing it properly before program exit.

## Improvements you can make

- Add JUnit unit tests for the game logic (separate pure logic from I/O to make testing easier).
- Add a maximum number of attempts or difficulty levels.
- Persist high scores to a file.
- Add a simple GUI (Swing/JavaFX) for a more user-friendly interface.

## Author

Subhadip (@subhadip2004999)

---

If you'd like, I can also:
- update the source code to be compatible with Java 8,
- add input validation, or
- create a build script (Gradle/Maven) and a runnable JAR.
