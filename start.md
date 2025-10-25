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
- ✅ Bilingual documentation (EN/PL)
- ✅ Session logging for full traceability
- ✅ Self-documenting and self-updating

---

## 🎯 How to Use This Template

### Step 1: Copy This Template

```bash
# Create a new project from this template
cp -r "D:\projekty AI\Default Project" "D:\projekty AI\[YOUR_PROJECT_NAME]"
cd "D:\projekty AI\[YOUR_PROJECT_NAME]"
```

### Step 2: Describe Your Project

**Fill in the following information:**

```markdown
PROJECT NAME: [e.g., Company X Website, Task Manager App, Trading Bot, etc.]

PROJECT GOAL: 
[What do you want to build? What problem does it solve? Who is the target user?]

CORE FEATURES:
1. [Feature 1]
2. [Feature 2]
3. [Feature 3]
...

TECHNOLOGY STACK:
- [e.g., Python, React, Node.js, etc.]

CONSTRAINTS:
- [e.g., Budget, Timeline, Platform requirements, etc.]

SUCCESS CRITERIA:
- [How do you measure if the project is successful?]
```

### Step 3: Start the AI-Driven Process

Once you've described your project above, the AI agent will:

1. **Create PRD (Product Requirements Document)**
   - Using `ai-dev-tasks/create-prd.md` as a guide
   - Document will be saved in `tasks/prd-[project-name].md`

2. **Generate Task List**
   - Using `ai-dev-tasks/generate-tasks.md` as a guide
   - Parent tasks + subtasks breakdown
   - Saved in `tasks/tasks-prd-[project-name].md` (EN)
   - Saved in `tasks/tasks-prd-[project-name]-PL.md` (PL)

3. **Initialize Memory**
   - Create `memory.md` from `memory-template.md`
   - Fill in project-specific information
   - Set up tracking systems

4. **Begin Implementation**
   - Follow `ai-dev-tasks/process-task-list.md`
   - Execute tasks one by one
   - Update task lists (EN + PL simultaneously)
   - Update memory.md after each parent task
   - Create session logs in `logi/`

---

## 📚 Template Contents

This template includes:

### Core Files

- ✅ **start.md** (this file) - Project initialization guide
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

When an AI agent reads this file in a new project context:

### Initialization Checklist

- [ ] 1. Read the project description filled in by the user above
- [ ] 2. Confirm understanding of the project goal
- [ ] 3. Ask clarifying questions if needed
- [ ] 4. Propose to create PRD using `@ai-dev-tasks/create-prd.md`
- [ ] 5. Once PRD is approved, generate task list using `@ai-dev-tasks/generate-tasks.md`
- [ ] 6. Initialize `memory.md` from `@memory-template.md`
- [ ] 7. Begin task execution using `@ai-dev-tasks/process-task-list.md`

### Ongoing Work Protocol

Follow these principles throughout the project:

1. **Task Lists:** Always update both EN and PL versions simultaneously
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

```markdown
PROJECT NAME: Acme Corp Website

PROJECT GOAL: 
Create a modern, responsive corporate website for Acme Corp that showcases 
products, company history, and contact information. Target users are potential 
B2B clients looking for manufacturing partners.

CORE FEATURES:
1. Homepage with hero section and value propositions
2. Products catalog with filtering and search
3. About Us page with company history and team
4. Contact form with email integration
5. Blog section for company news
6. Responsive design (mobile-first)

TECHNOLOGY STACK:
- Frontend: React + TypeScript
- Styling: Tailwind CSS
- Backend: Node.js + Express (API)
- Database: PostgreSQL
- Hosting: Vercel (frontend) + Railway (backend)

CONSTRAINTS:
- Budget: $5,000
- Timeline: 6 weeks
- Must be SEO-optimized
- WCAG 2.1 AA accessibility compliance

SUCCESS CRITERIA:
- Page load time < 2 seconds
- Mobile responsive on all devices
- 90+ Lighthouse score
- Contact form with 99% uptime
- Blog management system operational
```

After filling this in, the AI agent will:

1. Create `tasks/prd-acme-website.md`
2. Generate `tasks/tasks-prd-acme-website.md` (EN) and `tasks/tasks-prd-acme-website-PL.md` (PL)
3. Initialize `memory.md` with project-specific information
4. Begin implementing tasks systematically

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

For complete documentation on this methodology, see:

- Original project: `D:\projekty AI\bitkojnbot\`
- Original memory: `D:\projekty AI\memory.md`
- Original logs: `D:\projekty AI\logi\`

---

## 🙏 Credits

This template's AI-driven workflow is inspired by the excellent [**AI Dev Tasks**](https://github.com/snarktank/ai-dev-tasks) repository by [@snarktank](https://github.com/snarktank). The structured approach to PRD creation, task generation, and systematic task processing is based on their proven methodology for managing AI development agents.

**Shout out to the original ai-dev-tasks workflow:** <https://github.com/snarktank/ai-dev-tasks>

---

## 🎬 Ready to Start?

**Delete this section and fill in your project details above, then mention this file to the AI agent to begin!**

---

**Template Version:**  1.0  
**Last Updated:**  2025-10-24  
**Author:**  *fortenemy*
