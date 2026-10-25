---
title: Cleanzy
order: 1
featured: true
year: 2026
category: Full-stack, Backend
stack: TypeScript, Express, Prisma, PostgreSQL, Docker
thumbLabel: TypeScript · Express · Prisma
summary: A full-stack housekeeping management web platform built with TypeScript, Node.js (Express), Prisma ORM and PostgreSQL, with separate role-based interfaces for customers, housekeepers and administrators.
repo: https://github.com/00-Shreyas-00/Cleanzy
---

## Roles

### Customers, housekeepers and administrators

Customers browse cleaning services, get distance-based pricing, schedule bookings, leave ratings and reviews, and track their service history. Housekeepers view assignments, record daily check-in and check-out attendance, accept or reject jobs, and manage their availability. Administrators monitor live bookings, review staff performance metrics, manage leave requests and oversee platform analytics.

## Running it

### Docker, migrations and tests

The app ships with a multi-stage Dockerfile and a Docker Compose setup that runs the application alongside PostgreSQL. Prisma handles migrations, a seed script loads demo accounts and a service catalogue, and the test suite runs with Vitest.
