# [PROJECT_NAME] - Extended Memory

**Project Root:** `[PATH_TO_PROJECT_ROOT]`  
**Documentation Root:** `[PATH_TO_DOCUMENTATION]`  
**Logs Directory:** `[PATH_TO_LOGS]`  
**Project Initialized:** [YYYY-MM-DD]  
**Last Updated:** [YYYY-MM-DD]

---

## Table of Contents

**→ [How to Use This Memory (AI Instructions)](#how-to-use-this-memory-ai-instructions) ← START HERE**

1. [Project Overview](#project-overview)
   - [Goal](#goal)
   - [Target User](#target-user)
   - [Core Functionality](#core-functionality)
   - [Non-Goals](#non-goals)
   - [Acceptance Criteria](#acceptance-criteria)

2. [Project Setup](#project-setup)
   - [Environment](#environment)
   - [Required Accounts/APIs](#required-accountsapis)
   - [Dependencies](#dependencies)
   - [Configuration](#configuration)

3. [Architecture](#architecture)
   - [Directory Structure](#directory-structure)
   - [Module Dependencies](#module-dependencies)

4. [Development Workflow](#development-workflow)
   - [Task Management](#task-management)
   - [Workflow Protocol](#workflow-protocol)
   - [Logging System](#logging-system)
   - [Version Control](#version-control)

5. [Task History](#task-history)
   - [Task 1.0: ...](#task-10-...)

6. [Configuration Reference](#configuration-reference)
   - [Main Parameters](#main-parameters)
   - [Feature Flags](#feature-flags)
   - [Environment Variables](#environment-variables)

7. [Key Decisions](#key-decisions)
   - [1. ...](#1-...)

8. [Future Considerations](#future-considerations)
   - [Next Phase Enhancements](#next-phase-enhancements)
   - [Technical Debt](#technical-debt)
   - [Monitoring & Observability](#monitoring--observability)

9. [Memory Update Protocol](#memory-update-protocol)
   - [When to Update](#when-to-update-memorymd)
   - [Update Procedure](#update-procedure)
   - [Quick Update Checklist](#quick-update-checklist)
   - [Maintenance Guidelines](#maintenance-guidelines)
   - [Self-Check Questions](#self-check-questions)

10. [Quick Reference](#quick-reference)
    - [Running the Project](#running-the-project)
    - [Running Tests](#running-tests)
    - [Common Commands](#common-commands)
    - [Check Task Progress](#check-task-progress)
    - [View Session Logs](#view-session-logs)

---

## How to Use This Memory (AI Instructions)

### For AI Agent Reading This File

**CRITICAL: Always start with the Table of Contents above.**

When accessing this memory file:

1. **First Action: Read Table of Contents**
   - TOC is your navigation hub - it shows ALL available information
   - Identify which section(s) contain the information you need
   - Use direct links to jump to specific sections

2. **Information Lookup Strategy:**
   - **Need current task status?** → [Task History](#task-history)
   - **Need configuration values?** → [Configuration Reference](#configuration-reference)
   - **Need to understand architecture?** → [Architecture](#architecture)
   - **Need to know workflow?** → [Development Workflow](#development-workflow)
   - **Need decision rationale?** → [Key Decisions](#key-decisions)
   - **Need to update memory?** → [Memory Update Protocol](#memory-update-protocol)
   - **Need quick commands?** → [Quick Reference](#quick-reference)

3. **Before Starting Any Task:**
   - Check [Task History](#task-history) for what's been completed
   - Review [Key Decisions](#key-decisions) for relevant context
   - Verify current [Configuration Reference](#configuration-reference)
   - Follow [Workflow Protocol](#workflow-protocol)

4. **After Completing Any Parent Task:**
   - **MUST** update this file following [Memory Update Protocol](#memory-update-protocol)
   - Update [Task History](#task-history) with new completed task
   - Update [Table of Contents](#table-of-contents) with new task link
   - Update [Key Decisions](#key-decisions) if applicable

5. **Context Recovery:**
   - If returning after context window reset, read:
     1. [Table of Contents](#table-of-contents) (orientation)
     2. [Task History](#task-history) (what's done)
     3. Latest entry in Task History (current state)
     4. [Quick Reference](#quick-reference) (commands)

6. **Never Assume - Always Verify:**
   - Don't assume configuration values - check [Configuration Reference](#configuration-reference)
   - Don't assume architecture - check [Architecture](#architecture)
   - Don't assume decisions - check [Key Decisions](#key-decisions)
   - When in doubt, consult TOC first

### Memory File Purpose

This file serves as the **single source of truth** for:

- ✅ Project goals and requirements
- ✅ Complete task history with implementation details
- ✅ All configuration parameters
- ✅ Architectural decisions and rationale
- ✅ Development workflow and protocols
- ✅ Quick reference for common operations

**Always prefer information from this file over assumptions or partial memory.**

---

## Project Overview

### Goal

[Describe the main goal of the project. What problem does it solve? What value does it provide?]

**Example:**
> Build a responsive corporate website that showcases products and services, provides company information, and enables client contact through forms and chat.

### Target User

**Primary:** [Who is the main user of this project?]

**Secondary (optional):** [Any secondary user groups?]

**Example:**

> - **Primary:** Potential B2B clients looking for manufacturing partners
> - **Secondary:** Job seekers researching the company

### Core Functionality

[List the core features that must be present in the project]

**Example:**

1. Homepage with hero section and value propositions
2. Products catalog with filtering and search
3. Company history and team information
4. Contact form with email integration
5. Responsive design (mobile-first approach)

### Non-Goals

[What is explicitly NOT in scope for this project?]

**Example:**

- ❌ E-commerce functionality (no shopping cart)
- ❌ User authentication system
- ❌ Multi-language support (MVP in English only)
- ❌ Advanced analytics dashboard

### Acceptance Criteria

**Operational Requirements:**
[Technical requirements for project completion]

**Example:**

- Page load time < 2 seconds
- Mobile responsive on all screen sizes
- 90+ Lighthouse score
- WCAG 2.1 AA accessibility compliance

**Functional Requirements:**
[Feature completeness criteria]

**Example:**

- All pages accessible and functional
- Contact form delivers emails reliably
- Navigation works on all devices

---

## Project Setup

### Environment

- **Language/Runtime:** [e.g., Python 3.13, Node.js 20, etc.]
- **Development Environment:** [e.g., VS Code, Cursor, Windsurf, etc.]
- **OS:** [e.g., Windows 11, macOS, Linux]
- **Version Control:** [e.g., Git + GitHub]

### Required Accounts/APIs

[List any external services needed]

**Example:**

1. **Hosting Provider** - Vercel, Railway, AWS, etc.
2. **Email Service** - SendGrid, Mailgun, etc.
3. **Analytics** - Google Analytics, Plausible, etc.

### Dependencies

[List main dependencies with versions]

**Example:**

```
react==18.2.0
typescript==5.0.0
tailwindcss==3.3.0
express==4.18.2
postgresql==3.4.1
```

### Configuration

[Key configuration files and their purpose]

**Example:**

- `.env` - Environment variables (API keys, secrets)
- `config.json` - Application configuration
- `database.yml` - Database connection settings

---

## Architecture

### Directory Structure

[Document the project's directory layout]

**Example:**

```
project-name/
├── src/
│   ├── components/     # React components
│   ├── pages/         # Page components
│   ├── api/           # API routes
│   ├── styles/        # CSS/SCSS files
│   └── utils/         # Utility functions
├── public/            # Static assets
├── tests/             # Test files
├── docs/              # Documentation
└── config/            # Configuration files
```

### Module Dependencies

[Document how modules/components interact]

**Example:**

```
App
  ├─> Router
  │     ├─> HomePage
  │     ├─> ProductsPage
  │     │     └─> ProductCard
  │     ├─> AboutPage
  │     └─> ContactPage
  │           └─> ContactForm
  └─> GlobalStyles
```

---

## Development Workflow

### Task Management

- **Task List:** `tasks/tasks-prd-[project-name].md` (implementation roadmap)
- **Process Guidelines:** `ai-dev-tasks/process-task-list.md`

### Workflow Protocol

1. Read next sub-task from task list
2. Implement the sub-task
3. **Update both task lists simultaneously** (mark `[x]`)
4. Test implementation (if applicable)
5. Update session log after completing parent task
6. **Update memory.md** (see [Memory Update Protocol](#memory-update-protocol))
7. Proceed to next sub-task (or wait for user approval)

### Logging System

**Session Logs Location:** `logi/`

**Naming Convention:** `YYYY_MM_DD_log_<number>.md`

- `<number>` = sequential log number for that day (1, 2, 3...)

**Log Structure:**

```markdown
# YYYY_MM_DD_log_<number>

## Completed Tasks
- [x] Task X.X: Title

## Task Details
### Task X.X: Title
Description (max 5 sentences per task)
```

**When to Create Logs:**

- After completing a parent task
- At the end of a significant work session

### Version Control

- **.gitignore:** Exclude sensitive files, dependencies, build artifacts
- **Never commit:** API keys, secrets, credentials, personal data

---

## Task History

### Task 1.0: [First Task Title] ✅

**Status:** [PENDING / IN_PROGRESS / COMPLETED]  
**Date:** [YYYY-MM-DD]  
**Log:** `logi/YYYY_MM_DD_log_<number>.md`

#### Subtasks Completed

- [ ] 1.1 [Subtask description]
- [ ] 1.2 [Subtask description]
- [ ] 1.3 [Subtask description]

#### Files Created/Modified

1. **filename** - Description
2. **another-file** - Description

#### Key Implementation Details

**1.1 [Subtask Title]:**

- Implementation notes
- Key decisions made
- Important considerations

#### Statistics

- **Files Created/Modified:** X files
- **Lines of Code:** ~XXX lines
- **Completion:** XX% (X/X subtasks)
- **Next:** Task 2.0 ([Next task title])

---

## Configuration Reference

### Main Parameters

| Parameter | Value | Description |
|-----------|-------|-------------|
| [PARAM_NAME] | [value] | [what it does] |

### Feature Flags

| Flag | Status | Description |
|------|--------|-------------|
| [FEATURE_NAME] | Enabled/Disabled | [purpose] |

### Environment Variables

| Variable | Required | Description |
|----------|----------|-------------|
| [VAR_NAME] | Yes/No | [what it's for] |

---

## Key Decisions

### 1. [Decision Title]

**Decision:** [Clear statement of what was decided]  
**Rationale:** [Why this decision was made]  
**Alternatives Considered:** [What else was considered]  
**Impact:** [What this affects]  
**Source:** [Where this came from]

---

## Future Considerations

### Next Phase Enhancements

[Features to add after MVP is complete]

### Technical Debt

[Known issues or improvements needed]

### Monitoring & Observability

[Metrics, logging, monitoring to add]

---

## Memory Update Protocol

### When to Update Memory.md

This file **MUST** be updated after:

1. ✅ Completing any parent task
2. ✅ Making significant architectural decisions
3. ✅ Adding/modifying configuration parameters
4. ✅ Discovering new requirements or constraints
5. ✅ At the end of each development session (if substantial work was done)

### Update Procedure

When updating `memory.md`, follow this protocol:

#### 1. Update Header Metadata

```markdown
**Last Updated:** YYYY-MM-DD

```

- Always update the date at the top of the file

#### 2. Add New Task to Task History

After completing a parent task, add a new section following this template:

```markdown
### Task X.0: [Task Title] ✅
**Status:** COMPLETED  
**Date:** YYYY-MM-DD  
**Log:** `logi/YYYY_MM_DD_log_<number>.md`

#### Subtasks Completed:
- ✅ X.1 [Subtask description]
- ✅ X.2 [Subtask description]
...

#### Files Created/Modified:
1. **filename** - Brief description
...

#### Key Implementation Details:

**X.1 [Subtask Title]:**
- Bullet points describing implementation
...

#### Statistics:
- **Files Created/Modified:** X files
- **Lines of Code:** ~XXX lines
- **Completion:** 100% (X/X subtasks)
- **Next:** Task Y.0 ([Next task title])
```

**Important:** Also update the Table of Contents with the new task link.

#### 3. Update Key Decisions (If Applicable)

If the completed task involved important decisions, add them to "Key Decisions" section.

#### 4. Update Configuration Reference (If Applicable)

If new configuration parameters were added or modified, update the relevant tables.

#### 5. Update Architecture (If Applicable)

If structure changed, update "Directory Structure" and "Module Dependencies".

#### 6. Update Dependencies (If Applicable)

If new packages were added, update the "Dependencies" section.

### Quick Update Checklist

- [ ] Update "Last Updated" date at top of file
- [ ] Update "Table of Contents" - add new task link
- [ ] Add new Task X.0 section to "Task History"
  - [ ] Include all subtasks
  - [ ] List all files created/modified
  - [ ] Document implementation details
  - [ ] Add statistics
  - [ ] Note next task
- [ ] Update "Key Decisions" if applicable
- [ ] Update "Configuration Reference" if applicable
- [ ] Update "Architecture" if applicable
- [ ] Ensure chronological order in Task History

### Maintenance Guidelines

1. **Chronological Order:** Maintain chronological order in Task History
2. **Consistency:** Keep formatting consistent across entries
3. **Completeness:** Don't skip tasks - every parent task gets an entry
4. **Accuracy:** Cross-reference with actual code and logs
5. **Clarity:** Use clear, concise language (max 5 sentences per subtask)
6. **Links:** Reference session logs correctly

### Self-Check Questions

Before considering the memory update complete:

- ✅ Is the date at the top current?
- ✅ Is the Table of Contents updated?
- ✅ Is the new task fully documented?
- ✅ Are all subtasks listed with checkmarks?
- ✅ Are all files listed?
- ✅ Are implementation details clear?
- ✅ Are statistics accurate?
- ✅ Is the session log referenced correctly?
- ✅ Do all TOC links work?

---

## Quick Reference

### Running the Project

```bash
# [Add project-specific commands]
cd [project-path]
[start command]
```

### Running Tests

```bash
# [Add testing commands]
[test command]
```

### Common Commands

```bash
# [Add frequently used commands]
```

### Check Task Progress

- Task list: `tasks/tasks-prd-[project-name].md`

### View Session Logs

- Directory: `logi/`
- Latest: Check highest number for today's date

---

**End of Memory Document**  
**Next Task:** [Task number and title]

---

**Designed by** ***fortenemy***
