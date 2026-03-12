# CLAUDE.md
# Project Memory & AI Instructions
# (Loaded automatically by Claude Code in every session)

---

## 📌 Project Overview
**Name:**  
Describe the project purpose in 2–3 sentences.

**Tech Stack:**  
- Frontend:  
- Backend:  
- Database:  
- Infrastructure / CI/CD:  

**Key Domains:**  
(Example: authentication, payments, reporting, analytics, scheduling, etc.)

---

## 📁 Repository Structure (High‑Level)
Describe the major folders so Claude understands where things belong.

Example:
- `/src` – main application code  
- `/api` – backend endpoints  
- `/components` – UI components  
- `/lib` – helpers, utilities  
- `/tests` – unit/integration tests  
- `/scripts` – automations  

*(Update this for your repo.)*

---

## 🔧 Coding Conventions
These rules help Claude generate consistent code.

### **Language / Style**
- Use modern language features (e.g., async/await, ES modules, type hints).
- Prefer functional utilities where possible.
- Keep functions small, readable, composable.

### **Formatting**
- Follow Prettier/Black/GoFmt (specify your formatter).
- Enforce consistent import order and remove unused imports.

### **Error Handling**
- Always handle async errors.  
- Provide meaningful error messages.  
- Avoid silent failures.

### **Logging**
- Use structured logs.  
- Avoid printing sensitive data.

---

## 🧪 Testing Rules
- Every new feature should include tests located in `/tests/...`.
- Snapshot tests only when stable UI.
- Use dependency injection or mocks for external services.
- Keep tests deterministic and isolated.

---

## 🔐 Security & Data Rules
- Never log secrets, tokens, or user PII.
- Validate all external inputs.
- Use parameterized queries (no raw SQL unless sanitized).
- Follow least-privilege when generating CI scripts or infra code.

---

## 🏗️ Architectural Guidelines
### **Backend**
- Follow layered architecture (controllers → services → repositories).
- Avoid business logic in controllers.
- Use DTOs/schemas for validation.

### **Frontend**
- Keep UI pure; move business logic to hooks/services.
- Use reusable components over duplication.

### **APIs**
- REST or GraphQL? (Specify)  
- Response shape conventions.  
- Error format convention (example: `{ error: string, details?: any }`).

---

## 🔄 Git & Workflow Rules
- Use meaningful commit messages.  
- Keep PRs small and focused.  
- Always create a new branch for changes.  
- Do not commit environment secrets.

---

## 🤖 Claude Code Behavior Instructions
These rules tell the AI how you want it to behave.

### **General Rules**
- Before making large changes, generate a **plan** and wait for approval.
- Keep diffs minimal and readable.
- When refactoring, preserve behavior unless explicitly told otherwise.
- If unsure, ASK before proceeding.

### **File Editing**
- Use atomic PRs for big changes.  
- When modifying code, include comments summarizing reasoning if non-obvious.

### **Testing & Verification**
- After implementing changes, run tests automatically.
- If tests fail, attempt to fix them before returning the result.

### **Documentation**
- Update README or docs whenever generating features requiring explanation.

---

## 📚 Domain Knowledge (Optional)
Add domain or business rules Claude should always follow.

Examples:
- “User IDs are UUIDv4 only.”
- “Transactions must be idempotent.”
- “Never modify data outside the `tenant_id` scope.”

---

## 🚧 Known Issues / Workarounds
Document quirks or technical debt Claude should keep in mind.

Example:
- “Legacy `/auth` module—avoid refactoring until migration is complete.”
- “Search service rate-limits to 10 req/sec.”

---

## 📝 Custom Instructions to Agents
- Use subagents for repo scanning or large refactors.  
- Use clear diff blocks for multi-file changes.  
- Prefer creating small commits grouped by logical change.  
- When generating migrations, provide SQL + code changes together.

---

## 🎯 Goals for This Project
List long-term aims so Claude aligns changes with your direction.

Example:
- Improve test coverage to 80%.  
- Reduce complexity in the payment workflows.  
- Migrate API from REST to GraphQL.  

---

# End of CLAUDE.md