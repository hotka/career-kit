# CareerKit

A set of [Claude Code Skills](https://docs.anthropic.com/en/docs/claude-code/skills) that help with job searching — from collecting career data to generating tailored resumes, preparing for interviews, and optimizing your LinkedIn profile.

## Acknowledgments

Skills are based on templates from [SkillsMP](https://skillsmp.com/) and incorporate materials from the              
[HelloNewJob](https://hellonewjob.org/) career course by Kira Kuzmenko.

## Available Skills

| Skill | Description |
|-------|-------------|
| **career-biographer** | Conducts a structured career interview and extracts a CareerProfile (JSON) used by other skills |
| **cv-creator** | Transforms CareerProfile into ATS-optimized resumes in multiple formats (PDF, DOCX, LaTeX, JSON Resume, HTML, Markdown) |
| **linkedin-optimizer** | Analyzes and optimizes LinkedIn profiles — Headline, About, Experience, Skills, networking strategy |
| **job-search-strategist** | Analyzes job postings, matches skills, identifies gaps, and builds personalized application strategies |
| **interview-master** | Generates interview questions, runs mock interviews (behavioral, system design), and creates preparation roadmaps |
| **leetcode-teacher** | Interactive LeetCode-style practice with 20 algorithm patterns in Python, TypeScript, Kotlin, and Swift |

## Workflow

```
career-biographer → cv-creator → linkedin-optimizer → job-search-strategist → interview-master + leetcode-teacher
```

1. **Collect** career data through a guided interview
2. **Create** a master resume from structured career profile
3. **Optimize** LinkedIn profile to match your resume
4. **Tailor** resume and strategy for specific job postings
5. **Prepare** for interviews with mock sessions and algorithm practice

## Usage

Skills are invoked as slash commands in Claude Code:

```bash
# Career interview
/career-biographer

# Create master resume
/cv-creator Create a master resume using drafts/career-profile.json

# Tailor resume for a job posting
/job-search-strategist Analyze this job posting and tailor my resume: <URL or text>

# Optimize LinkedIn
/linkedin-optimizer Review my LinkedIn profile and suggest improvements

# Mock interview
/interview-master Conduct a behavioral mock interview for a Senior Frontend Developer role

# Algorithm practice
/leetcode-teacher Start a session on Two Pointers pattern in TypeScript
```

## Setup

1. Install [Claude Code](https://docs.anthropic.com/en/docs/claude-code/overview)
2. Clone this repository
3. Run `claude` in the project directory — skills are picked up automatically from `.claude/skills/`

## License

MIT
