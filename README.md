# Mini Task Manager — React

A simple, responsive Task Management application built with React and Vite for the Aqualion Digital technical home exercise.

## Features

- Create tasks with title, description, and Low / Medium / High priority.
- View all tasks with priority and Pending / Completed status.
- Edit existing tasks.
- Mark pending tasks as completed and reopen completed tasks.
- Delete tasks with a confirmation prompt.
- Search by title or description.
- Filter by status and priority.
- Sort tasks by priority or newest first.
- Basic validation and helpful empty/error states.
- Persist tasks in browser `localStorage` so they remain after refresh.

## Requirements

- Node.js 18 or later
- npm

## Run locally

1. Extract the ZIP.
2. Open the project folder in VS Code or a terminal.
3. Install dependencies:

   ```bash
   npm install
   ```

4. Start the development server:

   ```bash
   npm run dev
   ```

5. Open the local URL printed by Vite (usually `http://localhost:5173`).

Create a production build with:

```bash
npm run build
```

## Project structure

```text
src/
  components/
    TaskForm.jsx
    TaskItem.jsx
    TaskList.jsx
  App.jsx
  main.jsx
  styles.css
```

## Implementation notes and assumptions

1. This is a React-only web application; it does not require a backend or database server.
2. `localStorage` is used as lightweight browser storage. Tasks are stored on the current browser/device and are not shared across devices.
3. Each task gets a unique ID using `crypto.randomUUID()` when available, with a timestamp-based fallback.
4. New tasks start with `Pending` status.
5. Priority and status values are restricted to the supported options in the UI.
6. Editing updates all task fields. Completing/reopening a task is a separate quick action.
7. Deleting asks for confirmation to reduce accidental removal.

## AI usage

- Tool used: ChatGPT.
- Purpose: to help plan the component structure, draft the React implementation, and prepare the README.
- The candidate should run the project, review the code, make any required changes, and be prepared to explain the implementation and design decisions during the technical discussion.

