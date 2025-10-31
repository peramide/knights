# ♞ Knights and Knaves Logic Solver

A Python program that uses **propositional logic** and **model checking** to solve **Knights and Knaves** puzzles. It models each character’s statements to determine who tells the truth (knights) and who lies (knaves), demonstrating **logical inference** and **automated reasoning** in AI.

---

## 🧠 Overview

Inspired by **Raymond Smullyan’s** classic logic puzzles, this project showcases how **AI can reason about truth and lies** using formal logic.

In every puzzle:

* A **Knight** 🛡️ always tells the truth.
* A **Knave** 🤥 always lies.

The AI uses propositional logic to represent each puzzle as a **knowledge base**, then applies **model checking** to deduce each character’s identity.

---

## 🧩 Puzzles and Results

### **Puzzle 0**

**Statement:**
A says, “I am both a knight and a knave.”

**Result:**
🧩 A is a **Knave**

---

### **Puzzle 1**

**Statements:**
A says, “We are both knaves.”
B says nothing.

**Result:**
🧩 A is a **Knave**
🧩 B is a **Knight**

---

### **Puzzle 2**

**Statements:**
A says, “We are the same kind.”
B says, “We are of different kinds.”

**Result:**
🧩 A is a **Knight**
🧩 B is a **Knave**

---

### **Puzzle 3**

**Statements:**
A says either “I am a knight.” or “I am a knave.” (you don’t know which)
B says, “A said ‘I am a knave.’”
B then says, “C is a knave.”
C says, “A is a knight.”

**Result:**
🧩 A is a **Knight**
🧩 B is a **Knave**
🧩 C is a **Knight**

---

## ⚙️ How It Works

Each puzzle is represented as a **knowledge base (KB)** combining:

1. Logical structure: every person is either a knight or a knave (not both).
2. Statements made by each character, expressed as logical formulas.

The program applies **model checking** to explore all possible truth assignments and determines which ones satisfy the KB — identifying who’s telling the truth and who’s lying.

---

## 🗂️ Project Structure

* **`logic.py`** – Implements logical connectives (`And`, `Or`, `Not`, `Implication`, etc.) and model checking.
* **`puzzle.py`** – Encodes the puzzles (`knowledge0`–`knowledge3`) and runs the solver.

---

## 🚀 Run the Solver

```bash
git clone https://github.com/yourusername/knights.git
cd knights
python puzzle.py
```

You’ll see the reasoning results printed for each puzzle, as shown above.

---

## 🧠 Key Concepts

* Propositional Logic & Knowledge Representation
* Model Checking & Inference
* Automated Reasoning
* AI Problem Solving

---

## 📚 Acknowledgements

**CS50’s Introduction to Artificial Intelligence with Python**

