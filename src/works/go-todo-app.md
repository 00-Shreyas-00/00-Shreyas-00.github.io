---
title: Go Todo App
order: 2
featured: true
year: 2026
category: Backend, Go
stack: Go, Gin, PostgreSQL, JWT, React
thumbLabel: Go · Gin · PostgreSQL
summary: A basic to-do application with a Go REST API (Gin, PostgreSQL via pgx, JWT authentication) and a React and TypeScript frontend.
repo: https://github.com/00-Shreyas-00/Go-Todo-app
---

## Backend

### A layered Go API

The API is a Go module with a `cmd/api` entry point and `internal` packages for configuration, the PostgreSQL connection, HTTP handlers, authentication middleware, models and repositories. Versioned SQL migrations create the todo and user tables and link each todo to its user.

## Frontend

### React and TypeScript

A Vite-based React frontend provides login and registration pages, protected routes, and a todo list with display filters.
