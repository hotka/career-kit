---
name: interview-master
description: Use when the user asks to "prepare for interview", "conduct mock interview", "generate interview questions", or mentions interview preparation. Provides interview question generation, mock interviews, and preparation guidance for technical roles.
version: 0.2.0
---

# Interview Master

Specialized skill for technical interview preparation: question generation, mock interviews, and preparation roadmaps.

## When to Use This Skill

Use this skill when:

- Generating interview questions for specific roles or seniority levels
- Preparing for technical interviews (algorithms, system design, behavioral)
- Conducting mock interviews with realistic scenarios
- Creating interview preparation roadmaps

**Do NOT use for:**
- Resume creation or optimization → use `cv-creator`
- Career data collection → use `career-biographer`
- Job search strategy → use `job-search-strategist`
- Algorithm practice → use `leetcode-teacher`

## Core Capabilities

### 1. Interview Question Generation

Generate role-specific interview questions tailored to position requirements, seniority level, and technical stack.

**Process:**
1. Identify target role, seniority (junior/mid/senior/staff), and tech stack
2. Consult `references/interview-questions-bank.md` for question patterns
3. Generate questions across categories:
   - Technical fundamentals
   - Problem-solving and algorithms
   - System design (for senior+ roles)
   - Behavioral and situational
   - Role-specific deep dives
4. Include follow-up questions and evaluation criteria
5. Provide answer guidelines for interviewers

Typical output includes 10-15 questions with difficulty ratings, estimated time, and evaluation rubrics.

### 2. Mock Interview Simulation

Conduct realistic mock interviews with real-time feedback and performance evaluation.

**Process:**
1. Establish interview context (role, company type, interview stage)
2. Reference `references/interview-flow.md` for realistic pacing
3. Ask questions progressively, adapting difficulty based on responses
4. Provide hints if candidate struggles
5. Evaluate responses on:
   - Technical accuracy
   - Communication clarity
   - Problem-solving approach
   - Time management
6. Deliver constructive feedback with improvement areas

See `examples/mock-interview-dialogue.md` for interaction patterns.

### 3. Interview Preparation Guidance

Create personalized preparation roadmaps for technical interviews.

**Process:**
1. Assess candidate current level and target role
2. Generate study plan covering:
   - Algorithm and data structures (reference: `references/algorithm-prep.md`)
   - System design concepts (reference: `references/system-design-prep.md`)
   - Behavioral interview techniques (reference: `references/behavioral-interview.md`)
3. Provide timeline-based milestones (2 weeks, 1 month, 3 months)
4. Include practice resources and mock interview schedules
5. Track preparation progress and adjust plan

## Workflow

### For Job Seekers

1. **Assess Level**: Determine current skills and target role
2. **Create Roadmap**: Generate personalized preparation plan
3. **Practice**: Conduct mock interviews, iterate based on feedback
4. **Review**: Adjust plan based on progress

### For Interviewers

1. **Question Design**: Specify role requirements → generate tailored question set
2. **Evaluation Framework**: Use provided rubrics → standardize candidate assessment
3. **Interview Calibration**: Reference mock interview examples → align interview style

## Reference Files

- **`references/interview-questions-bank.md`** - Comprehensive question library by role and category
- **`references/algorithm-prep.md`** - Algorithm interview preparation roadmap
- **`references/system-design-prep.md`** - System design concepts and practice problems
- **`references/behavioral-interview.md`** - STAR method and behavioral question patterns
- **`references/interview-flow.md`** - Realistic interview pacing guide

## Example Files

- **`examples/interview-questions-set.md`** - Complete interview question sets
- **`examples/mock-interview-dialogue.md`** - Realistic interview conversation flows

## Interview Stages & Types

### Interview Funnel

