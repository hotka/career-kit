# CareerKit

Collection of instruments for job searching.

## Project Goal

Preparation for a new job as **Middle+/Senior Frontend Developer**:

- Master resume preparation
- Tailored resumes for specific job postings
- Mock interviews with knowledge gap filling
- LinkedIn profile analysis and optimization

---

## MCP Tools

Prefer MCP tools over built-in when available:

| Task             | Prefer                                                                                | Instead of            |
| ---------------- | ------------------------------------------------------------------------------------- | --------------------- |
| Read/edit files  | `mcp__jetbrains__get_file_text_by_path`, `mcp__jetbrains__replace_text_in_file`       | Read, Edit            |
| Create files     | `mcp__jetbrains__create_new_file`                                                     | Write                 |
| Search in files  | `mcp__jetbrains__search_in_files_by_text`, `mcp__jetbrains__search_in_files_by_regex` | Grep                  |
| Find files       | `mcp__jetbrains__find_files_by_name_keyword`, `mcp__jetbrains__find_files_by_glob`    | Glob                  |
| Directory tree   | `mcp__jetbrains__list_directory_tree`                                                 | Bash ls               |
| File diagnostics | `mcp__jetbrains__get_file_problems`                                                   | Manual inspection     |
| Format file      | `mcp__jetbrains__reformat_file`                                                       | Bash prettier/eslint  |
| Rename symbol    | `mcp__jetbrains__rename_refactoring`                                                  | Manual find & replace |
| Symbol info      | `mcp__jetbrains__get_symbol_info`                                                     | Reading source code   |
| Run terminal     | `mcp__jetbrains__execute_terminal_command`                                            | Bash                  |
| Open in IDE      | `mcp__jetbrains__open_file_in_editor`                                                 | —                     |
**Why?** MCP tools integrate with IDE, provide better context, and respect project settings.

---

## Skills (Detailed Guides)

Skills are located in `.claude/skills/`. **Load multiple skills together** for complex tasks.

### Skill Reference

| Skill                   | Contains                                                                                                                   |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| `career-biographer`     | Career data collection: conducts interviews, extracts structured data (CareerProfile) for use by other skills              |
| `cv-creator`            | Resume creation: transforms CareerProfile into ATS-optimized resumes (PDF, DOCX, LaTeX, JSON Resume, HTML, Markdown)       |
| `linkedin-optimizer`    | LinkedIn optimization: profile analysis, completion checklists, Headline/About writing, networking strategy                |
| `interview-master`      | Interview preparation: question generation, mock interviews, preparation roadmaps                                          |
| `job-search-strategist` | Job search strategy: job posting analysis, skills-matching, skill gap identification, personalized application strategies  |
| `leetcode-teacher`      | Technical interview prep: interactive LeetCode-style challenges, 20 algorithm patterns                                    |
| `create-skill`          | Meta-skill: creating new Agent Skills (SKILL.md files)                                                                     |

### Skill Usage Chain

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                          JOB SEARCH PREPARATION                             │
└─────────────────────────────────────────────────────────────────────────────┘

1. DATA COLLECTION
   ┌──────────────────┐
   │ career-biographer │ → Career interview → CareerProfile (JSON)
   └──────────────────┘

2. DOCUMENT CREATION
   ┌──────────────────┐
   │ cv-creator       │ → CareerProfile → Master resume (ATS-optimized)
   └──────────────────┘
   ┌──────────────────┐
   │ linkedin-optimizer │ → Profile analysis → Optimized LinkedIn
   └──────────────────┘

3. SEARCH STRATEGY
   ┌──────────────────────┐
   │ job-search-strategist │ → Job posting analysis → Tailored resume + application strategy
   └──────────────────────┘

4. INTERVIEW PREPARATION
   ┌──────────────────┐     ┌──────────────────┐
   │ interview-master │  +  │ leetcode-teacher │
   └──────────────────┘     └──────────────────┘
           │                         │
           ▼                         ▼
   Mock interviews           Algorithms and
   (behavioral,              data structures
    system design)
```

**Typical workflow:**
1. `career-biographer` — collect career data through interview
2. `cv-creator` — create master resume from collected data
3. `linkedin-optimizer` — optimize LinkedIn profile
4. `job-search-strategist` — analyze job posting and tailor resume
5. `interview-master` + `leetcode-teacher` — prepare for interviews

### Example Commands

```bash
# 1. Career interview — collect structured career data
/career-biographer

# 2. Create master resume from career profile
/cv-creator Create a master resume using drafts/career-profile.json

# 3. Tailor resume for a specific job posting
/job-search-strategist Analyze this job posting and tailor my resume: <URL or pasted text>

# 4. Optimize LinkedIn profile
/linkedin-optimizer Review my LinkedIn profile and suggest improvements

# 5. Mock behavioral interview
/interview-master Conduct a behavioral mock interview for a Senior Frontend Developer role

# 6. Mock system design interview
/interview-master Conduct a system design mock interview for a Senior Frontend Developer role

# 7. Practice algorithms (interactive)
/leetcode-teacher Start a session on Two Pointers pattern in TypeScript

# 8. Generate PDF from markdown resume
npx md-to-pdf drafts/resume-senior-frontend.md
```