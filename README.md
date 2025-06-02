## 💻 Live Coding – Appointment Booking System

### Objective

Implement a basic appointment booking system using Rails 8 and Turbo.

### Requirements

Users should be able to book appointments. Each appointment must have:

- Start date and time (`starts_at`)
- Duration in minutes (`duration_minutes`)
- Status (`pending`, `confirmed`, `cancelled`)

You must:

- Set up the necessary models, controllers, and views from scratch.
- Create a minimal UI to **list and create appointments**, using **Turbo Frames or Streams**.
- Ensure that **appointments cannot overlap** in time for the same user.
- Decide **how and where to implement the overlap validation logic** (e.g. at the model, service, or database level).

You can assume a `User` model will be created as part of the task. There is no authentication—just associate appointments with a user manually.

### Time estimate

20 minutes.

### Scope

- Use Turbo to update the appointment list when a new one is created.
- Use any method you prefer to render the appointment form and list.
- Implement proper validations to prevent invalid or conflicting data.

### Nice to have

- Propose or implement a strategy to **scale appointment conflict validation** (e.g. through database constraints, indexes, or background checks).
- Add a basic test or comment explaining how the system would behave under high concurrency.