| Этап | Кто проводит | Что оценивает | Длительность |
|------|--------------|---------------|--------------|
| Screening | Рекрутер | Базовое соответствие, мотивация, salary expectations | 15-30 мин |
| Technical Screen | HR/Tech Lead | Базовые технические знания, коммуникация | 30-60 мин |
| Technical Deep-Dive | Hiring Manager | Глубокие технические навыки, problem-solving | 60-90 мин |
| System Design | Senior Engineers | Архитектурное мышление, trade-offs (для Senior+) | 45-60 мин |
| Peer Interview | Future Teammates | Culture fit, collaboration style | 30-45 мин |
| Bar Raiser / Culture | Cross-team | Соответствие ценностям компании | 30-45 мин |
| Final / Offer | Hiring Manager/Director | Финальное решение, обсуждение оффера | 30-60 мин |

### Типы интервью по формату

| Тип | Описание | Как готовиться |
|-----|----------|----------------|
| **Behavioral** | Вопросы о прошлом опыте (STAR) | Подготовить 10-15 историй из опыта |
| **Technical** | Кодинг, алгоритмы | LeetCode, mock coding sessions |
| **System Design** | Проектирование систем | Изучить паттерны, практиковать на примерах |
| **Live Coding** | Код в реальном времени | Практика с таймером, думать вслух |
| **Take-Home** | Тестовое задание | Чистый код, документация, тесты |
| **Case Study** | Бизнес-кейсы | Структурированный подход к анализу |

---

## Standard Interview Questions

### "Расскажите о себе" (Tell me about yourself)

**Структура ответа (Present-Past-Future):**

```
1. PRESENT (30 сек): Кто вы сейчас
   "Я [роль] с [X лет] опыта в [область]. Сейчас работаю в [компания], где [ключевая ответственность]."

2. PAST (60 сек): Ключевые достижения
   "До этого я [предыдущий опыт]. Главное достижение — [результат с цифрами]."

3. FUTURE (30 сек): Почему эта позиция
   "Сейчас ищу возможность [что хотите]. Эта роль интересна, потому что [конкретная причина]."
```

**Пример для Frontend Developer:**
> "Я Frontend Developer с 4 годами опыта в React экосистеме. Сейчас работаю в fintech-стартапе, где отвечаю за разработку клиентского dashboard'а с 50K MAU.
>
> До этого я работал в продуктовой компании, где переписал legacy jQuery-код на React, что сократило время загрузки страниц на 40% и уменьшило количество багов на 60%.
>
> Сейчас хочу расти в сторону Senior-позиции в продукте с высокой нагрузкой. Ваша компания интересна мне, потому что вы работаете с миллионами пользователей и активно используете современный стек."

### "Почему хотите работать у нас?"

**Формула ответа:**
1. Что знаете о компании (research!)
2. Что вас привлекает конкретно
3. Как это связано с вашими целями

**Что изучить перед ответом:**
- Продукт/сервис компании
- Технологический стек
- Последние новости, блог, публикации
- Ценности и культура
- Glassdoor/отзывы сотрудников

### "Ваши сильные и слабые стороны"

**Сильные стороны — формат:**
```
Сильная сторона + Пример из опыта + Результат
```

**Слабые стороны — формат:**
```
Реальная слабость + Что делаете для улучшения + Прогресс
```

**НЕ говорите:**
- "Я перфекционист" (клише)
- "Работаю слишком много" (неискренне)
- Критичные для роли слабости

**Хороший пример:**
> "Раньше мне было сложно давать негативный фидбек коллегам — избегал конфликтов. Осознал это после 360-review и начал практиковать nonviolent communication. Сейчас провожу code review с конструктивной критикой, и коллеги отмечают, что мой фидбек помогает расти."

### "Где видите себя через 5 лет?"

**Структура:**
1. Рост в профессии (конкретные навыки)
2. Рост в компании (если релевантно)
3. Связь с текущей позицией

**НЕ говорите:**
- "На вашем месте" (агрессивно)
- "Не знаю" (нет амбиций)
- Планы, не связанные с компанией

### "Почему уходите с текущего места?"

