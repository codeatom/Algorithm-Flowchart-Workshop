![Lexicon Logo](https://lexicongruppen.se/media/wi5hphtd/lexicon-logo.svg)

# Workshop: Algorithm and Flowchart

For each question in this workshop, you must complete **two** things:

1.  **Write the pseudocode**
2.  **Draw the flowchart** using either
    - **Option 1:** Draw.io (recommended) → export image → upload to
      your repository → link it in this file
    - **Option 2 (optional):** Write a Mermaid flowchart directly in
      Markdown
    - **Option 3 (optional):** Any other valid method

👉 **IMPORTANT:** At the **bottom of each question**, add the
following sections:

### ✔ Pseudocode

### ✔ Flowchart

---

## 1. Check Even or Odd Number

Design an algorithm and flowchart that take a number as input and
determine whether it is even or odd.

### ✔ Pseudocode

```text
START
    INPUT number
    IF number % 2 == 0 THEN
        PRINT Even
    ELSE
        PRINT Odd
    ENDIF
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> I[/Get input N/]
    I --> B{N % 2 == 0 ?}
    B -->|Yes| C[/Print Even/]
    B -->|No| D[/Print Odd/]
    C --> E([End])
    D --> E([End])
```

---

## 2. Calculate Total and Average Marks

Write the algorithm and draw the flowchart for a program that inputs
marks for 3 subjects, calculates the total and average, and displays
both.

### ✔ Pseudocode

```text
START

    INPUT marks1
    INPUT marks2
    INPUT marks3

total = marks1 + marks2 + marks3
average = total / 3

DISPLAY total
DISPLAY average

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]) --> B[/INPUT marks1/]
    B --> C[/INPUT marks2/]
    C --> D[/INPUT marks3/]
    D --> E[total = marks1 + marks2 + marks3]
    E --> F[average = total / 3]
    F --> G[/DISPLAY total/]
    G --> H[/DISPLAY average/]
    H --> I([END])

```

---

## 3. Display Multiplication Table

Create an algorithm and flowchart that input a number and display its
multiplication table from 1 to 10 using a loop.

### ✔ Pseudocode

```text
START

INPUT number

FOR i = 1 TO 10
    result = number × i
    DISPLAY number, " × ", i, " = ", result
END FOR

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]) --> B[/INPUT number/]
    B --> C[i = 1]
    C --> D{Is i = 10?}
    D -- Yes --> E[result = number × i]
    E --> F[/DISPLAY result/]
    F --> G[i = i + 1]
    G --> D
    D -- No --> H([END])
```

---

## 4. Positive, Negative, or Zero Check

Write the algorithm and flowchart to input a number and display whether
it is positive, negative, or zero.

### ✔ Pseudocode

```text
START

INPUT number

IF number > 0 THEN
    DISPLAY "Positive"
ELSE IF number < 0 THEN
    DISPLAY "Negative"
ELSE
    DISPLAY "Zero"
END IF

END

```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Input number]
    B --> C{Is number > 0?}
    C -->|Yes| D[Display Positive]
    C -->|No| E{Is number < 0?}
    E -->|Yes| F[Display Negative]
    E -->|No| G[Display Zero]
    D --> H([End])
    F --> H
    G --> H
```
---

## 5. Simple Interest Calculator

Create an algorithm and flowchart for a program that calculates simple
interest using the formula:

**SI = (P × R × T) / 100**

- **P = Principal** → original amount of money
- **R = Rate of Interest** → percentage per year
- **T = Time** → number of years

### ✔ Pseudocode

```text
BEGIN

    INPUT P
    INPUT R
    INPUT T

    SI = (P × R × T) / 100

    OUTPUT SI

END

```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input Principal P/]
    B --> C[/Input Rate of Interest R/]
    C --> D[/Input Time T/]
    D --> E[SI = P * R * T / 100]
    E --> F[/Display SI/]
    F --> G([End])
```

---

## 6. Average Temperature Calculation

Write the algorithm and draw the flowchart for a program that takes the
temperature of 7 days, finds the average temperature, and displays it.

### ✔ Pseudocode

