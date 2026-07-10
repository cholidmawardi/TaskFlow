# TaskFlow Coding Rules v1.0

These rules apply to both developers and AI assistants.

The goal is consistency, readability, and long-term maintainability.

---

# Philosophy

Always prefer:

Simplicity
Readability
Maintainability

Never optimize for clever code.

Optimize for understandable code.

---

# General Rules

## 1. TypeScript

Always use TypeScript.

Strict Mode is required.

Never disable type checking.

---

## 2. No any

Avoid any.

If unavoidable, explain why with a comment.

---

## 3. Naming

Names must clearly describe their purpose.

Good

assignedTasks

Bad

data

tmp

value

---

## 4. Single Responsibility

One function should have one responsibility.

Avoid long functions.

---

## 5. Small Components

Prefer small reusable components.

Avoid components larger than necessary.

---

## 6. Business Logic

Business logic must NEVER exist inside UI components.

Business logic belongs in the Service Layer.

---

## 7. Validation

Always validate input using Zod.

Never duplicate validation logic.

---

## 8. Database Access

Database access must go through the Repository Layer.

UI must never access the database directly.

---

## 9. Comments

Comments should explain WHY.

Do not explain WHAT.

Bad

// increment counter

Good

// Prevent duplicate task ordering after drag-and-drop

---

## 10. Keep It Simple

Prefer the simplest implementation that solves the problem.

Avoid premature optimization.

---

# AI Collaboration Rules

AI must:

Read README.md before coding.
Read docs/vision.md before coding.
Read docs/architecture.md before coding.
Follow these coding rules.
Ask questions if requirements are unclear.
Explain important trade-offs.
Never assume missing requirements.
Never introduce unnecessary libraries.
Never create features outside Product Vision.
Prefer readability over cleverness.

---

# Git Rules

Use Conventional Commits.

Examples:

feat:

fix:

docs:

refactor:

test:

chore:

Keep commits small and focused.

---

# Project Scope

TaskFlow is NOT:

Chat Application
Social Media
ERP
HR System
Finance Application

AI should reject features outside the Product Vision unless explicitly approved.

---

# Security

Never commit:

.env
API Keys
Passwords
Secrets

Always use environment variables.

---

# Final Principle

Every line of code should make the project easier to understand.

Not harder.