**Правила:**
- ❌ Не критиковать текущего работодателя
- ❌ Не жаловаться на коллег/менеджера
- ✅ Фокус на том, что ищете (pull), не на том, от чего бежите (push)

**Хорошие причины:**
- Ищу новые технические вызовы
- Хочу работать с [технология/масштаб]
- Готов к следующему уровню ответственности
- Интересна другая доменная область

### Вопрос о зарплатных ожиданиях (на скрининге)

**Стратегии:**
1. **Перенаправить:** "Хотел бы сначала узнать больше о роли и ответственности. Какой бюджет заложен на эту позицию?"
2. **Диапазон:** "Ориентируюсь на диапазон $X-$Y, но готов обсудить после понимания полного пакета компенсации."
3. **Market rate:** "Ожидаю рыночный уровень для [роль] с моим опытом в [локация]."

---

## STAR(L) Framework for Behavioral Questions

### Структура STAR

| Компонент | Вопрос | Время | Доля ответа |
|-----------|--------|-------|-------------|
| **S**ituation | Какой был контекст? | 20 сек | 15% |
| **T**ask | Какая была ваша задача/цель? | 15 сек | 10% |
| **A**ction | Что конкретно вы сделали? | 90 сек | 60% |
| **R**esult | Каков измеримый результат? | 20 сек | 15% |
| **L**earning (опц.) | Что вы из этого вынесли? | 15 сек | — |

### Правила STAR

1. **Situation/Task — коротко:** Только необходимый контекст
2. **Action — максимум деталей:**
   - Используйте "Я", не "Мы"
   - Конкретные действия, не общие фразы
   - Покажите ваше мышление и решения
3. **Result — измеримо:**
   - Цифры, метрики, проценты
   - Если нет цифр — качественный результат
   - Фидбек от stakeholders

### Примеры behavioral вопросов

**Командная работа:**
- Tell me about a time you had a conflict with a teammate
- Describe a situation where you had to work with a difficult colleague
- Give an example of successful collaboration

**Проблемы и неудачи:**
- Tell me about a time you failed
- Describe a situation where you made a mistake
- How did you handle a project that went wrong?

**Лидерство и влияние:**
- Tell me about a time you led a project
- Describe when you had to convince others of your idea
- Give an example of mentoring someone

**Работа под давлением:**
- Tell me about a time you had a tight deadline
- Describe handling multiple priorities
- How did you deal with ambiguity?

### Пример STAR-ответа

**Вопрос:** "Tell me about a time you had to meet a tight deadline."

> **Situation:** В прошлом году наш главный клиент запросил срочную интеграцию нового payment provider за 2 недели вместо обычных 6.
>
> **Task:** Как lead developer, я отвечал за техническую реализацию и координацию с командой из 3 человек.
>
> **Action:**
> - Первым делом провёл анализ scope и выделил MVP-функционал, отложив nice-to-have фичи
> - Разбил работу на параллельные потоки: один разработчик — API интеграция, другой — UI, я — архитектура и code review
> - Организовал daily standup в 9:00 и async-check в 17:00 для быстрого разблокирования
> - Договорился с QA о параллельном тестировании вместо sequential
> - Сам взял на себя самую рискованную часть — обработку ошибок и retry logic
>
> **Result:** Запустили за 12 дней. Клиент сохранил $50K комиссии за счёт нового провайдера в первый же месяц. Получил отличный фидбек от CTO за crisis management.
>
> **Learning:** Понял важность раннего выявления критического пути и параллелизации работы.

---

## Alternative Interview Frameworks

Beyond STAR, these frameworks help adapt your answers to different question types:

### CHAPEL — For Problem-Solving Stories

Best for describing how you solved a complex problem.

| Component | Description |
|-----------|-------------|
| **C**hallenge | What was the problem/situation? |
| **H**ypothesis | What insight led to your actions? |
| **A**ctions | What did you do? |
| **P**ersonal Results | Results for you/team/project |
| **E**mployer Results | Results for clients/business |
| **L**earning | What would you do differently now? |

