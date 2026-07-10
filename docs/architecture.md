# TaskFlow Architecture v1.0

Status: LOCKED

## Overview

TaskFlow is a workflow management application for small teams (2–10 members).

The architecture prioritizes:

Simplicity
Maintainability
Readability
AI-assisted development

We intentionally avoid unnecessary complexity during MVP.

---

# Architecture

Browser

↓

Next.js App Router

↓

Route Handlers / Server Actions

↓

Service Layer

↓

Repository Layer

↓

PostgreSQL

---

## Frontend

Framework:
Next.js (App Router)
React
TypeScript

Reason:
One codebase
Excellent AI ecosystem
Server Components support
Simple deployment

Status:
LOCKED

---

## Backend

Architecture:
Modular Monolith

Components:
Route Handlers
Server Actions
Service Layer
Repository Layer

Reason:
Easy to maintain
Clear separation of concerns
Easy future extraction if needed

Status:
LOCKED

---

## Database

Database:
PostgreSQL

ORM:
Drizzle ORM

Reason:
Strong relational model
Excellent TypeScript support
Transparent SQL generation

Status:
LOCKED

---

## Authentication

Library:
Auth.js

Authentication:
Session-based Authentication

Reason:
Secure default
Easy integration with Next.js
Suitable for small teams

Status:
LOCKED

---

## Validation

Library:
Zod

Reason:
Shared validation
Strong typing
Avoid duplicated validation

Status:
LOCKED

---

## Styling

Tailwind CSS

Reason:
Fast development
Consistent UI
AI-friendly ecosystem

Status:
LOCKED

---

## UI Components

Library:
Radix UI

Reason:
Accessible
Unstyled primitives
Flexible

Status:
LOCKED

---

## Drag and Drop

Library:
@dnd-kit

Reason:
Modern
Flexible
Accessible

Status:
LOCKED

---

## Package Manager

pnpm

Reason:
Fast
Efficient
Great workspace support

Status:
LOCKED

---

# Deferred Decisions

The following decisions are intentionally postponed.

Deployment platform
Docker
CI/CD
Real-time communication
Redis
Email notifications
Mobile application
Offline mode
Multi-team support

These will only be discussed when required by the product.

---

# Out of Scope

TaskFlow will NOT include:

Chat
Video Call
Voice Call
Finance
Payroll
Invoice
Time Tracking

These features are outside the current Product Vision.

---

# Guiding Principle

Choose the simplest architecture that satisfies today's requirements.

Future complexity should only be added when justified by real product needs.