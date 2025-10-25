# 🚀 Default Project Template

**Version:**  1.0  
**Created:**  2025-10-24

> 💡 **Quick Start:** Copy this repo template → Start new chat → Add `@init.md` to context → AI asks about your project → AI creates everything!

---

## 📋 What is This?

This is a **universal project template** for AI-driven, structured development. Use it to start any new project with a proven workflow that includes:

- ✅ **PRD-driven development** (Product Requirements Document)
- ✅ **Task-based implementation** (Parent tasks → Subtasks → Execution)
- ✅ **Extended memory system** (Context preservation across sessions)
- ✅ **Session logging** (Full traceability of all development decisions)
- ✅ **Self-documenting** (Memory updates automatically after each task)

---

## 🎯 Quick Start

### Step 1: Copy This Template

Choose one of the following methods to clone the repository:

#### HTTPS

```bash
# Clone the repository
git clone https://github.com/fortenemy/default-project.git YourProjectName
cd YourProjectName
```

#### SSH

```bash
# Clone the repository using SSH
git clone git@github.com:fortenemy/default-project.git YourProjectName
cd YourProjectName
```

#### GitHub CLI

```bash
# Clone the repository using GitHub CLI
gh repo clone fortenemy/default-project YourProjectName
cd YourProjectName
```

#### Use as GitHub Template