### DIGS — For Deep-Dive Stories

Best for stories that need more context and alternatives considered.

| Component | Description |
|-----------|-------------|
| **D**ramatize | Add life to the story: specific clients, specific deals, exact words. Why was your work important? |
| **I**ndicate alternatives | Describe 3 possible solutions (max), explain pros/cons, why you chose your approach |
| **G**o through what you did | Show how you influenced the situation with specific details, team reactions, resistance overcome |
| **S**ummarize impact | Positive impact on product/company/client with numbers, percentages, or qualitative feedback |

### PEARL — For Negative Case Stories

Best for describing failures, conflicts, or negative feedback.

| Component | Description |
|-----------|-------------|
| **P**roblem | What happened? |
| **E**motion | What did you feel? What did others feel? |
| **A**ction | What did you do? |
| **R**esult | What was the outcome? |
| **L**earning | What did you learn? How did you change? |

**Use for:**
- Failed projects
- Overestimated your abilities
- Conflicts with teammates
- Negative feedback received

### CIRCLE — For Product Design Questions

Best for questions about improving or designing products.

| Component | Description |
|-----------|-------------|
| **C**ontext | Describe the situation for the design decision |
| **I**ssue | Who are the users? What problems do they have? |
| **R**esolution | What steps and methods did you apply? |
| **C**onsequence | What were the results? How did you measure impact? |
| **L**earning | What did you learn for future projects? |

### HEART — For Success Metrics (Large Companies)

Framework for evaluating UX quality and business impact.

| Component | Description |
|-----------|-------------|
| **H**appiness | User satisfaction metrics |
| **E**ngagement | Activity, frequency of use, interaction |
| **A**doption | How successfully is the product adopted by market? |
| **R**etention | How well are users retained? |
| **T**ask Success | How well does product help users achieve goals? |

### AARRR — For Success Metrics (Startups)

"Pirate Metrics" — for measuring key stages of user interaction.

| Component | Description |
|-----------|-------------|
| **A**cquisition | How does the startup attract new users? |
| **A**ctivation | How do users start interacting with the product? |
| **R**etention | How does the startup retain users and create loyalty? |
| **R**eferral | How do users become advocates and recommend the product? |
| **R**evenue | What strategies are used for monetization? |

### When to Use Each Framework

| Situation | Framework |
|-----------|-----------|
| Standard behavioral question | STAR(L) |
| Complex problem you solved | CHAPEL or DIGS |
| Failure or conflict | PEARL |
| Product/design improvement | CIRCLE |
| Metrics discussion (enterprise) | HEART |
| Metrics discussion (startup) | AARRR |

---

## Behavioral vs Situational Questions

### Why Interviewers Use These Questions

Instead of asking "Are you stress-resistant?" (gets "yes"), they ask:
"Tell me about a time when your presentation didn't go as planned. What did you do?"

This reveals:
1. **Real experience**: How you actually behaved in situations
2. **Your thinking and approach**: Your strategies for problem-solving
3. **Predictive behavior**: Past behavior predicts future behavior

### Behavioral Questions (Past Experience)

**Question**: "Tell me about a time you had a conflict at work. How did you resolve it?"

**What it reveals**: How you typically handle conflicts and stress. Your answer shows your strategies for resolving difficult situations.

### Situational Questions (Hypothetical)

**Question**: "Imagine you're working on an important project, and at the last moment you receive additional tasks. How would you act?"

**What it reveals**: How you plan to handle pressure and multitasking. Shows prioritization, time management, and composure under pressure.

### Preparation Strategy

1. **Remember examples**: Think of situations where you successfully handled conflicts, stress, multitasking
2. **Use STAR method**: Structure your answer with Situation, Task, Action, Result
3. **Don't fear mistakes**: Real examples with problems and errors are more credible than "perfect" stories. Show what you learned.

