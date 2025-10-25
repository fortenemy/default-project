
# Task List Management

Guidelines for managing task lists in markdown files to track progress on completing a PRD

## Task Implementation

- **One parent-task at a time:** Do **NOT** start the next parent‑task until you ask the user for permission.
- **Completion protocol:**  
  1. When you finish a **sub‑task**, immediately mark it as completed by changing `[ ]` to `[x]`.  
  2. If **all** subtasks underneath a parent task are now `[x]`, also mark the **parent task** as completed.  
- Stop after each sub‑task and wait for the user's go‑ahead.

## Task List Maintenance

1. **Update the task list as you work:**
   - Mark tasks and subtasks as completed (`[x]`) per the protocol above.
   - Add new tasks as they emerge.

2. **Maintain the "Relevant Files" section:**
   - List every file created or modified.
   - Give each file a one‑line description of its purpose.

3. **Maintain session logs:**
   - After completing a parent task (or significant work session), create/update a session log
   - Logs are stored in: `logi/` (relative to project root)
   - Log filename format: `YYYY_MM_DD_log_<number>.md`
     - `<number>` is the sequential log number for that day (1, 2, 3, etc.)
   - Log content structure:
     ```markdown
     # YYYY_MM_DD_log_<number>
     
     ## Completed Tasks
     
     - [x] Task number and title
     
     ## Task Details
     
     ### Task X.X: Task Title
     
     Brief description (max 5 sentences in English) of what was implemented, key decisions made, files created/modified, and any important notes or considerations for future work.
     ```

## AI Instructions

When working with task lists, the AI must:

1. Regularly update the task list file after finishing any significant work.
2. Follow the completion protocol:
   - Mark each finished **sub‑task** `[x]`.
   - Mark the **parent task** `[x]` once **all** its subtasks are `[x]`.
3. Add newly discovered tasks.
4. Keep "Relevant Files" accurate and up to date.
5. Before starting work, check which sub‑task is next.
6. After implementing a sub‑task, update the file and then pause for user approval.
7. **Parallel task list updates:** When working with bilingual task lists (e.g., `tasks-prd-[project].md` and `tasks-prd-[project]-PL.md`), **always update both files simultaneously** in the same operation. Both files must maintain identical task completion status (`[ ]` or `[x]`) at all times.
   - **Source of truth:** The English version is the primary source of truth for task implementation.
   - **Polish version purpose:** The Polish version serves only as a reference aid for the user to understand what is being implemented at the moment. It should be kept in sync for user convenience, but all implementation decisions are based on the English version.
8. **Session logging:** After completing a parent task or at the end of a significant work session:
   - Create or update a session log in `logi/`
   - Use the naming convention `YYYY_MM_DD_log_<number>.md`
   - Include: completed tasks list and detailed descriptions (max 5 sentences per task)
   - Log content should be in English for consistency
9. **Memory maintenance:** After completing a parent task:
   - Update `memory.md` following the Memory Update Protocol
   - Add completed task to Task History section with all details
   - Update Key Decisions if applicable
   - Update Last Updated date
   - Maintain chronological order

