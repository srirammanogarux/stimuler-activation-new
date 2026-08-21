# Activation cohorts

Working doc for **step 1: converge on the cohorts.** Subgoals and the activation
event come after this is settled, not before.

Nothing here is in the build yet.

---

## The funnel

The sequence, as described. Everything resolves before the level step.

```
1  Native language
2  Source            App Store · Play Store · Facebook · friends · TikTok
                     Google Ads · YouTube · Instagram Reels
3  Age               under 18 · 18–24 · 25–34 · 35–44 · 45+
4  Current situation the 7 occupations below
5  Goal              the 6 goals below
   └─ if Exam        which exam → IELTS goes deeper, others capture only
6  Level
7  Activation event
```

**New steps:** age and current situation. Neither exists in the flow today.

**Not yet placed:** app language, name, phone, testimonials, notifications. All
five are in the current flow but absent from the sequence above — they need a
home before this becomes a build.

---

## Goals

Renamed. `other` stops being an option list and becomes a free-text field.

| Key | Name | Was |
|---|---|---|
| `exam` | Prepare for an English Exam | IELTS |
| `career` | Grow in my career | Improve my career |
| `personal` | Personal growth | Everyday conversations |
| `school` | Excel at my school | *(unchanged)* |
| `travel` | Travel confidently | Travel |
| `other` | *free text* | Any other goal |

### The Exam branch

Exam is the only goal that branches. Which exam changes the **task**, because
the speaking formats genuinely differ.

| Exam | Speaking format | Depth |
|---|---|---|
| IELTS | 2-min cue-card monologue + examiner follow-ups | Full sub-flow |
| TOEFL | 45-sec responses to a screen, no interlocutor | Capture only |
| PTE | Repeat sentence, describe image, retell lecture | Capture only |
| TOEIC | Read aloud, describe a photo, respond to prompts | Capture only |
| Other | — | Capture only |

IELTS alone goes deeper:

- **Academic / General / not sure** — intent signal
- **Timing** — within a month · within 2 months · more than 2 months
- **Target band**

> **Open contradiction.** The cohorts doc says IELTS Speaking is identical for
> Academic and General, so *do not branch the task on it*. The brief says
> Academic and General have different jobs to be done. These reconcile if the
> **task** stays shared and only the **subgoal list** differs — but that needs
> confirming before anything is built on it.

---

## Occupations

Seven segments, asked as "current situation".

`student` · `working professional` · `freelancer` · `business owner` ·
`homemaker` · `career break` · `looking for work`

---

## The grid

6 goals × 7 occupations = **42 boxes.** Each box tested with one question:
*would this person be asked a different question, by a different judge?*

| Goal | Student | Working | Freelance | Owner | Homemaker | Break | Job-seeking |
|---|---|---|---|---|---|---|---|
| **Exam** | C1 | C1 | C1 | C1 | C1 | C1 | C1 |
| **Career** | C2 | C3 | C4 | C4 | C2 | C2 | C2 |
| **Personal** | C5 | C5 | C5 | C5 | C5 ⚠ | C5 | C5 |
| **Travel** | C6 | C6 | C6 | C6 | C6 | C6 | C6 |
| **School** | ? | ? | ? | ? | ? | ? | ? |
| **Other** | → | → | → | → | → | → | → |

Career is the only row that splits, three ways, on your relationship to the job:
don't have it yet → **C2**, already have it → **C3**, *are* it → **C4**.

**Coverage: 28 of 42 boxes.** School (7) and Other (7) have no cohort — a third
of the grid. That is the main thing left to close.

---

## The six cohorts

| # | Cohort | Judge | Scoreboard | Question |
|---|---|---|---|---|
| C1 | Exam | An examiner with a rubric and a clock | Band estimate vs target | "Describe a place you often visit." |
| C2 | Interview | A hiring manager deciding in real time | Would this survive the room | "So, why should we hire you?" |
| C3 | At Work | Colleagues who already hired you | Clarity, no rambling | "What are you working on right now?" |
| C4 | Own Boss | A customer deciding whether to hire you | Would they choose you | "Tell me about your business." |
| C5 | Belonging | Nobody — and that is the problem | Fillers, dead air, time to first word | "What do you like doing in your free time?" |
| C6 | Travel | A stranger with thirty seconds | Were you understood | "Where are you from?" |

The judge is the load-bearing idea: it determines the question that makes sense,
what "good" means, what number we show, and what the paywall sells.

Occupation never picks the question. It swaps one line in C2, sets the room in
C5, and writes the plan and paywall story everywhere.

---

## Open decisions

### 1. School needs to be generic — proposal: make it C7

Dissolving School into "oral exam" (C1) and "campus social" (C5) is too
specific, and it leaves 7 boxes homeless. But School passes the judge test on
its own terms:

- **Judge:** a teacher and a room of classmates — people who already know you and
  are not deciding whether to admit you, but are forming a view of you
- **Scoreboard:** clarity in an academic setting — were you followed
- **Question, generic across ages and subjects:** *"Tell me about something
  you're studying right now."*

That is deliberately broad. It works for a school student and a university
student, any subject, with no assumption of an exam or a campus social life.

Structurally it is C3 for people who don't have a job yet — same shape, genuinely
different judge and question.

**Note:** a student picking Career still goes to C2. School is for students whose
goal is the studying itself.

### 2. Other is free text — how does it route?

Free text has to reach a cohort somehow. Unresolved. The cheapest honest option
is a single follow-up question after the text field; the most ambitious is
matching the text against the six cohorts.

### 3. Personal growth × homemaker — proposal: not a cohort

Flagged in the source doc as a possible seventh: *"handle the school and the
clinic myself, without my child translating"* — different judge (an institution),
different stakes (someone else's welfare), often a phone call.

It is a real situation, but it does not split on **goal or occupation**, which is
what a cohort is made of. Anyone in a new country handles clinics, banks,
landlords and schools — a working professional as much as a homemaker. What
makes it distinct is the *situation*, and situations are what the subgoal layer
encodes.

So: leave it inside C5 for now and let it resurface as a subgoal, rather than
bending the cohort model around one box.

---

## Still to come

2. Subgoals per cohort
3. The activation event per cohort