---

## Portfolio for Interview Preparation

### Why Build a Portfolio (Even If You Don't Show It)

Your resume doesn't tell the full story:
- Important details about your projects and results
- Context and complexity of tasks
- Your individuality

### What Portfolio Gives You

1. **Deeper project stories**: Scale, complexity, implementation details
2. **Visual proof**: Links, screenshots, videos
3. **Professional evolution**: Show your growth journey
4. **NDA-safe illustrations**: Show impact without revealing confidential data
5. **Interview preparation**: Structured stories ready for any behavioral question

### Portfolio Rules

- **Only strong projects**: Employers judge you by your weakest piece
- **2-3 excellent > 10 mediocre**
- **Remove old and weak work**

### Building Non-Public Portfolio for Interviews

1. Choose one role from your "Career Closet"
2. List projects/cases you're ready to discuss in interview
3. Match each key skill to at least one project/case
4. If no case exists for important skill → create one (volunteer work, side project, etc.)

**Lifehack**: A well-organized portfolio helps you prepare structured, detailed answers for any interview question.

---

## Stress Interviews

### Тактики стресс-интервью

| Тактика | Пример | Как реагировать |
|---------|--------|-----------------|
| **Агрессивные вопросы** | "Почему вы до сих пор на такой позиции?" | Спокойно ответить по существу |
| **Прерывание** | Не дают закончить мысль | "Позвольте закончить мысль, это важно" |
| **Молчание** | Долгая пауза после ответа | Спросить "Могу ли дополнить?" |
| **Провокации** | "Это слабый ответ" | Попросить конкретный фидбек |
| **Impossible tasks** | Задача без решения | Показать процесс мышления |

### Признаки нездоровой культуры

🚩 **Red flags:**
- Грубость, переходящая в оскорбления
- Вопросы о личной жизни/планах на детей
- Требование решить задачу "немедленно"
- Интервьюер опаздывает без извинений

✅ **Нормальный стресс-тест:**
- Проверка реакции на давление
- Технически сложные вопросы
- Быстрый темп
- Вопросы о failures

### Скрипты для сложных ситуаций

**Если не знаете ответ:**
> "Хороший вопрос. Честно, не работал с этим напрямую. Но могу предположить, что... [гипотеза]. Как бы вы это решали?"

**Если вопрос неуместный:**
> "Не уверен, как это связано с позицией. Можете пояснить, что хотите узнать?"

**Если интервьюер груб:**
> "Чувствую, что разговор идёт в напряжённом тоне. Хочу убедиться, что правильно понимаю вопросы — можем сделать паузу?"

---

## Test Assignments (Take-Home)

### Когда соглашаться на тестовое

✅ **Делать:**
- Компания мечты
- Интересная техническая задача
- Разумный объём (4-8 часов)
- Есть дедлайн и чёткие требования

❌ **Отказаться или обсудить:**
- Задача на 20+ часов
- Нечёткие требования
- Нет фидбека (одностороннее)
- Похоже на бесплатную работу

### Best Practices для тестовых

| Аспект | Рекомендация |
|--------|--------------|
| **README** | Обязательно: как запустить, архитектурные решения |
| **Тесты** | Минимум unit-тесты для core логики |
| **Код** | Чистый, читаемый, без over-engineering |
| **Git** | Осмысленные коммиты, показывают процесс |
| **Время** | Не превышать заявленное; лучше MVP в срок |

### Структура README для тестового

```markdown
# Project Name

## Как запустить
- Prerequisites
- Installation
- Running

## Архитектурные решения
- Почему выбрал X вместо Y
- Trade-offs

## Что бы улучшил с большим временем
- Feature A
- Optimization B

## Затраченное время
- X часов
```

---

## Questions to Ask the Interviewer

### По роли и команде

- What does a typical day/week look like for this role?
- What are the biggest challenges the team is facing right now?
- How is the team structured? Who would I work with most closely?
- What does the onboarding process look like?
- How do you measure success for this position?

