# 🚀 Project Initialization Guide

**Default Project** Template v1.0  
**Created:**  2025-10-24  
**Author:**  *fortenemy*

---

## 📋 What is This?

This is a **universal project template** that helps you start any new project using a proven, structured approach:

- ✅ AI-driven development workflow
- ✅ Task-based implementation (PRD → Tasks → Execution)
- ✅ Extended memory system for context preservation
- ✅ Session logging for full traceability
- ✅ Self-documenting and self-updating

---

## 🎯 How to Use This Template

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

### Step 2: Initialize with AI

**Start AI-driven initialization process:**

1. Open a new chat session in your IDE (Cursor/Windsurf/Claude Code)
2. Add this file to context by typing: `@init.md`
3. Tell the AI: "Initialize this project" or "Help me initialize this project"

**The AI will ask you about your project and then automatically:**

### STEP 1: Ask About Your Project

- AI asks: "What would you like to build?"
- You describe your project idea
- AI asks clarifying questions about features, users, goals

### STEP 2: Create PRD (using `@ai-dev-tasks/create-prd.md`)

- AI asks detailed questions about requirements
- You provide answers
- AI generates complete PRD document
- Saved as `tasks/prd-[project-name].md`

### STEP 3: Generate Tasks (using `@ai-dev-tasks/generate-tasks.md`)

- AI analyzes the PRD
- AI creates parent tasks and subtasks
- AI generates detailed task list
- Saved as `tasks/tasks-prd-[project-name].md`

### STEP 4: Initialize Memory

- AI creates `memory.md` from `@memory-template.md`
- Fills in project-specific information from PRD
- Sets up tracking systems

### STEP 5: Create Project Structure

- Ensures `tasks/` directory exists
- Ensures `logi/` directory exists
- Verifies `.cursor/rules/start.mdc` is in place

### STEP 6: Ready for Implementation

- AI confirms: "All initialization complete!"
- AI asks: "Ready to start on Task 1.1?"
- From here, use `@ai-dev-tasks/process-task-list.md` for implementation

**You don't need to manually reference workflow files** - just add `@init.md` to context and let the AI guide you!

---

## 📚 Template Contents

This template includes:

### Core Files

- ✅ **init.md** (this file) - Project initialization guide
- ✅ **memory-template.md** - Extended memory template
- ✅ **README.md** - Template documentation

### AI Dev Tasks (`ai-dev-tasks/`)

- ✅ **create-prd.md** - How to create a Product Requirements Document
- ✅ **generate-tasks.md** - How to generate a task list from PRD
- ✅ **process-task-list.md** - How to execute tasks systematically
- ✅ **README.md** - Workflow overview

### Empty Directories (Ready for Your Project)

