# 💰 Who Wants to Be a Millionaire? (C# Console)

A fully text-based, command-line implementation of the classic TV game show *Who Wants to Be a Millionaire?*. This project was built using **C#** and the **.NET Core CLI**, serving as a comprehensive showcase of Object-Oriented Programming (OOP) principles and robust File Handling.

---

## 🚀 Features

*   **15-Question Ladder:** Progressively harder questions.
*   **The 3 Classic Lifelines:** 
    *   *50:50* – Eliminates two random incorrect answers.
    *   *Phone a Friend* – Simulates a friend's advice with varying accuracy based on difficulty.
    *   *Ask the Audience* – Simulates audience voting percentages.
*   **Walk Away Option:** Players can secure their current winnings before risking a wrong answer.
*   **Persistent High Scores:** Saves the player's name and final score to a local data file.

---

## 🛠️ Core Concepts Demonstrated

This project represents a major milestone in my development journey, moving from basic scripts to structured, modular software architecture.

### 1. Object-Oriented Programming (OOP)
*   **Encapsulation:** Question data, player profiles, and game states are isolated within dedicated classes with restricted access modifiers (`private`, `public`, `internal`).
*   **Inheritance & Polymorphism:** Lifelines are structured under a base `Lifeline` class, allowing distinct behaviors while sharing core game-state access.
*   **Abstraction:** The complex rules of the game loops, score calculations, and randomizations are hidden behind clean, reusable methods like `GameController.StartSession()`.

### 2. File Handling & Data Parsing
*   **Dynamic Question Loading:** Questions are not hardcoded. The application reads from an external `.txt` or `.csv` data bank file, parsing questions, options, and difficulty tiers at runtime.
*   **Leaderboard Persistence:** Stream readers and writers (`StreamReader` / `StreamWriter`) handle saving and loading historical player scores, ensuring user data persists even after closing the application.

---