### По технологиям

- What's the tech stack? Any plans to change it?
- How do you handle technical debt?
- What's the deployment process like?
- How do you approach testing?
- What's the code review process?

### По росту

- What does career progression look like here?
- How do you support professional development?
- Are there opportunities for mentorship?
- How often do you promote from within?

### По культуре

- How would you describe the team culture?
- What do you enjoy most about working here?
- How does the team handle disagreements?
- What's the work-life balance like?

### Red flag вопросы (слушайте ответы внимательно)

- Why is this position open?
- What happened to the previous person in this role?
- What's the biggest challenge someone in this role would face?
- How do you handle it when deadlines slip?

### Вопросы, которые НЕ стоит задавать

❌ Информация с сайта компании
❌ Зарплата на первом интервью (если не спросили)
❌ Отпуск и бенефиты до оффера
❌ "Когда меня повысят?"

---

## Thank You Letters & Follow-up

### Когда отправлять

| Ситуация | Timing |
|----------|--------|
| После интервью | В тот же день или на следующий день утром |
| После отказа | В течение 24 часов |
| Если нет ответа | Через 1 неделю после обещанного срока |

### Структура thank you письма

```
Subject: Thank you - [Position] Interview

Hi [Name],

Thank you for taking the time to speak with me today about the [Position] role.

[1-2 предложения о том, что особенно заинтересовало в разговоре]

[Опционально: ответ на вопрос, который не удалось хорошо раскрыть]

I'm very excited about the opportunity to [конкретный аспект роли].

Please let me know if you need any additional information.

Best regards,
[Your name]
```

### Follow-up при отсутствии ответа

```
Subject: Following up - [Position] application

Hi [Name],

I wanted to follow up on our conversation from [date] about the [Position] role.

I remain very interested in the opportunity and would welcome any updates you can share about the process.

Thank you for your time.

Best,
[Name]
```

### Как получить фидбек после отказа

> "Thank you for letting me know. I really appreciate the time the team spent with me. If possible, could you share any feedback on areas where I could improve? I'm committed to growing and would value any insights."

---

## Cultural Differences by Country

### USA

- Direct communication style
- "Small talk" перед интервью — норма
- Важны enthusiasm и positive attitude
- "Tell me about yourself" — почти всегда первый вопрос
- Salary negotiation ожидается

### UK

- Более формальный тон, чем в США
- Understatement культура ("not bad" = good)
- Меньше "selling yourself"
- Важны teamwork и collaboration
- Сдержанный энтузиазм

### Germany

- Пунктуальность критична
- Факты и квалификации важнее soft skills
- Прямолинейные вопросы и ответы
- Формальное обращение (Herr/Frau)
- Длинный процесс принятия решений

### Netherlands

- Очень прямая коммуникация
- Egalitarian культура — иерархия размыта
- Work-life balance обсуждается открыто
- Ожидается собственное мнение
- Неформальная атмосфера

### Israel

- Очень прямой стиль ("chutzpah")
- Вопросы могут казаться агрессивными — норма
- Ценятся инновационность и challenge authority
- Неформальный dress code
- Быстрые решения

### France

- Формальность в начале, затем расслабление
- Важны дипломы и образование
- Дискуссии и дебаты — часть культуры
- Обеденный перерыв священен
- Личные вопросы могут быть

### Russia/СНГ

- Формальный стиль на первых этапах
- Может быть много этапов интервью
- Тестовые задания — обычная практика
- Вопросы о планах на семью возможны
- Обсуждение зарплаты — в конце процесса

---

## Handling Offers

### Что проверить в оффере

| Компонент | На что смотреть |
|-----------|-----------------|
| Base salary | Соответствие рынку, периодичность выплат |
| Bonus | Target %, условия получения |
| Equity/RSU | Vesting schedule, cliff, strike price |
| Benefits | Health, dental, vision, 401k match |
| PTO | Дни отпуска, sick days, holidays |
| Remote policy | Full remote, hybrid, office days |
| Start date | Гибкость, notice period |
| Signing bonus | Условия возврата |

