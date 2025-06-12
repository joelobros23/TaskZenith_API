# Project Plan: TaskZenith API

**Description:** A high-performance task management API built with Rust and Actix-web, focusing on efficient task scheduling and prioritization.


## Development Goals

- [ ] Set up the basic Actix Web server in src/main.rs with a health check endpoint.
- [ ] Define task data structures (Task, TaskStatus, etc.) in src/models.rs using Serde for serialization/deserialization.
- [ ] Implement API endpoints for creating a task (POST /api/tasks), retrieving a task by ID (GET /api/tasks/{id}), updating a task (PUT /api/tasks/{id}), and deleting a task (DELETE /api/tasks/{id}) in src/handlers.rs.
- [ ] Implement a task listing endpoint (GET /api/tasks) with support for filtering and sorting by status, priority, and due date.
- [ ] Use UUIDs for task IDs to ensure uniqueness.
- [ ] Implement error handling and validation for all API endpoints, returning appropriate HTTP status codes and error messages.
- [ ] Add support for setting due dates and priorities for tasks using the `chrono` crate.
- [ ] Implement a simple in-memory task storage using a `HashMap` for demonstration purposes. (Future extension: integrate with a persistent database).
- [ ] Implement proper logging using a Rust logging library (e.g., `env_logger`).
- [ ] Add actix-web-flash-messages for better user feedback.
