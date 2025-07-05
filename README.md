# ⚽ Football Management System in C++

## 📌 Overview

This **Football Management System** is a console-based C++ project that simulates the operations of a football club. It allows to:

- Add and view players, stadiums, chairmen, and winners.
- Simulate football matches (practice and league).
- Assess player skills and fitness.
- Handle match outcomes including penalties.
- Use exception handling for invalid inputs.

---

## 🚀 Features

### ✅ Management Functionalities

- **Add / View**:
  - Stadiums
  - Chairmen
  - Players
  - Past Winners

### 🏟 Match Simulation

- **Match Types**:
  - Practice Match
  - League Match (includes penalties if drawn)
- **Flow**:
  - Simulates 2 halves (5 rounds each)
  - Displays goal stats at halftime and end
  - Handles extra penalty rounds if required

### 🧪 Player Assessment

- **Goal-Scoring Test**
- **Fitness Test**:
  - Motor Skill
  - Cognitive Skill
  - Perception Skill

### 🧾 Menu Options
```text
  1. ADD STADIUM
  2. DISPLAY STADIUM
  3. ADD CHAIRMAN
  4. DISPLAY CHAIRMAN
  5. PLAY A GAME
  6. ADD PLAYER
  7. DISPLAY PLAYER
  8. GET TEAM
  9. ADD WINNER LIST
  10. GET WINNER LIST
  11. QUIT
---

### 🔐 Exception Handling

- `choiceexception` – Invalid menu input
- `yearexception` – Negative year values
- `ageexception` – Negative age values

---

## 📂 Class Structure

- `game` (abstract class): Match engine base
  - `practice`, `league`: Derived for match types
- `football`: Interface to manage menu and actions
- `win`, `ground`, `chairman`, `atagar`: Data classes
- `Winner`, `stadium`, `president`, `player`: Handlers for input/display
- `yearexception`, `choiceexception`, `ageexception`: Custom exception classes

---

## 🧑‍💻 How to Run

1. **Compile** the project:
   ```bash
   g++ football_management.cpp -o football_management
