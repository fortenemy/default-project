# 🚀 Default Project Template

**Version:** 1.0  
**Created:** 2025-10-24  

---

## 📋 What is This?

This is a **universal project template** for AI-driven, structured development. Use it to start any new project with a proven workflow that includes:

- ✅ **PRD-driven development** (Product Requirements Document)
- ✅ **Task-based implementation** (Parent tasks → Subtasks → Execution)
- ✅ **Extended memory system** (Context preservation across sessions)
- ✅ **Bilingual documentation** (English + Polish task lists)
- ✅ **Session logging** (Full traceability of all development decisions)
- ✅ **Self-documenting** (Memory updates automatically after each task)

---

## 🎯 Quick Start

### Step 1: Copy This Template

```bash
# Create a new project from this template
cp -r "D:\projekty AI\Default Project" "D:\projekty AI\YourProjectName"
cd "D:\projekty AI\YourProjectName"
```

### Step 2: Describe Your Project

Open `start.md` and fill in your project details:

- Project name
- Goal
- Core features
- Technology stack
- Constraints
- Success criteria

### Step 3: Begin AI Development Workflow

In your IDE's chat:

```
Use @start.md to initialize the project
```

The AI will guide you through:

1. Creating a PRD
2. Generating task lists
3. Initializing memory
4. Implementing tasks systematically

---

## 📁 Template Structure

```
Default Project/
├── start.md                    # Project initialization guide
├── memory-template.md          # Extended memory template
├── README.md                   # This file
│
├── ai-dev-tasks/              # AI workflow guidelines
│   ├── create-prd.md         # How to create PRD
│   ├── generate-tasks.md     # How to generate tasks
│   ├── process-task-list.md  # How to execute tasks
│   └── README.md             # Workflow documentation
│
├── tasks/                     # (empty) PRD and task lists go here
├── logi/                      # (empty) Session logs go here
│
└── .cursor/
    └── rules/
        └── start.mdc         # Always-active AI initialization rule
```

---

## 🔄 Workflow Overview

### 1. Initialize Project

- Fill in `start.md` with project description
- Mention `@start.md` to AI

### 2. Create PRD

- AI asks clarifying questions
- Generates `tasks/prd-[project-name].md`

### 3. Generate Tasks

- AI creates task list with parent/subtasks
- Saves as `tasks/tasks-prd-[project-name].md` (EN)
- Saves as `tasks/tasks-prd-[project-name]-PL.md` (PL)

### 4. Initialize Memory

- AI creates `memory.md` from template
- Fills in project-specific information

### 5. Execute Tasks

- AI works on tasks one by one
- Updates both task lists simultaneously
- Waits for approval after each subtask
- Updates memory after each parent task
- Creates session logs in `logi/`

---

## 📚 Key Files Explained

### `start.md`

**Purpose:** Main project initialization file  
**When to use:** At the very beginning of a new project  
**Contains:** Project description, goals, features, tech stack

### `memory-template.md`

**Purpose:** Template for project memory  
**Becomes:** `memory.md` (project-specific extended memory)  
**Contains:** Table of Contents, Task History, Configuration, Key Decisions

### `ai-dev-tasks/`

**Purpose:** Contains workflow guidelines for AI  
**Files:**

- `create-prd.md` - PRD creation process
- `generate-tasks.md` - Task list generation
- `process-task-list.md` - Task execution protocol

### `tasks/` (generated)

Will contain:

- `prd-[project-name].md` - Product Requirements Document
- `tasks-prd-[project-name].md` - English task list (source of truth)
- `tasks-prd-[project-name]-PL.md` - Polish task list (reference)

### `logi/` (generated)

Will contain session logs:

- `YYYY_MM_DD_log_1.md` - First session of the day
- `YYYY_MM_DD_log_2.md` - Second session, etc.

### `memory.md` (generated)

Project's extended memory containing:

- Complete task history
- All configuration parameters
- Architectural decisions
- Quick reference commands

---

## ✨ Features

### 🔄 Structured Workflow

From idea → PRD → Tasks → Implementation with clear checkpoints

### 📝 Extended Memory

Context preserved across sessions in `memory.md` with:

- Task history with implementation details
- Configuration reference
- Key decisions and rationale
- Quick reference commands

