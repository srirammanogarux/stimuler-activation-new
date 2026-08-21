# Activation cohorts

**Step 1 of three: the cohorts.** Settled at eight. Subgoals live in
[SUBGOALS.md](SUBGOALS.md); the activation event per cohort comes after.

Nothing here is in the build yet.

---

## The funnel

The sequence. Everything resolves before the level step.

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
five are in the current flow but absent from the sequence above.

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

> **Open contradiction.** The source doc says IELTS Speaking is identical for
> Academic and General, so *do not branch the task on it*. The brief says
> Academic and General have different jobs to be done. These reconcile if the
> **task** stays shared and only the **subgoal list** differs — written that way
> throughout, but confirm before anything is built on it.

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
| **Personal** | C5 | C5 | C5 | C5 | **C8** | C5 | C5 |
| **Travel** | C6 | C6 | C6 | C6 | C6 | C6 | C6 |
| **School** | **C7** | C7 | C7 | C7 | C7 | C7 | C7 |
| **Other** | → | → | → | → | → | → | → |

Career is the only row that splits, three ways, on your relationship to the job:
don't have it yet → **C2**, already have it → **C3**, *are* it → **C4**.

**Coverage: 35 of 42 boxes.** Only the Other row is unresolved.

> **Box count is not user volume.** C3 occupies a single box and is probably the
> largest cohort in the product. C8 also occupies a single box and is probably
> one of the smallest. Do not read the grid as a sizing map.

---

## The eight cohorts

| # | Cohort | Judge | Scoreboard | Question |
|---|---|---|---|---|
| C1 | Exam | An examiner with a rubric and a clock | Band estimate vs target | "Describe a place you often visit." |
| C2 | Interview | A hiring manager deciding in real time | Would this survive the room | "So, why should we hire you?" |
| C3 | At Work | Colleagues who already hired you | Clarity, no rambling | "What are you working on right now?" |
| C4 | Own Boss | A customer deciding whether to hire you | Would they choose you | "Tell me about your business." |
| C5 | Belonging | Nobody — and that is the problem | Fillers, dead air, time to first word | "What do you like doing in your free time?" |
| C6 | Travel | A stranger with thirty seconds | Were you understood | "Where are you from?" |
| C7 | School | A teacher and a room of classmates | Were you followed | "Tell me about something you're studying." |
| C8 | Household | An institution with a queue behind you | Did you get what you came for | "Is there anything you'd like to ask me?" |

The judge is the load-bearing idea: it determines the question that makes sense,
what "good" means, what number we show, and what the paywall sells.

Occupation never picks the question. It swaps one line in C2 and C8, sets the
room in C5, and writes the plan and paywall story everywhere.

C1–C6 are unchanged from the source doc. The two new ones are specified below.

---

## C7 — School

**Goal:** Excel at my school · **Occupation:** all seven
**Judge:** a teacher and a room of classmates
**Scoreboard:** were you followed — clarity in an academic setting

### The scenario

This person is not being admitted and not being hired. They are being *formed a
view of* — daily, by a teacher who calls on them and classmates who notice who
speaks. The failure is knowing the answer and letting someone else give it.

Structurally this is C3 for people who do not have a job yet: the room already
knows you, and the question is about your own work.

Deliberately generic. No assumption of an oral exam, a campus social life, a
subject, or an age — it has to work for a school student and a university
student alike.

### The question

> **"Tell me about something you're studying right now."**

| step | the learner says |
|---|---|
| Name it | This year I am studying biology. |
| Say what part | Right now we are learning how plants make food. |
| Give a detail | Last week we did an experiment with some leaves. |
| Say what you think | I understand it better when we do it ourselves. |

**Drilled:** *studying* · *experiment*

### Why this question

It is the question a student's life asks constantly — by teachers, by relatives,
by every new classmate. It is answerable cold with no role to adopt, it is warm
rather than adversarial, and the model answer demonstrates the cure: four
sentences where the failure mode is one.

---

## C8 — Household

**Goal:** Personal growth · **Occupation:** homemaker
**Judge:** an institution with a queue behind you — a teacher, a receptionist, a clerk
**Scoreboard:** did you get what you came for

### The scenario

This person runs the household and deals with institutions on the family's
behalf: the school office, the clinic, the bank, the parent-teacher meeting.

The failure is specific and costly. Asked whether they have any questions, they
say "no, it's fine" — and leave without the thing they came for. Often the
workaround is having a child translate, which is exactly the dependency they
want to end.

Unlike C5 there *is* a judge, and unlike C6 the stakes are someone else's
welfare rather than their own convenience.

### The question

> **"Is there anything you'd like to ask me?"**

| step | the learner says |
|---|---|
| Say that you do | Yes, actually, I do have one question. |
| Say what it is about | It is about the homework she gets. |
| Give the detail | She spends about two hours on it every night. |
| Ask it directly | Is that normal for her age? |

**Drilled:** *question* · *hours*

### Occupation swaps

Not every household runs a child. Same cohort, same scoring, one line different:

| Situation | Lines 2–4 |
|---|---|
| Has children | *(default — about the child's schooling)* |
| No children | "It is about the appointment I booked… I have been waiting about three weeks… Is there anything sooner?" |

### Why this question

It is the exact moment of failure rather than a description of it, and it is
asked at every institution — school, clinic, bank, office. It is answerable
cold, it requires no role to adopt, and the model answer does the one thing the
user does not do: it asks.

---

## Open decisions

### Other is free text — how does it route?

Free text still has to reach a cohort. Unresolved, and the last hole in the
grid. Cheapest honest option is a single follow-up question after the text
field; the most ambitious is matching the text against the eight cohorts.

---

## Still to come

2. Subgoals per cohort → [SUBGOALS.md](SUBGOALS.md)
3. The activation event per cohort
