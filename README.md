# Lab 1: Egg Drop (C++ Edition)

## 🥚 Overview

This lab involves writing a C++ program that determines whether an egg will break when dropped from a building, based on the height of the fall and gravitational acceleration.

You will:
- Prompt the user to enter the height of a building in meters.
- Use physics to calculate the time it takes for the egg to fall.
- Determine if the egg will break based on that time.
- Display the result, matching the expected output format exactly.

---

## 📚 Background

To compute the time it takes for the egg to fall, use the following physics formula for free fall (ignoring air resistance): t = √(2h / g)

Where:
- `t` is the time in seconds,
- `h` is the height in meters,
- `g` is the gravitational constant (9.8 m/s²).

If the **time exceeds 2.00 seconds**, the egg will break.

---

## ✅ Program Requirements

- Prompt the user for the building height (in meters).
- Calculate fall time using the formula above.
- Print the time to exactly **2 decimal places**.
- If time > 2.00 seconds → print: `"The egg will break!"`
- If time ≤ 2.00 seconds → print: `"The egg will not break!"`
- Output should match the example exactly (formatting matters).

---

## 💡 Example Executions

```bash
Enter the height of the building in meters: 20
Time to fall: 2.02 seconds
The egg will break!
```
```bash
Enter the height of the building in meters: 5
Time to fall: 1.01 seconds
The egg will not break!
```

---

## 🧪 Grading Criteria (100 Points Total)

The majority of your score (**85 points**) will come from **program correctness**, meaning your program passes all required tests and behaves as specified. The remaining **15 points** will be awarded for **code style** and **comments**.

| Category                 | Description                                                     | Points |
|--------------------------|------------------------------------------------------------------|--------|
| **Correctness**          | Program compiles, runs, and passes all functional tests          | 85     |
| • Input Handling         | Proper prompt and reading of numeric input                       | 10     |
| • Fall Time Calculation  | Uses correct physics formula                                     | 20     |
| • Output Formatting      | Fall time printed with exactly **2 decimal places**              | 10     |
| • Conditional Logic      | Correct branching and message based on fall time                 | 15     |
| • Output Matching        | Matches sample output exactly (format, punctuation, spacing)     | 10     |
| • Edge Cases             | Handles values unexpected/invalid numeric values                 | 20     |
| **Code Style & Comments**| Proper indentation, naming, organization, and inline comments    | 15     |

> ✅ To earn full credit, make sure your program produces the correct result **and** is cleanly written with helpful comments.

## 🛠️ Compilation and Execution

To compile your code:

```bash
g++ main.cpp -o main
```
To run your program:

```bash
./main
```

🧵 Tips
- Use #include <cmath> for sqrt().
- Use std::fixed and std::setprecision(2) from <iomanip> for decimal formatting.
- Your code should adapt to any numeric input. The sample executions are a good place to start, but don't test ONLY those cases.
- Be sure your output formatting matches the sample exactly, including spacing and punctuation.


