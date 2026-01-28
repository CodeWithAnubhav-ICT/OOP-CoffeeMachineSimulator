# ☕ OOP Smart Coffee Machine (v2.0)

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![Architecture](https://img.shields.io/badge/Architecture-OOP-orange?style=for-the-badge)

> **A complete refactor of the Coffee Machine Simulator using Object-Oriented Programming (OOP).**

---

## 🔄 The Refactor Story (v1 vs v2)
In **Day 15**, I built this machine using *Procedural Programming*. It worked, but the code was a single file with complex dependency on global variables.

In **Day 16**, I rebuilt the system from scratch using **OOP**. This version treats every component as a distinct software object, making the codebase:
* **Modular:** Components (`CoffeeMaker`, `MoneyMachine`) can be reused or replaced independently.
* **Scalable:** Adding new functionality (like a new payment method) doesn't break the coffee logic.
* **Readable:** The `main.py` is now a simple "manager" script that delegates tasks to the objects.

---

## 🏗️ System Architecture
The project is split into three primary classes:

| Class | Responsibility | Methods |
| :--- | :--- | :--- |
| **`CoffeeMaker`** | Manages resources (water, milk, coffee). | `report()`, `is_resource_sufficient()`, `make_coffee()` |
| **`MoneyMachine`** | Handles currency, change, and profit. | `report()`, `make_payment()` |
| **`Menu`** | Manages drink items and ingredients. | `get_items()`, `find_drink()` |

---

## 🛠️ How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/CodeWithAnubhav-ICT/OOP-Coffee-Machine.git](https://github.com/CodeWithAnubhav-ICT/OOP-Coffee-Machine.git)
    ```
2.  **Run the application:**
    ```bash
    python main.py
    ```

## 🎮 Usage
* **User Experience:** Identical to the v1 simulator (Order -> Insert Coins -> Enjoy).
* **Developer Experience:** vastly improved code structure and maintenance capability.

---
*Part of my [100 Days of Code Journey](https://github.com/CodeWithAnubhav-ICT).*