```text
START

SET total = 0

FOR day = 1 TO 7
    INPUT temperature
    total = total + temperature
END FOR

SET average = total / 7

DISPLAY average

END

```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Set total = 0]
    B --> C[Set days = 1]
    C --> D[Input temperature]
    D --> E[total = total + temperature]
    E --> F[days = days + 1]
    F --> G{days <= 7?}
    G -- Yes --> D
    G -- No --> H[Calculate average = total / 7]
    H --> I[Display average]
    I --> J([End])

```

---

## 7. Calculate Area of a Rectangle

Create an algorithm and flowchart to input length and width, calculate
the area (**Area = Length × Width**), and display the result.

### ✔ Pseudocode

```text
BEGIN

    INPUT Length
    INPUT Width

    Area = Length × Width

    DISPLAY Area

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[/Input Length/]
    B --> C[/Input Width/]
    C --> D[Area = Length × Width]
    D --> E[/Display Area/]
    E --> F([End])
```

---

## 8. Determine Pass or Fail

Write the algorithm and draw the flowchart for a program that takes a
student's average marks and displays **"Pass"** if average ≥ 50,
otherwise **"Fail"**.

### ✔ Pseudocode

```text
BEGIN

    INPUT average

    IF average >= 50 THEN
        DISPLAY "Pass"
    ELSE
        DISPLAY "Fail"
    END IF

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Input average marks]
    B --> C{Average >= 50?}
    C -->|Yes| D[Pass]
    C -->|No| E[Fail]
    D --> F([End])
    E --> F
```

---

## 9. Calculate Factorial of a Number

Write the algorithm and draw the flowchart that input a number and
calculate its factorial using a loop.

### ✔ Pseudocode

```text
BEGIN

    INPUT number
    factorial = 1

    FOR i = 1 TO number DO
        factorial = factorial × i
    END FOR

    DISPLAY factorial

END

```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Input number]
    B --> C[Set factorial = 1]
    C --> D[Set i = 1]
    D --> E{i <= number?}
    E -->|Yes| F[factorial = factorial * i]
    F --> G[i = i + 1]
    G --> E
    E -->|No| H[/Display factorial/]
    H --> I([End])

```

---

## 10. Calculate Discount on Purchase

Write the algorithm and draw the flowchart for a program that inputs the
purchase amount and gives a **10% discount** if the amount is greater
than 1000.

### ✔ Pseudocode

```text
START

INPUT purchaseAmount

IF purchaseAmount > 1000 THEN
    discount = purchaseAmount * 0.10
    finalAmount = purchaseAmount - discount
ELSE
    finalAmount = purchaseAmount
END IF

OUTPUT finalAmount

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Input purchase amount]
    B --> C{Amount > 1000?}
    C -- Yes --> D[discount = amount * 0.10]
    D --> E[finalAmount = amount - discount]
    C -- No --> F[finalAmount = amount]
    E --> G([Output final amount])
    F --> G
    G --> H([End])

```

---

## Optional Exercises (11–16)

## 11. Online Shopping Delivery Eligibility

Write the algorithm and draw the flowchart for a program that inputs a
customer's purchase amount and displays **"Free Delivery"** if the
amount is 500 SEK or more; otherwise display **"Delivery Charge
Applies"**.

### ✔ Pseudocode

```text
START

INPUT purchaseAmount

IF purchaseAmount >= 500 THEN
    DISPLAY "Free Delivery"
ELSE
    DISPLAY "Delivery Charge Applies"
END IF

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Input purchase amount]
    B --> C{purchase amount >= 500 SEK?}
    C -->|Yes| D["Display Free Delivery"]
    C -->|No| E["Display Delivery Charge Applies"]
    D --> F([End])
    E --> F
```

---

## 12. Employee Salary and Bonus Calculator

Write the algorithm and draw the flowchart for a program that inputs an
employee's monthly salary and years of service, calculates a bonus of
**10%** for employees with 5 or more years of service and **5%** for
others, then displays the bonus and total salary.

### ✔ Pseudocode

```text
START

INPUT monthlySalary
INPUT yearsOfService

IF yearsOfService >= 5 THEN
    bonus = monthlySalary * 0.10
ELSE
    bonus = monthlySalary * 0.05
END IF

totalSalary = monthlySalary + bonus

DISPLAY bonus
DISPLAY totalSalary

END

```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Input monthly salary]
    B --> C[Input years of service]
    C --> D{Years of service >= 5?}
    D -->|Yes| E[bonus = salary * 10%]
    D -->|No| F[bonus = salary * 5%]
    E --> G[total salary = monthly salary + bonus]
    F --> G
    G --> H[Display bonus]
    H --> I[Display total salary]
    I --> J([End])

