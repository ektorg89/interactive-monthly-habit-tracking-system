# Interactive Monthly Habit Tracking System (Excel)

## Overview
This project is an interactive **monthly habit tracking system** built in **Microsoft Excel**.  
It allows users to track daily habits across each month using a multi-state input system and evaluates progress through a centralized statistics sheet.

The focus of this project is **system design, clarity, and correctness**, rather than overloading features or visual complexity.

---

## Motivation
The goal of this project was to build a **complete and usable system**, from idea to finished version (v1), without leaving it half-done.

The system is inspired by progress-tracking mechanics commonly found in applications and games, where progress is clearly visualized and evaluated over time.

---

## Project Structure


### Monthly Sheets (JAN–DEC)
Each month has its own sheet with:
- A full calendar layout (days + weekdays)
- A fixed list of habits
- Daily input cells for each habit

These sheets are responsible **only for data entry and visual feedback**.

---

### STATS Sheet
The `STATS` sheet acts as the **logic and analytics layer** of the system.

It calculates:
- Points earned per habit
- Days evaluated per habit
- Progress percentage per habit
- Overall monthly progress

A **dynamic month selector** allows switching between months (JAN–DEC), automatically updating all calculations.

---

## Habit Tracking Logic

Each daily habit cell supports four states:

- **Completed** → 1 point  
- **Partially completed** → 0.5 points  
- **Not completed** → 0 points  
- **Not evaluated** → blank (ignored)

### Scoring Formula

This approach ensures:
- Days not evaluated do not negatively affect progress
- Partial completion is reflected fairly
- Progress metrics remain meaningful and accurate

---

## Key Features

- Multi-state daily habit tracking
- One sheet per month (JAN–DEC) with consistent structure
- Conditional formatting for instant visual feedback
- Centralized statistics and calculations
- Dynamic month selection using dropdowns
- Clear separation between input and analytics

---

## Design Principles Applied

- **Separation of concerns**
  - Input (monthly sheets)
  - Logic (STATS)
- **Scalability**
  - Same structure reused across all months
- **Edge case handling**
  - Blank days are not treated as failures
- **Completion over perfection**
  - Version 1 was fully completed before adding new ideas

---

## Tools & Techniques Used

- Microsoft Excel
- Data Validation (dropdown inputs)
- Conditional Formatting
- Dynamic formulas
- INDIRECT-based references
- Percentage-based scoring logic

---

## What I Learned

- Designing systems with clear responsibility boundaries
- Handling real-world edge cases in data evaluation
- Translating raw user input into meaningful metrics
- Structuring projects to be scalable and maintainable
- The importance of defining scope and finishing a complete version

---

## Screenshots
Screenshots of the monthly view and the STATS page are available in the `/screenshots` folder.

---

## Future Improvements (Post V1)
- Optional visual dashboard
- Weekly summaries
- Trend analysis across months
- Exportable reports

These were intentionally left out of v1 to keep the system stable and focused.

---

## Version
**v1.0 — Completed**