- 📁 **tasks/** - Will contain PRD and task lists
- 📁 **logi/** - Will contain session logs (`YYYY_MM_DD_log_N.md`)
- 📁 **.cursor/rules/** - Contains `start.mdc` (always-active rule)

---

## 🤖 AI Agent Instructions

When an AI agent reads this file, **automatically initiate the project initialization workflow:**

### Initialization Protocol

**You (AI Agent) must guide the user through project initialization by following these steps:**

- [ ] **STEP 1: Discover the Project**
  - Ask: "What would you like to build?"
  - Ask clarifying questions about the project idea
  - Understand the problem, users, and goals

- [ ] **STEP 2: Create PRD** (use `@ai-dev-tasks/create-prd.md`)
  - Follow create-prd.md instructions to ask detailed questions
  - Generate comprehensive PRD based on user's answers
  - Save as `tasks/prd-[project-name].md`
  - Confirm with user: "PRD created. Ready for task generation?"

- [ ] **STEP 3: Generate Task Lists** (use `@ai-dev-tasks/generate-tasks.md`)
  - Analyze the PRD you just created
  - Generate parent tasks (wait for user "Go" confirmation)
  - Generate all subtasks
  - Save as: `tasks/tasks-prd-[project-name].md`

- [ ] **STEP 4: Initialize Memory** (use `@memory-template.md`)
  - Create `memory.md` from the template
  - Fill in all sections with project-specific information from PRD
  - Include task history, configuration, architecture details

- [ ] **STEP 5: Verify Structure**
  - Ensure `tasks/` directory exists with PRD and task lists
  - Ensure `logi/` directory exists (empty, ready for logs)
  - Verify `.cursor/rules/start.mdc` exists (should already be there)

- [ ] **STEP 6: Confirm Completion**
  - Tell user: "✅ Project initialization complete!"
  - Summarize what was created:
    - PRD document
    - Task list
    - Memory file
    - Project structure
  - Ask: "Ready to start on Task 1.1?"

**Important Notes:**

- User should NOT need to manually reference workflow files - you handle this automatically
- Follow each step in sequence - don't skip steps
- Wait for user approval before moving between major phases (PRD → Tasks → Implementation)

### Ongoing Work Protocol

Follow these principles throughout the project:

1. **Task List:** Update task list after completing each subtask
2. **Memory:** Update `memory.md` after completing each parent task
3. **Logging:** Create session logs after each parent task
4. **Verification:** Check memory.md TOC before starting work
5. **Consistency:** Maintain the same standards as the original project

### Quick Links to Guidelines

- How to create PRD: `@ai-dev-tasks/create-prd.md`
- How to generate tasks: `@ai-dev-tasks/generate-tasks.md`
- How to process tasks: `@ai-dev-tasks/process-task-list.md`
- Memory structure: `@memory-template.md`

---

## ✨ Example Usage

### Example: Company Website Project

**User adds `@init.md` to chat and says:**

```text
"Initialize this project"
```

**AI conversation:**

```text
AI: "I'll help you initialize your project. What would you like to build?"

You: "A modern corporate website for Acme Corp"

AI: "Great! What's the main goal of this website?"

You: "Showcase products, company history, and contact info for potential B2B clients"

AI: "What are the core features you need?"

You: "Homepage with hero, products catalog with filtering, about us page, 
     contact form, blog section, all mobile-first responsive"

AI: "What technology stack do you prefer?"

You: "React + TypeScript frontend, Tailwind CSS, Node.js + Express backend, 
     PostgreSQL database, hosted on Vercel and Railway"

AI: "Any specific constraints or requirements?"

You: "Budget $5,000, 6 weeks timeline, must be SEO-optimized, WCAG 2.1 AA compliant"

AI: "Perfect! I'm now generating the PRD..."
AI: "✅ PRD created at tasks/prd-acme-website.md"
AI: "Ready to generate task lists?"

You: "Yes, continue"

AI: "Analyzing PRD and generating tasks..."
AI: "✅ Task list created: tasks/tasks-prd-acme-website.md"
AI: "Initializing project memory..."
AI: "✅ memory.md created with your project info"
AI: "✅ Project structure verified"
AI: ""
AI: "🎉 All initialization complete!"
AI: "Ready to start on Task 1.1?"
```

---

## 🔧 Customization

Feel free to customize this template for your needs:

- Add/remove sections in `memory-template.md`
- Modify task generation templates in `ai-dev-tasks/`
- Adjust logging formats in `process-task-list.md`
- Create project-specific guidelines

The template is designed to be flexible while maintaining structure.

---

## 📖 Documentation

**GitHub Repository:** [https://github.com/fortenemy/default-project](https://github.com/fortenemy/default-project)

This template's methodology was developed and proven on real-world projects, including a Bitcoin Trading Bot MVP that served as the foundation for this structured approach.

---

## 🙏 Credits

This template's AI-driven workflow is inspired by the excellent [**AI Dev Tasks**](https://github.com/snarktank/ai-dev-tasks) repository by [@snarktank](https://github.com/snarktank). The structured approach to PRD creation, task generation, and systematic task processing is based on their proven methodology for managing AI development agents.

**Shout out to the original ai-dev-tasks workflow:** <https://github.com/snarktank/ai-dev-tasks>

---

## 🎬 Ready to Initialize?

**To start project initialization:**

1. **Start a new chat session** in your IDE
2. **Add this file to context:** `@init.md`
3. **Tell the AI:** "Initialize this project" or "Help me initialize this project"

The AI will ask about your project and automatically create everything you need!

---

**Note:** This is a template file - no need to edit it. The AI will gather all information through conversation.

---

**Template Version:**  1.0  
**Last Updated:**  2025-10-24  
**Author:**  *fortenemy*