```
---

## 13. Mobile Data Usage Monitor

Write the algorithm and draw the flowchart for a program that inputs a
user's monthly data limit and data usage, then displays whether the user
has exceeded the limit or how much data remains.

### ✔ Pseudocode

```text
START

INPUT dataLimit
INPUT dataUsage

IF dataUsage > dataLimit THEN
    DISPLAY "Data limit exceeded"
ELSE
    remainingData = dataLimit - dataUsage
    DISPLAY "Data remaining: ", remainingData
END IF

END

```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Input data limit]
    B --> C[Input data usage]
    C --> D{Data usage > data limit?}
    D -->|Yes| E["Display Data limit exceeded"]
    D -->|No| F["remaining data = data limit - data usage"]
    F --> G["Display remaining data"]
    E --> H([End])
    G --> H

```
---

## 14. Login System (Maximum 3 Attempts)

Create an algorithm and flowchart for a login system that allows a user
up to 3 attempts to enter the correct password. Display **"Access
Granted"** if the password is correct; otherwise display **"Account
Locked"** after 3 failed attempts.

### ✔ Pseudocode

```text
START

SET correctPassword = "password123"
SET attempts = 0

WHILE attempts < 3
    INPUT password

    IF password = correctPassword THEN
        DISPLAY "Access Granted"
        END
    ELSE
        attempts = attempts + 1
    END IF
END WHILE

DISPLAY "Account Locked"

END


```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Set attempts = 0]
    B --> C[Input password]
    C --> D{Is password correct?}
    D -->|Yes| E["Display Access Granted"]
    D -->|No| F[attempts = attempts + 1]
    F --> G{attempts < 3?}
    G -->|Yes| C
    G -->|No| H["Display Account Locked"]
    E --> I([End])
    H --> I

```
---

## 15. Store Checkout with Multiple Items

Write the algorithm and draw the flowchart for a program that inputs the
number of items purchased, calculates the total purchase amount using a
loop, and applies a **15% discount** if the total exceeds 5000 SEK.

### ✔ Pseudocode

```text
START

INPUT numberOfItems
SET total = 0

FOR i = 1 TO numberOfItems
    INPUT itemPrice
    total = total + itemPrice
END FOR

IF total > 5000 THEN
    discount = total * 0.15
    total = total - discount
END IF

DISPLAY total

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Input number of items]
    B --> C[Set total = 0]
    C --> D[Set i = 1]
    D --> E{i <= number of items?}
    E -->|Yes| F[Input item price]
    F --> G[total = total + item price]
    G --> H[Set i = i + 1]
    H --> E
    E -->|No| I{Total > 5000 SEK?}
    I -->|Yes| J[discount = total * 15%]
    J --> K[total = total - discount]
    I -->|No| L[Keep total unchanged]
    K --> M[Display total]
    L --> M
    M --> N([End])

```
---

## 16. Electricity Bill Calculator

Write the algorithm and draw the flowchart for a program that inputs the
number of electricity units consumed and calculates the total bill using
the following rates: first 100 units at 1.5 SEK per unit, next 200
units at 2.0 SEK per unit, and all remaining units at 3.0 SEK per unit.

### ✔ Pseudocode

```text
START

INPUT units

SET bill = 0

IF units <= 100 THEN
    bill = units * 1.5

ELSE IF units <= 300 THEN
    bill = (100 * 1.5) + ((units - 100) * 2.0)

ELSE
    bill = (100 * 1.5) + (200 * 2.0) + ((units - 200 - 100) * 3.0)
END IF

DISPLAY bill

END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> B[Input units]
    B --> C[Set bill = 0]
    C --> D{Units <= 100?}

    D -->|Yes| E[Bill = units * 1.5]
    D -->|No| F{Units <= 300?}

    F -->|Yes| G["Bill = 100 * 1.5 + (units - 100)*2.0"]
    F -->|No| H["Bill = 100 * 1.5 + 200 * 2.0 + (units - 100 - 200) * 3.0"]

    E --> I[Display bill]
    G --> I
    H --> I
    I --> J([End])

```
---
