<div align="center">

# 🐍 Object-Oriented Programming in Python
### A Hands-On 2-Hour Tutorial

*From zero OOP to building a real abstract-base-class hierarchy — in one Jupyter notebook.*

[![Python](https://img.shields.io/badge/python-3.10+-3776ab.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-f37626.svg?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Level: Beginner → Intermediate](https://img.shields.io/badge/level-beginner%20%E2%86%92%20intermediate-blue.svg)](#)

</div>

---

## Overview

This repository contains a **self-contained, pedagogically-structured Jupyter notebook** that teaches Object-Oriented Programming (OOP) in Python from the ground up. It is designed for learners who already know basic Python (functions, lists, loops) but have **never written a class** before.

The tutorial covers every core OOP concept, uses consistent, beginner-friendly examples throughout, and culminates in a **capstone project** that ties every concept together: a mini **library management system** with abstract base classes, composition, properties, and operator overloading.

> **Time commitment:** ~2 hours of active reading + running cells + doing exercises.

---

##  What You Will Learn

<table>
<tr>
<td width="50%" valign="top">

### Core concepts
- ✅ Classes and instances
- ✅ Instance vs. class variables
- ✅ Instance, class, and static methods
- ✅ Inheritance and `super()`
- ✅ Method overriding and polymorphism
- ✅ Special (dunder) methods

</td>
<td width="50%" valign="top">

### Advanced topics
- ✅ Property decorators (`@property`, setters, deleters)
- ✅ Encapsulation & naming conventions
- ✅ Abstract Base Classes (`abc` module)
- ✅ Composition vs. inheritance
- ✅ Operator overloading (`+`, `==`, `<`, `len`, `in`, `[]`, …)

</td>
</tr>
</table>

---

## Notebook Roadmap

```
0. Motivation — why do we need classes?
     │
     ▼
1. Classes & Instances ─────── your first class, self, __init__
     │
     ▼
2. Class Variables ─────────── shared state, the mutable-default trap
     │
     ▼
3. Method Types ────────────── instance / class / static
     │
     ▼
4. Inheritance ─────────────── super(), overriding, polymorphism, MRO
     │
     ▼
5. Dunder Methods ──────────── __repr__, __eq__, __lt__, __add__, __len__ …
     │
     ▼
6. Properties ──────────────── getter, setter, deleter, validation
     │
     ▼
7. Encapsulation & ABCs ────── _private, @abstractmethod, composition
     │
     ▼
8. Capstone: Library Management System
     │
     ▼
9. Summary & further reading
```

Each section ends with a short **hands-on exercise** so you can test your understanding immediately.

---

## Getting Started

### Prerequisites

- Python **3.10 or later**
- `jupyter` (or an IDE with native notebook support such as VS Code or PyCharm)

### Run locally (recommended)

```bash
# 1. Clone the repo
git clone https://github.com/demirayonur/OOP-Tutorial.git
cd oop-python-tutorial

# 2. (Optional but recommended) create a virtual environment
python -m venv .venv
source .venv/bin/activate          # macOS / Linux
# .venv\Scripts\activate           # Windows

# 3. Install Jupyter
pip install jupyter

# 4. Launch
jupyter notebook OOP_in_Python_Tutorial.ipynb
```
---

## How to Get the Most Out of This Tutorial

> **Read → Run → Break → Fix → Repeat.**

1. **Read** each markdown cell carefully. The explanations are written to build intuition, not just list facts.
2. **Run** every code cell yourself. Don't just read the output.
3. **Break** the code on purpose. Change a class variable to a list. Assign a negative value. See what happens.
4. **Fix** it. That is where the real learning happens.
5. **Do the exercises** before reading the solution in the next cell.

Each section is designed so you can stop, take a break, and come back without losing your place.

---

## Repository Structure

```
oop-python-tutorial/
├── OOP_in_Python_Tutorial.ipynb     ← the tutorial (start here)
├── README.md                        ← you are here
└── .gitignore                       ← standard Python .gitignore
```

---


## Capstone Project: Library Management System

The final section builds a realistic mini-system that uses **every concept** from the tutorial:

- **Abstract base class** (`LibraryItem`) with abstract methods
- **Inheritance tree**: `PrintBook`, `EBook`, `AudioBook`
- **Class-level ID counter** auto-assigning unique IDs
- **Properties** with validation (page count, duration)
- **State management** (check-out / return logic)
- **Dunder methods** for equality, ordering, iteration, membership, and length
- **Composition**: a `Library` that *has* items rather than *is* one
- **Alternative constructor** via `@classmethod`
- **Static helper** via `@staticmethod`

---

## 🙋 FAQ

<details>
<summary><strong>Do I need to install anything besides Jupyter?</strong></summary><br/>
No. The entire tutorial uses only the Python standard library (<code>abc</code>, <code>functools</code>, <code>dataclasses</code>, <code>collections.abc</code>). No <code>pip install ...</code> of third-party packages is required.
</details>

<details>
<summary><strong>Why Python 3.10+?</strong></summary><br/>
The tutorial uses modern type-hint syntax like <code>list[Book]</code> and <code>int | None</code> (PEP 604), which require Python 3.10 or later. If you are on 3.9, the notebook still runs thanks to <code>from __future__ import annotations</code>, but upgrading is recommended.
</details>

<details>
<summary><strong>I found a typo / have a suggestion. What should I do?</strong></summary><br/>
Open an issue or submit a pull request. See the Contributing section below.
</details>

---

## 🤝 Contributing

Contributions are warmly welcomed! If you spot a typo, think an explanation could be clearer, or want to add an exercise:

1. Fork the repository
2. Create a feature branch (`git checkout -b improve/section-5-examples`)
3. Commit your changes (`git commit -m 'Improve dunder section example'`)
4. Push to the branch (`git push origin improve/section-5-examples`)
5. Open a Pull Request

For larger changes, please open an issue first to discuss what you would like to modify.

---

## 📜 License

This work is released under the **MIT License** — see the [LICENSE](LICENSE) file for details.

You are free to use, modify, and distribute this material for any purpose, including commercial and educational use.

---

## 🌟 Acknowledgments

Inspired by the countless educators who have made Python OOP approachable over the years. Special thanks to the Python Software Foundation for maintaining such an elegant, teachable language.

---

<div align="center">

### If this tutorial helped you, please consider giving it a ⭐ on GitHub!

*Happy coding.* 🐍

</div>