1. Visit [https://github.com/fortenemy/default-project](https://github.com/fortenemy/default-project)
2. Click the green "Use this template" button
3. Create a new repository from the template
4. Clone your new repository locally

### Step 2: Initialize Project with AI

1. Open a new chat in your IDE (Cursor/Windsurf/Claude Code, etc.)
2. Add to context: `@init.md`
3. Say: "Initialize this project"

**The AI agent will automatically guide you through project initialization:**

The AI will ask about your project and **automatically create everything you need**:

1. **Create PRD** - AI will use `@create-prd.md` to:
   - Ask you clarifying questions about your project
   - Generate a complete PRD based on your answers
   - Save it as `tasks/prd-[project-name].md`

2. **Generate Tasks** - AI will automatically use `@generate-tasks.md` to:
   - Break down the PRD into parent tasks and subtasks
   - Create detailed task lists
   - Save them in the `tasks/` directory

3. **Initialize Memory** - AI will create `memory.md` from the template with project-specific information

4. **Begin Implementation** - AI will guide you through executing tasks using `@process-task-list.md`

You just need to respond to questions and approve each step - the AI handles the workflow!

---

## 🎬 What to Expect

After you add `@init.md` to context and say "initialize this project", here's what happens:

### Step 1: PRD Creation

Example:

```text
AI: "I'll help you initialize your project. What would you like to build?"
You: "An e-commerce website for handmade crafts"
AI: "Great! Let me ask some clarifying questions..."
You: [Answer questions about features, tech stack, etc.]
AI: "Perfect! I'm generating the PRD now..."
AI: "PRD created and saved at tasks/prd-ecommerce-website.md. Ready for task generation?"
```

### Step 2: Task Generation

```text
You: "Yes, continue"
AI: "Using @generate-tasks.md to analyze PRD and create task breakdown..."
AI: "Task lists created. Now initializing project memory..."
```

### Step 3: Memory Initialization

```text
AI: "Memory (memory.md) initialized with your project details."
AI: "Project structure created. All initialization complete!"
AI: "Ready to start on Task 1.1?"
```

### Step 4: Implementation

```text
You: "Yes, let's start"
AI: [Works on Task 1.1]
AI: "Task 1.1 complete. Please review. Approve to continue?"
You: "yes"
AI: [Moves to Task 1.2 automatically]
```

**That's it!** The AI guides you through everything step by step.

---

## 📁 Template Structure

```text
Default Project/
├── init.md                     # Project initialization guide
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

- Copy the template to your new project directory
- **Start new chat session** and add `@init.md` to context
- Tell AI: "Initialize this project"
- Answer AI's questions about your project

**From this point, the AI agent automatically guides you through all remaining steps:**

### 2. Create PRD (AI-Initiated)

- **AI automatically uses `@create-prd.md`** to guide the process
- AI asks clarifying questions about your project
- You provide answers
- AI generates and saves `tasks/prd-[project-name].md`

### 3. Generate Tasks (AI-Initiated)

- **AI automatically uses `@generate-tasks.md`** after PRD is approved
- AI creates task list with parent/subtasks
- Saves as `tasks/tasks-prd-[project-name].md`

### 4. Initialize Memory (AI-Initiated)

- **AI automatically creates `memory.md`** from template
- Fills in project-specific information from PRD and tasks

### 5. Execute Tasks (AI-Guided)

- **AI uses `@process-task-list.md`** to guide implementation
- AI works on tasks one by one
- Updates task list as work progresses
- Waits for your approval after each subtask
- Updates memory after each parent task
- Creates session logs in `logi/`

> 💡 **You don't need to manually reference the workflow files** - the AI agent knows to use them automatically based on `@init.md` initialization!

---

## 📚 Key Files Explained

### `init.md`

**Purpose:** Main project initialization file  
**When to use:** At the very beginning of a new project  
**Contains:** Instructions for AI to initialize the project through conversation

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
- `tasks-prd-[project-name].md` - Task list with all implementation steps

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
2. **Start new chat with `@init.md`:**

   ```text
   You: "Initialize this project - I want to build an e-commerce website"
   
   AI: "What would you like to build?"
   You: "An e-commerce website for handmade crafts with catalog, cart, and checkout"
   
   AI: "Great! Let me ask about the technical details..."
   AI: "What tech stack do you prefer?"
   You: "React + TypeScript frontend, Node.js + Express backend, PostgreSQL database"
   
   AI: "Any specific requirements or constraints?"
   You: "Need Stripe payment integration, user accounts, and admin panel"
   ```

3. **AI automatically takes over and:**
   - Asks clarifying questions about your e-commerce project
   - You answer the questions
   - AI generates `tasks/prd-ecommerce-website.md`
   - AI automatically creates `tasks/tasks-prd-ecommerce-website.md`
   - AI initializes `memory.md` with your project info
   - AI asks: "Ready to start on task 1.1?"

4. **You just:**
   - Approve to continue
   - Review each completed subtask
   - Say "yes" to move to the next
   - AI handles all the rest (updates, logs, memory)

---

## 💡 Best Practices

### ✅ Do

- **Always add `@init.md` to context at the start of new chat**
- Answer AI's questions thoroughly during initialization
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

**GitHub Repository:** [https://github.com/fortenemy/default-project](https://github.com/fortenemy/default-project)

This template's methodology was developed and proven on real-world projects.

---

## 🆘 Troubleshooting

### AI doesn't start workflow

**Solution:**

- Make sure you **added `@init.md` to the chat context** (not just mentioned it in text)
- Start a fresh chat session
- Say clearly: "Initialize this project" or "Help me initialize this project"

### Task list not updating

**Solution:** AI should mark tasks as complete after each subtask. If not, remind: "Update task list to mark completed items"

### Memory not updating

**Solution:** After completing parent task, explicitly request: "Update memory.md following Memory Update Protocol"

### Lost context after long break

**Solution:** AI should read TOC → Task History → Latest log. If not, mention: "Read @memory.md TOC first"

---

## 🎓 Learning Resources

### First Time Using This?

1. Read `init.md` to understand the initialization process
2. Copy the template to your project directory
3. **Start new chat and add `@init.md` to context**
4. Review `ai-dev-tasks/README.md` for workflow details
5. Look at `memory-template.md` structure
6. Start with a simple project to learn the workflow

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

This project is licensed under the **Apache License 2.0** - see the [LICENSE.md](LICENSE.md) file for details.

### What This Means

You are free to:
- ✅ Use this template for commercial or personal projects
- ✅ Modify and adapt it to your needs
- ✅ Distribute and share it
- ✅ Create derivative works

**Requirements:**
- Include a copy of the Apache 2.0 license
- State significant changes made to the original files
- Preserve copyright and attribution notices

### Attribution

The AI workflow methodology (`ai-dev-tasks/` directory) is adapted from [AI Dev Tasks](https://github.com/snarktank/ai-dev-tasks) by [@snarktank](https://github.com/snarktank), also licensed under Apache 2.0.

***~ credits to @snarktank !***

**Methodology designed for:**

- Structured development
- Context preservation
- AI collaboration
- Junior developer friendly
- Production-ready results

---

**Template Version:** 1.0  
**Last Updated:** 2025-10-24

---
**Designed by** ***fortenemy***
