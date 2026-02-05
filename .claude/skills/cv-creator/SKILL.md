---
name: cv-creator
description: Professional CV and resume builder transforming career narratives into ATS-optimized, multi-format resumes. Integrates with career-biographer for data and competitive-cartographer for positioning. Generates PDF, DOCX, LaTeX, JSON Resume, HTML, and Markdown. Activate on 'resume', 'CV', 'ATS optimization', 'job application'. NOT for cover letters, portfolio websites (use web-design-expert), LinkedIn optimization, or interview preparation.
allowed-tools: Read,Write,Edit,WebFetch,WebSearch
category: Business & Monetization
tags:
  - resume
  - ats
  - career
  - pdf
  - latex
pairs-with:
  - skill: career-biographer
    reason: Get structured career data
  - skill: job-application-optimizer
    reason: Tailor CVs to specific roles
---

# CV Creator

Professional resume builder that transforms structured career data into ATS-optimized, professionally formatted resumes.

## Integrations

Works with: career-biographer, competitive-cartographer, web-design-expert, typography-expert

## Production Implementation Available!

**GitHub**: [github.com/erichowens/cv-creator](https://github.com/erichowens/cv-creator)
- Status: Production-ready (~2,000 LOC)
- ATS Score: 95/100 achieved
- Deploy: `npm install && npm run example`

Built through multi-skill orchestration (8 skills, 9 phases).

## Quick Start

```
User: "Create a resume for senior software engineer roles"

CV Creator:
1. Request CareerProfile (from biographer or direct input)
2. Request PositioningStrategy (from cartographer or skip)
3. Request target role/company (optional)
4. Generate resume with clean formatting
5. Calculate ATS score and provide recommendations
6. Export in requested formats (PDF, DOCX, JSON Resume)
```

**Key principle**: ATS compatibility first, human readability second, visual flair never.

## Core Capabilities

### 1. Multi-Format Generation
| Format | Use Case |
|--------|----------|
| PDF | Email applications, job boards, print |
| DOCX | Recruiter submissions, editable |
| JSON Resume | Developer portfolios, programmatic |
| HTML | Portfolio websites, responsive |
| Markdown | Version control, git-based management |
| LaTeX | Academic CVs (optional) |

### 2. ATS Optimization Engine
- Keyword analysis and matching from job descriptions
- Formatting validation (single-column, standard fonts)
- Scoring system (0-100) with specific recommendations
- Parsing simulation

### 3. Template System

| Template | Best For |
|----------|----------|
| **Modern Minimalist** | Tech roles (Engineers, Data Scientists) |
| **Professional Traditional** | Finance, Legal, Senior Executives |
| **Creative Hybrid** | Design Engineers, UX Researchers |
| **Academic CV** | PhD, Professors, Researchers |

## ATS Score Breakdown

| Category | Points | Criteria |
|----------|--------|----------|
| Formatting | 30 | Single-column, standard fonts, no graphics |
| Structure | 20 | Summary, Skills, Experience, Education present |
| Content | 30 | Proper lengths, skills count, metrics in bullets |
| Keywords | 20 | Job description coverage (or 15 for general) |

**Target**: 85+ out of 100

## When to Use

**Use for:**
- Creating resume from career-biographer data
- Optimizing resume for specific job posting
- Generating multiple resume variants
- ATS score and improvement recommendations
- Multi-format export

**Do NOT use for:**
- Cover letters (different format)
- Portfolio websites (use web-design-expert)
- LinkedIn profile optimization
- Interview preparation
- Career counseling or job search strategy

## Anti-Patterns

### Anti-Pattern: Creative Resume for Tech Roles
**What it looks like**: Colorful infographics, skill bars, profile photo, two-column layout
**Why wrong**: ATS systems can't parse graphics or complex layouts
**Instead**: Use Minimalist template with clean, single-column text format

### Anti-Pattern: Generic Objective Statement
**What it looks like**: "Seeking a challenging role in a growth-oriented company..."
**Why wrong**: Wastes space, provides no information
**Instead**: Professional summary with specific metrics and target role

### Anti-Pattern: Listing Every Technology Ever Used
**What it looks like**: 40+ skills including outdated technologies
**Why wrong**: Dilutes expertise, unclear proficiency
**Instead**: List 15-20 most relevant skills for target role

### Anti-Pattern: Responsibilities Without Outcomes
**What it looks like**: "Managed a team", "Worked on backend systems"
**Why wrong**: Doesn't show impact or value
**Instead**: "Led team of 5 to deliver microservices migration, reducing deployment time by 70%"

### Anti-Pattern: Inconsistent Formatting
**What it looks like**: Mixed date formats, different bullet styles, varying fonts
**Why wrong**: Looks unprofessional, confuses ATS parsers
**Instead**: Strict consistency throughout

## Troubleshooting Quick Reference

| Issue | Cause | Fix |
|-------|-------|-----|
| ATS Score &lt;70 | Complex formatting, graphics | Switch to Minimalist, remove images |
| Keyword Coverage &lt;60% | Not tailoring to job description | Extract keywords, add to Core Skills |
| Exceeds 2 pages | Too verbose, old roles included | Consolidate old roles, limit bullets |
| Generic summary | No positioning insights | Include specific metric, state target role |
| Long bullets | Trying to explain entire project | Split into multiple bullets, focus on outcome |

## Length Guidelines

| Experience | Pages |
|------------|-------|
| Entry-level (0-3 years) | 1 page |
| Mid-level (3-10 years) | 1-2 pages |
| Senior-level (10+ years) | 2 pages max |

**Never exceed 2 pages**, even for very senior roles.

## Resume Formats

| Format | When to Use | ATS |
|--------|-------------|-----|
| **Chronological** | Standard, most roles | ✅ Best |
| **Functional** | Diverse experience, long tenure at one company, entrepreneurs | ⚠️ Poor |
| **Hybrid** | Best of both, maximum relevance | ✅ Good |

**Recommendation**: Use hybrid format. If ATS is critical, keep chronological structure with functional highlights.

## Company Description

**Always describe your company** — recruiters don't know it. Include:
- Industry/sector
- Scale indicator (choose 1-2):
  - Market position: "Top 3 in industry"
  - Headcount: "500+ employees"
  - Revenue: "$100M+ annual revenue"
  - Users: "50K+ daily active users"
  - Geography: "Operating in 15 countries"

**Examples**:
- "Scentbird — subscription service in the U.S., offering 500+ branded fragrances, with 300K avg. monthly subs."
- "DeepCloud AI — building 'Airbnb version of AWS Cloud' to democratize cloud computing."

## Experience Block Structure

Each role should contain:
1. **Company name** + brief description
2. **Your role title** (match to target job title if possible)
3. **Dates**: Month/Year - Month/Year (use "Present" for current)
4. **Location** (optional, useful for international search)
5. **Results** as bullets (3-5 per role, max 7)

### Writing Results

**Start with action verbs** (past tense):
- Increased, reduced, improved, optimized
- Developed, implemented, launched, created
- Led, managed, coordinated, mentored
- Analyzed, designed, architected, automated

**One result = one bullet**. Keep to 1-2 sentences max.

## Additional Sections

### Education
- **Top international university** → Place BEFORE Experience
- **Standard education** → Place AFTER Experience
- Include: Degree, Specialization, University name, Years
- Shorten unknown university names to keywords: "Technical Institute" not full Russian name

### Certifications
- Only relevant to target role
- Only recent (last 5 years)
- Internationally recognized preferred

### Languages
- **USA/Europe**: Don't specify English level if resume is in English
- **Russia**: Use A1-C2 levels
- Use descriptive levels: "Full professional proficiency", "Limited working proficiency"

### Hobbies/Volunteering
Only include if they illustrate soft skills with achievements:
- ✅ "Organized Burning Man camps for 5 years, 200+ participants"
- ✅ "Mentored 15 junior developers, 3 promoted to senior"
- ❌ "Reading, traveling, movies"

## Red Flags to Avoid

| Flag | Risk | Fix |
|------|------|-----|
| **Employment gaps 6+ months** | Unmotivated | Fill with consulting, projects, education |
| **Job hopping** (<1 year repeatedly) | Unreliable | Frame as project work, explain context |
| **Non-relevant roles** | Unclear focus | Minimize or connect to current profession |
| **Overlapping jobs** | Confusing | Clarify: "(contract)", "(part-time)", "(freelance)" |
| **Toxicity** | Instant reject | Never criticize past employers |
| **Role mismatch** | Wrong fit | Align last role title with target |
| **Long tenure without growth** | Stagnation | Show progression, promotions, expanded scope |
| **Photo** (USA/Europe) | Discrimination risk | Remove for international applications |
| **Personal info** | Discrimination risk | Remove age, gender, marital status, religion |

### How to Describe Employment Gaps

**Don't write**: "Sabbatical", "Burnout recovery"

**Do write**: Consulting, freelance, project work, own business, education

Example: "Independent Consultant (2022-2023): Advised 3 startups on product strategy, resulting in $2M combined seed funding."

## Green Flags

- Known company names in experience
- Top university education
- Concise summary tailored to role
- Role progression showing growth
- Results with metrics
- Logical career path

## Market-Specific Guidelines

### USA
- **Remove**: Photo, age, gender, marital status, address, religion
- **Resume** (not CV)
- **Dates**: "4/2023" or "April 2023"
- **Numbers**: 100,000 (comma separator), 25.5% (dot decimal)
- **Currency**: $5,000 or USD5,000 (before number, no space)
- **Abbreviations**: K (thousand), M (million), B (billion)

### Europe
- **Remove**: Same as USA (varies by country)
- **CV** (not Resume)
- **Dates**: "April 2023"
- UK spelling: personalisation, behaviour, fulfil

### Russia
- Photo acceptable
- Age may be calculated from graduation year
- Use A1-C2 for language levels

## ATS Technical Requirements

**ATS loves:**
- ✅ PDF format
- ✅ Single column layout
- ✅ Standard section names (Experience, Education, Skills)
- ✅ Bullets for results
- ✅ Month + Year for dates
- ✅ Keywords from job description
- ✅ Links to: LinkedIn, GitHub, Kaggle, Behance

**ATS hates:**
- ❌ Graphics, images, charts
- ❌ Tables, columns
- ❌ White text on dark background
- ❌ Special symbols (฿₽®©™), emojis
- ❌ Font smaller than 11pt
- ❌ Non-standard section names

## File Naming

Format: `FirstName_LastName_Resume.pdf` or `FirstName_LastName_Resume_RoleName.pdf`

---

## ATS System-Specific Requirements

Different ATS systems have specific parsing behaviors. Adapt your resume based on target company's system.

### Taleo (Oracle)
- **Format**: DOC/DOCX preferred (PDF poorly parsed)
- **Fonts**: Minimum 11pt or text may not be recognized
- **Keywords**: Must be exact matches from job posting
- ❌ Graphics, tables, visual elements
- ✅ Plain text format

### Greenhouse
- **Format**: PDF and DOCX both work well
- **Bullets**: Supports bullets and numbered lists
- **Keywords**: Uses context-aware algorithms (sentences > keyword lists)
- **Company descriptions**: Auto-matches company data
- ❌ Complex graphical elements

### Workday
- **Format**: DOCX preferred (PDF may misparse)
- **Section names**: Must be standard ("Experience", "Education", "Skills")
- **Keywords**: Exact term matching with job description
- ❌ Creative section names

### Lever
- **Format**: PDF and DOCX both work
- **Keywords**: Context-aware, use terms in sentences
- ❌ Tables, columns, complex formatting

### JazzHR
- **Format**: PDF, DOC, DOCX
- **Bullets**: Supported and recommended
- **Context**: Analyzes phrase context, not just keywords
- ❌ Complex tables and graphics in PDF

### SmartRecruiters
- **Format**: DOCX preferred
- **Profiles**: Include LinkedIn, GitHub links (system uses them)
- **Keywords**: Keyword-focused matching

### iCIMS
- **Format**: PDF and DOCX
- **Layout**: Single-column recommended
- **Soft skills**: System considers soft skills keywords
- ❌ Images, graphics

### Jobvite
- **Format**: PDF and DOCX
- **Links**: Avoid excessive links/images
- **Keywords**: Strict matching to job description
- ❌ Complex visual elements

### Universal ATS Rules
1. **Use standard section names**: "Experience", "Education", "Skills", "Certifications"
2. **Minimize visual elements**: No graphics, images, tables
3. **Formatting**: Use 1-2 level bullets max, avoid complex lists
4. **Keywords**: Tailor resume to each job posting
5. **Simple structure**: Easy to parse, no complex layouts

---

## Power Verbs for Results

### Technical Work
Scoped, Troubleshooted, Strengthened, Segmented, Diagnosed, Installed, Implemented, Planned, Re-engineered, Visualized, Assembled, Restructured, Tested, Developed, Automated, Architected, Re-architected, Engineered, Coded, Validated, Designed, Steered

### Creating / Writing
Acted, Adapted, Combined, Composed, Conceptualized, Condensed, Created, Customized, Designed, Developed, Devised, Directed, Displayed, Established, Fashioned, Formulated, Founded, Illustrated, Initiated, Instituted, Integrated, Introduced, Invented, Modeled, Modified, Originated, Performed, Planned, Revised, Revitalized, Shaped, Solved

### Research / Analysis
Analyzed, Clarified, Collected, Compared, Conducted, Critiqued, Detected, Determined, Diagnosed, Evaluated, Examined, Experimented, Explored, Extracted, Formulated, Gathered, Identified, Inspected, Interpreted, Interviewed, Investigated, Located, Measured, Organized, Researched, Reviewed, Searched, Summarized, Surveyed, Systematized

### Project / Team Management
Accomplished, Administered, Advanced, Appointed, Approved, Assigned, Attained, Authorized, Chaired, Consolidated, Contracted, Controlled, Coordinated, Decided, Delegated, Directed, Eliminated, Enhanced, Established, Executed, Generated, Handled, Headed, Hired, Hosted, Improved, Incorporated, Increased, Initiated, Inspected, Led, Managed, Merged, Motivated, Navigated, Organized, Originated, Overhauled, Oversaw, Planned, Presided, Prioritized, Produced, Recommended, Reorganized, Restored, Reviewed, Scheduled, Secured, Selected, Streamlined, Strengthened, Supervised

### Numbers / Metrics
Administered, Adjusted, Allocated, Analyzed, Appraised, Assessed, Audited, Balanced, Budgeted, Calculated, Computed, Conserved, Controlled, Corrected, Decreased, Determined, Developed, Estimated, Forecasted, Managed, Marketed, Measured, Netted, Planned, Prepared, Programmed, Projected, Qualified, Reconciled, Reduced, Researched, Retrieved

### Helping / Collaborating
Adapted, Advocated, Aided, Answered, Arranged, Assessed, Assisted, Clarified, Coached, Collaborated, Contributed, Cooperated, Counseled, Demonstrated, Diagnosed, Educated, Encouraged, Ensured, Expedited, Facilitated, Furthered, Guided, Helped, Intervened, Motivated, Prevented, Provided, Referred, Represented, Resolved, Simplified, Supplied, Supported, Volunteered

### Teaching / Mentoring
Adapted, Advised, Clarified, Coached, Communicated, Conducted, Coordinated, Critiqued, Developed, Enabled, Encouraged, Evaluated, Explained, Facilitated, Focused, Guided, Individualized, Informed, Instructed, Motivated, Persuaded, Simulated, Stimulated, Taught, Tested, Trained, Transmitted, Tutored

---

## Developer Results Examples

### Software Developer
- Coded and optimized algorithms that enhanced data processing efficiency by 90% YoY
- Designed automated low latency, high throughput data pipelines for 20+ trading systems
- Cut downtime by 20% by maintaining maximum uninterrupted flow of critical ops
- Boosted coding efficiency by 30% by identifying and fixing process bottlenecks
- Streamlined and automated 500+ reports, saving $120K in quarterly costs

### Frontend / React Developer
- Decreased load times by 58% using isomorphic React and Node.js for 13 web applications
- Reduced development time by 73% by creating maintainable reusable components
- Created HTML email templates that improved CTR rates by 65% for 23 weeks
- Revamped UI for customer-facing e-commerce site, leading to 200K unique visitors/week

### Backend Developer
- Reduced deployment time from 72 hours to 50 minutes using Jenkins Pipelines and Kubernetes
- Developed microservices architecture with Node.js serving 1.5M users hourly
- Collaborated with team of 25 to create platform scaling to 10M daily visitors

### Mobile Developer
- Created web service used by 200K clients generating $100K monthly within 20 days
- Launched mobile app generating 100K downloads, featured as "App of the Year"
- Achieved 400K+ downloads on App Store across apps in 45 countries

### Python Developer
- Built API-driven publishing service handling 17M pageviews monthly at 94% cache efficiency
- Cleared 200+ performance bottlenecks in Mercurial for large-scale deployments
- Extended build system reducing 47% performance issues

### Database / SQL
- Created aggregates and partitions reducing cube processing from 4.6 hours to 45 minutes
- Optimized SQL queries reducing data retrieval time by 25% and improving efficiency by 60%
- Developed custom queries improving report accuracy by 88%

---

## Junior Resume Guidelines

### What to Include (Even Without Commercial Experience)
- **All work in new profession**: Even academic projects, even free work
- **Hackathon participation**: Write it up
- **Test assignments**: Complete and showcase as portfolio
- **Help to friends/family**: "Created logo for local business", "Built website for startup"
- **Pet projects**: Task managers, utilities, games you built

### Block Order for Juniors
1. Summary (called "Personal Profile" is also acceptable)
2. **Education** (place BEFORE Experience if from good university)
3. Skills
4. Experience (including academic projects)
5. Certifications / Courses

### What to Include from Education
- University, faculty, specialization
- Coursework and thesis projects related to target role
- GPA if above 3.0 (USA)
- Academic awards
- Relevant disciplines (e.g., Mathematics, Statistics, Computer Science)
- Student activities showing leadership

### Professional Motivation
Employers invest in juniors who show:
- Strong motivation ("hungry to learn")
- Extra activities in profession
- Pet projects and test assignments
- Hackathon participation
- Clear professional goals

---

## Career Switcher Resume Guidelines

### Core Principles
1. **Show both**: New profession skills AND previous background
2. **Connect the dots**: Explain how previous experience helps in new role
3. **Prove motivation**: Show transition logic and what you've already done

### What Works
- Switching within same company (internal transfer)
- Highlighting achievements in previous career (shows you're capable)
- Using background as advantage (e.g., medical background → health tech)
- Showing already acquired skills in new profession

### What to Avoid
❌ Deleting all previous experience (looks like no work history)
❌ No explanation of career change logic
❌ 37-year-old "junior" with no mention of prior career

### Example: Good vs Bad Switcher Presentation

**Bad**: "Junior Frontend Developer, 37 years old"

**Good**: "Junior Frontend Developer with 10 years in financial analysis. Completed [bootcamp], built [3 projects]. Looking to apply analytical mindset to data-driven frontend development in fintech."

### Balance Rule
- More experience in new profession → shorter previous career section
- Less experience in new profession → leverage transferable skills more

---

## Summary Formula for Role Targeting

**Formula**: Who + doing what + for how long + with which differentiated expertise

**Structure**:
```
[Role type] с [X лет] опыта в [специализация/домен].
[Ключевой навык/технология] + [масштаб/контекст].
[Уникальная экспертиза или достижение].
```

**Example**:
> "Senior Frontend Developer with 5+ years of experience in React ecosystem. Built and scaled customer-facing products serving 500K+ monthly users. Domain expertise in fintech and payment systems."

**Process**:
1. Take target role from "Career Closet"
2. Select 3-5 key requirements where you rate yourself 4-5
3. Write each skill in third person using formula
4. Condense with ChatGPT to "dry out" verbose text

---

## Tech Industry Categories (45 domains)

Use for describing domain expertise in resume:

| Category | Description |
|----------|-------------|
| **Adtech** | Ad targeting, placement, measurement, fraud detection |
| **Fintech** | Digital banks, payments, blockchain, crypto, lending |
| **Edutech** | LMS, e-learning platforms, tutoring, educational games |
| **HealthTech** | EHR, telemedicine, health trackers, fitness apps |
| **HRTech** | ATS, performance management, HRIS |
| **Ecommerce** | Online stores, marketplaces, shopping tools |
| **Gamedev** | Game design, development (PC, mobile, console, VR) |
| **SaaS/Cloud** | SaaS, IaaS, PaaS platforms |
| **InfoSec** | Firewalls, encryption, IAM, SIEM, VPN |
| **IoT** | Smart home, industrial IoT, smart cities |
| **Delivery** | Food delivery, goods delivery, logistics |
| **TravelTech** | Tour aggregators, booking, trip planning |
| **PropTech** | Real estate tech, property management |
| **MarTech** | Marketing automation, CRM, analytics |
| **BioTech** | Drug design, medical imaging software |
| **Automotive** | ADAS, autonomous vehicles, V2V communication |
| **BigTech** | IT corporations with diverse product ecosystems |

Use format: "Domain expertise in [Category]: [specific experience]"

## Reference Files

- `references/resume-protocol.md` - Complete 8-step generation protocol, ATS scoring, before/after examples
- `references/formatting-rules.md` - Best practices, templates, output formats, success metrics
- `references/interfaces-integration.md` - TypeScript interfaces, multi-skill workflows

---

**Core insight**: ATS compatibility first—the best-written resume is worthless if it never reaches human eyes.

**Use with**: career-biographer (content) | competitive-cartographer (positioning) | web-design-expert (portfolio)