### Принятие оффера

**Письменно подтвердить:**
```
Subject: Offer Acceptance - [Position]

Dear [Name],

I am delighted to accept the offer for the [Position] role at [Company].

I confirm:
- Start date: [Date]
- Base salary: [Amount]
- [Other key terms]

Please let me know the next steps for onboarding.

Thank you for this opportunity.

Best regards,
[Name]
```

### Отклонение оффера

**Вежливо, сохраняя отношения:**
```
Subject: [Position] Offer - Decision

Dear [Name],

Thank you so much for the offer for the [Position] role. I've genuinely enjoyed learning about [Company] and the team.

After careful consideration, I've decided to pursue another opportunity that more closely aligns with my current career goals.

I have great respect for what you're building and hope our paths cross again in the future.

Thank you again for your time and consideration.

Best regards,
[Name]
```

---

## Salary Negotiation

### Когда торговаться

✅ **Да:**
- После получения письменного оффера
- Когда есть leverage (другой оффер, редкие навыки)
- Когда оффер ниже рынка

❌ **Осторожно:**
- На первом скрининге (отложить)
- Когда оффер уже на верхней границе
- В компаниях с фиксированными грейдами

### Алгоритм переговоров

1. **Поблагодарить** за оффер
2. **Выразить энтузиазм** о роли
3. **Назвать конкретную цифру** (не диапазон)
4. **Обосновать** почему
5. **Замолчать** и ждать ответа

### Скрипт переговоров

> "Thank you so much for the offer — I'm really excited about joining [Company].
>
> Based on my research of market rates for this role and my [X years of experience / specific skill], I was hoping we could discuss the base salary.
>
> I'm looking for [specific number]. Is there flexibility here?"

### Что можно торговать кроме зарплаты

| Компонент | Как просить |
|-----------|-------------|
| Signing bonus | "Is a signing bonus possible to bridge the gap?" |
| Equity | "Could we increase the equity grant?" |
| PTO | "Is there flexibility on vacation days?" |
| Remote days | "Could we discuss a hybrid arrangement?" |
| Start date | "I'd need [X weeks] for transition" |
| Title | "Could we adjust the title to [X]?" |
| Review timing | "Could we schedule a 6-month review?" |

### Если говорят "нет"

**Варианты ответа:**
1. Принять как есть: "I understand. I'm still excited to join."
2. Попросить пересмотр: "Could we revisit compensation at the 6-month mark?"
3. Попросить другой компонент: "If base is fixed, is there flexibility on [bonus/equity]?"
4. Взять время: "Can I have until [date] to consider?"

### Red flags в переговорах

🚩 Оффер отзывают из-за переговоров
🚩 Агрессия или давление принять немедленно
🚩 "Exploding offer" (24 часа на решение)
🚩 Отказываются давать оффер письменно

---

## Best Practices

1. **Interview Questions**: Adapt difficulty to candidate level; avoid questions beyond role requirements
2. **Mock Interviews**: Maintain realistic pacing; provide hints before revealing answers
3. **Feedback Delivery**: Be constructive and specific; focus on actionable improvements
4. **Preparation Plans**: Set realistic milestones; adjust based on progress

## Common Use Cases

**Scenario 1: Junior Developer Preparing for First Interview**
- Focus on fundamentals and communication
- Provide entry-level interview prep roadmap
- Practice behavioral questions with STAR method

**Scenario 2: Senior Engineer Targeting Staff Role**
- Emphasize system design interviews
- Practice leadership and influence questions
- Deep dive into architecture trade-offs

**Scenario 3: Hiring Manager Building Interview Process**
- Generate role-specific question bank
- Establish evaluation criteria
- Calibrate interview difficulty across team
