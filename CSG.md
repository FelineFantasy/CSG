# CSG - Code Style Guide

> **Code Style Guide** — coding standard for projects.
>
> 🇷🇺 **Русская версия:** [CSG.ru.md](CSG.ru.md)

---

## 🎯 Scope
This standard applies to all new projects (greenfield).
Existing projects are migrated gradually and may declare
a compliance level in their README:

- `CSG: full` — fully compliant
- `CSG: partial` — partially compliant, migration in progress
- `CSG: legacy` — not compliant, kept as-is

---

## 📁 Project Structure
- All code must reside within the `src/` or `app/` directory.
- No code should be placed in the project root.

---

## 📝 Documentation and Comments
- All code comments and documentation must be written in **English**.
- Every **executable script** (e.g., Python, Bash) should begin with a **shebang** (`#!/usr/bin/env ...`) followed by a multi-line comment describing the project or module.
- **Shebangs are not required** for:
  - Python modules (e.g., files meant to be imported, not executed directly).
  - Rust crates.
  - C/C++ source files.
  - Any language that does not use shebangs.

---

## 🐍 Naming Conventions
- **Variables, functions, directories:** `snake_case`
  Example: `get_data()`, `user_id`
- **Classes:** `CapitalizedCamelCase`
  Example: `CatDatabase`

---

## ⚠️ Error Handling
- The code must **never fail silently**.
- Critical errors must be caught using:
  - `try/except` (Python)
  - `Result` types (Rust)
  - Equivalent mechanisms in other languages
- Always display a **clear, user-friendly error message**.

---

## 🧠 Type Annotations
- Type annotations must be provided for **all function signatures**.
- Improves code clarity and enables static analysis.

---

## 📦 Commit Messages
- Must follow **Conventional Commits** standard:
  - `feat:`, `fix:`, `docs:`, `style:`, `refactor:`, `test:`, `chore:`
- Must be written exclusively in **English**.

---

## 📄 License
This document is part of the **CSG** project and is distributed under the MIT License.

---

**Author:** FelineFantasy
