### 🔄 Project Awareness & Context
- **Always read `PLANNING.md`** at the start of a new conversation to understand the project's architecture, goals, style, and constraints.
- **Check `TASK.md`** before starting a new task. If the task isn't listed, add it with a brief description and today's date.
- **Use consistent naming conventions, file structure, and architecture patterns** as described in `PLANNING.md`.
- **Use npm or yarn** for package management and script execution, including for running tests.

### 🧱 Code Structure & Modularity
- **Never create a file longer than 500 lines of code.** If a file approaches this limit, refactor by splitting it into modules or helper files.
- **Organize code into clearly separated modules**, grouped by feature or responsibility.
  For applications this looks like:
    - `index.js` or `app.js` - Main application entry point and setup
    - `routes/` - API route handlers and middleware
    - `services/` - Business logic and external service integrations
    - `models/` - Data models and database schemas
    - `utils/` - Helper functions and utilities
    - `config/` - Configuration files and environment setup
- **Use clear, consistent imports** (prefer ES6 modules with `import/export`).
- **Use dotenv** for environment variables with `process.env`.

### 🧪 Testing & Reliability
- **Always create unit tests for new features** (functions, classes, routes, etc) using Jest, Mocha, or your preferred testing framework.
- **After updating any logic**, check whether existing unit tests need to be updated. If so, do it.
- **Tests should live in a `/tests` or `/__tests__` folder** mirroring the main app structure.
  - Include at least:
    - 1 test for expected use
    - 1 edge case
    - 1 failure case

### ✅ Task Completion
- **Mark completed tasks in `TASK.md`** immediately after finishing them.
- Add new sub-tasks or TODOs discovered during development to `TASK.md` under a "Discovered During Work" section.

### 📎 Style & Conventions
- **Use JavaScript/TypeScript** as the primary language (prefer TypeScript for larger projects).
- **Follow ESLint and Prettier** for code formatting and linting.
- **Use JSDoc for documentation** and TypeScript types for type safety.
- Use **Express.js** for APIs, **Mongoose** or **Prisma** for ORM if applicable.
- Write **JSDoc comments for every function**:
  ```javascript
  /**
   * Brief summary.
   * 
   * @param {string} param1 - Description.
   * @param {number} param2 - Description.
   * @returns {Promise<Object>} Description of return value.
   */
  function example(param1, param2) {
      // implementation
  }
  ```

### 📚 Documentation & Explainability
- **Update `README.md`** when new features are added, dependencies change, or setup steps are modified.
- **Comment non-obvious code** and ensure everything is understandable to a mid-level developer.
- When writing complex logic, **add an inline `// Reason:` comment** explaining the why, not just the what.

### 🧠 AI Behavior Rules
- **Never assume missing context. Ask questions if uncertain.**
- **Never hallucinate libraries or functions** – only use known, verified npm packages and Node.js APIs.
- **Always confirm file paths and module names** exist before referencing them in code or tests.
- **Never delete or overwrite existing code** unless explicitly instructed to or if part of a task from `TASK.md`.