### 🌐 Bilingual Support

Task lists in both English (source of truth) and Polish (reference)

### 📊 Session Logging

Every development session logged in `logi/` with:

- Completed tasks
- Implementation details
- Key decisions
- Files modified

### 🤖 AI-Ready

`.cursor/rules/start.mdc` automatically initializes AI context

### ✅ Self-Updating

Memory and task lists update automatically as work progresses

---

## 🎯 Example Usage

### Example: E-commerce Website

1. **Copy template** to `EcommerceWebsite/`
2. **Edit start.md:**

   ```markdown
   PROJECT NAME: E-commerce Website
   
   PROJECT GOAL: 
   Create an online store for selling handmade crafts with 
   product catalog, shopping cart, and checkout functionality.
   
   CORE FEATURES:
   1. Product catalog with categories and search
   2. Shopping cart functionality
   3. Checkout with payment integration
   4. User accounts and order history
   5. Admin panel for product management
   
   TECHNOLOGY STACK:
   - Frontend: React + TypeScript
   - Backend: Node.js + Express
   - Database: PostgreSQL
   - Payment: Stripe
   ```

3. **In your IDE:** `Use @start.md to initialize`
4. **AI creates:**
   - `tasks/prd-ecommerce-website.md`
   - `tasks/tasks-prd-ecommerce-website.md`
   - `tasks/tasks-prd-ecommerce-website-PL.md`
   - `memory.md`

5. **Begin implementation:**
   - `Please start on task 1.1 and use @process-task-list.md`
   - Review and approve each subtask
   - AI updates everything automatically

---

## 💡 Best Practices

### ✅ Do

- Fill in `start.md` completely before beginning
- Review each subtask before approving
- Check `memory.md` TOC when resuming work
- Read latest session log to understand context
- Trust the workflow - it's battle-tested

### ❌ Don't

- Skip the PRD creation step
- Jump ahead to tasks without approval
- Manually edit both task lists separately
- Forget to update memory after parent tasks
- Work on multiple parent tasks simultaneously

---

## 🔧 Customization

This template is flexible. Customize:

- PRD sections in `ai-dev-tasks/create-prd.md`
- Task structure in `ai-dev-tasks/generate-tasks.md`
- Memory template sections in `memory-template.md`
- Logging format in `ai-dev-tasks/process-task-list.md`

---

## 📖 Documentation

For the complete methodology, see the original project:

- **Project:** `D:\projekty AI\bitkojnbot\`
- **Memory:** `D:\projekty AI\memory.md`
- **Logs:** `D:\projekty AI\logi\`

---

## 🆘 Troubleshooting

### AI doesn't start workflow

**Solution:** Make sure you mention `@start.md` explicitly

### Task lists out of sync

**Solution:** AI should update both simultaneously. If not, remind: "Update both EN and PL task lists"

### Memory not updating

**Solution:** After completing parent task, explicitly request: "Update memory.md following Memory Update Protocol"

### Lost context after long break

**Solution:** AI should read TOC → Task History → Latest log. If not, mention: "Read @memory.md TOC first"

---

## 🎓 Learning Resources

### First Time Using This?

1. Read `start.md` completely
2. Review `ai-dev-tasks/README.md`
3. Look at `memory-template.md` structure
4. Start with a simple project to learn the workflow

### Understanding the Workflow

- **PRD** = What to build and why
- **Tasks** = How to build it (step by step)
- **Memory** = Persistent project context
- **Logs** = Development history

---

## 🤝 Contributing

Improve this template? Great!

- Suggest enhancements
- Share customizations
- Report issues
- Contribute examples

---

## 📄 License

Free to use and modify for any project.

---

## 🙏 Credits

This AI-driven **default-project**'s workflow was inspired by [**AI Dev Tasks**](https://github.com/snarktank/ai-dev-tasks) by [@snarktank](https://github.com/snarktank) - a proven system for managing AI development agents through structured PRDs, task generation, and systematic task processing. Shout out to Mr.Ryan Carson!

**Methodology designed for:**

- Structured development
- Context preservation
- AI collaboration
- Junior developer friendly
- Production-ready results

---

**Template Version:** 1.0  
**Last Updated:** 2025-10-24  
**Status:** Ready to use 🚀
