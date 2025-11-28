# Piscine Mobile - 0: Introduction to Mobile Development

**Version:** 2.3

## Summary

This document contains the subject matter for Module00 of the Piscine Mobile.

---

## Table of Contents

1. [Instructions](#chapter-i-instructions)
2. [Introduction](#chapter-ii-introduction)
   - [II.1 What is a mobile application?](#ii1-what-is-a-mobile-application)
   - [II.2 What is Flutter?](#ii2-what-is-flutter)
3. [Exercise 00: A basic display](#chapter-iii-exercise-00-a-basic-display)
4. [Exercise 01: Say Hello to the World](#chapter-iv-exercise-01-say-hello-to-the-world)
5. [Exercise 02: More Buttons](#chapter-v-exercise-02-more-buttons)
6. [Exercise 03: It's Alive!](#chapter-vi-exercise-03-its-alive)
7. [Submission and peer-evaluation](#chapter-vii-submission-and-peer-evaluation)

---

## Chapter I: Instructions

- Only this page will serve as reference. Do not trust rumors.
- Read attentively the whole document before beginning.
- Your exercises will be corrected by your piscine colleagues.
- The document can be relied upon, do not blindly trust the demos or pictures example which can contain not required additions.
- Got a question? Ask your peer on the right. Otherwise, try your peer on the left.
- By Odin, by Thor! Use your brain!!!

⚠️ **Important Notice:**

Intra indicates the date and the hour of closing for your repositories. This date and hour also corresponds to the beginning of the peer-evaluation period for the corresponding piscine day. This peer-evaluation period lasts exactly 24h. After 24h passed, your missing peer grades will be completed with a 0.

---

## Chapter II: Introduction

### II.1 What is a mobile application?

A mobile application is a software program designed to run on mobile devices, such as personal digital assistants, enterprise digital assistants, or mobile phones.

These applications can either be pre-installed on phones during manufacturing or delivered as web applications using server-side or client-side processing.

Mobile applications often differ from desktop applications, which run on desktop computers, and web applications, which run in mobile web browsers rather than directly on the mobile device.

### II.2 What is Flutter?

Flutter is Google's mobile UI framework for crafting high-quality native interfaces on iOS and Android in record time.

Flutter works with existing code, is used by developers and organizations around the world, and is free and open source.

---

## Chapter III: Exercise 00: A basic display

### Exercise Information

| Field | Value |
|-------|-------|
| **Name** | A basic display |
| **Turn-in directory** | mobileModule00 |
| **Files to turn in** | ex00 and all necessary files |
| **Forbidden functions** | None |

⚠️ **Framework Note:**

As explained in the main project, we are using Flutter for these projects, so we will sometimes use terms specific to this framework. It is up to you to adapt and find the equivalent in the framework you choose to use.

### Objective

For your first exercise, you will need to create a new ex00 project using the tools provided by the framework of your choice.

If you are using Flutter, it is important to understand the structure of a Flutter project and, for this exercise, what **widgets** are and their different states.

### Requirements

For now, your project must contain a single page with some widgets:

- A text widget with a button below it, both centered horizontally and vertically.
- When the button is clicked, you must display "Button pressed" in the debug console.
- Your application must be responsive.

### Expected Output

Your application should look something like this:

**On Phone:**
- Centered text: "A simple text"
- Below: "Click me" button

**On Tablet:**
- Same layout but scaled for larger screen

**Debug Console:**
```
I/flutter (50264): Button pressed
```

---

## Chapter IV: Exercise 01: Say Hello to the World

### Exercise Information

| Field | Value |
|-------|-------|
| **Name** | Say Hello to the World |
| **Turn-in directory** | mobileModule00 |
| **Files to turn in** | ex01 and all necessary files |
| **Forbidden functions** | None |

💡 **Tip:**

For this exercise, you will need to retrieve the code from your previous exercise and create a new ex01 project.

### Objective

Now you will need to ensure that the text displayed in the application changes when you click the button.

### Requirements

- It should display "Hello World!" instead of the initial text.
- Each time you click the button, the text should toggle between the initial text and "Hello World!".

### Expected Output

**Base State:**
- Text displays: "A simple text"

**After First Click:**
- Text displays: "Hello World"

**After Second Click:**
- Text displays: "A simple text"

---

## Chapter V: Exercise 02: More Buttons

### Exercise Information

| Field | Value |
|-------|-------|
| **Name** | More Buttons |
| **Turn-in directory** | mobileModule00 |
| **Files to turn in** | ex02 and all necessary files |
| **Forbidden functions** | None |

### Objective

Now that you understand the basics of displaying text and buttons, create a new project called ex02.

In this new project, display an **AppBar** at the top of your screen with the title "Calculator".

### Requirements

You also need to add two TextFields (one to display the expression and one to display the result) and several buttons. For now, just display "0" inside both TextFields; you will handle this in the next exercise.

**Buttons to implement:**

- Numbers from 0 to 9
- "." for decimal numbers
- "AC" to reset the expression and result
- "C" to delete the last character of the expression
- "=" to display the result of the expression
- Operators: "+", "-", "*", "/"

**Debug Feature:**

Add a debug feature. For each button you press, display the text of the button in the debug console.

**Responsiveness:**

Once all the buttons are properly set, make sure the display is responsive for all devices (phone, tablet, etc.).

### Expected Output

Your calculator should display:
- AppBar with title "Calculator"
- Two TextFields showing "0"
- Grid of buttons with numbers, operators, and control buttons
- Layout should adapt to different screen sizes

**Debug Console Example:**
```
I/flutter (30769): button pressed '+'
I/flutter (30769): button pressed '4'
I/flutter (30769): button pressed '6'
I/flutter (30769): button pressed '*'
I/flutter (30769): button pressed '5'
I/flutter (30769): button pressed '-'
```

---

## Chapter VI: Exercise 03: It's Alive!

### Exercise Information

| Field | Value |
|-------|-------|
| **Name** | It's Alive! |
| **Turn-in directory** | mobileModule00 |
| **Files to turn in** | calculator_app and all necessary files |
| **Forbidden functions** | None |

💡 **Tip:**

For this exercise, you will need to retrieve the code from your previous exercise and create the calculator_app project. You can use the `math_expressions` library or an equivalent library.

### Objective

Now it's time to make your calculator work! You need to add the logic behind it.

The TextFields created in the previous exercise must now display the expression and the result of the expression.

### Requirements

**Supported Operations:**

- Addition
- Subtraction
- Multiplication
- Division

**Features:**

- You can perform multiple operations in one expression (e.g., `1 + 2 * 3 - 5 / 2`)
- You must be able to enter a negative number (by pressing the "-" button before the number)
- You must be able to enter decimal numbers
- You must be able to delete the last character of the expression
- You must be able to clear the whole expression and result

### Important Notes

Be careful—if you don't thoroughly test your code, you might encounter issues. For example, an incorrect expression, division by 0, or very large numbers can cause problems.

⚠️ **Critical Requirement:**

**Your application must NEVER crash!**

### Expected Output

Your calculator should:
- Display mathematical expressions as you type them
- Show the calculated result in real-time or when "=" is pressed
- Handle all edge cases gracefully (division by zero, invalid expressions, etc.)
- Maintain responsive layout on different screen sizes

---

## Chapter VII: Submission and peer-evaluation

Turn in your assignment in your Git repository as usual. Only the work inside your repository will be evaluated during the defense. Don't hesitate to double check the names of your folders and files to ensure they are correct.

ℹ️ **Important:**

The evaluation process will happen on the computer of the evaluated group.

---

## Project Structure Summary

```
mobileModule00/
├── ex00/                    # Basic display exercise
│   └── (Flutter project files)
├── ex01/                    # Hello World toggle exercise
│   └── (Flutter project files)
├── ex02/                    # Calculator layout exercise
│   └── (Flutter project files)
└── calculator_app/          # Functional calculator
    └── (Flutter project files)
```

## Key Learning Outcomes

By completing this module, you will understand:

1. **Flutter Basics:**
   - Project structure
   - Widget fundamentals
   - State management
   - UI layout and responsiveness

2. **Mobile Development Concepts:**
   - How mobile applications differ from web/desktop apps
   - Responsive design for multiple screen sizes
   - User interaction handling (button clicks, text input)
   - Debug console logging

3. **Practical Skills:**
   - Creating functional UI components
   - Handling state changes
   - Implementing business logic (calculator)
   - Error handling and edge cases
   - Cross-device compatibility

---

**Last Updated:** Version 2.3
**Framework:** Flutter (Google's mobile UI framework)
**Target Platforms:** iOS and Android
