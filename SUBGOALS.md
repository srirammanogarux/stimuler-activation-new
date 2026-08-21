# Subgoals — jobs to be done, per cohort

**Step 2 of three.** Built on the eight cohorts in [COHORTS.md](COHORTS.md).

Nothing here is in the build yet.

---

## The budget is pairs, not jobs

Taken from how v1 converged — see `onboarding-form/docs/BRANCHING.md`.

v1 shows **47 distinct JTBD labels**. It does not author 47 variants. Each label
carries a `fam`, an internal **family** key the user never sees, and the copy is
keyed on `goal|family` — because the same family means different things under
different goals. That gives 20 reachable pairs, and only **12 need bespoke copy**.
The rest fall through:

```
PLAN_GF['goal|family']  →  the family map  →  the 'smalltalk' fallback
```

So the count that costs anything is **pairs**, not options. The label is free and
should stay concrete. The pair is expensive and should stay capped.

**Applied here:** the cohort already carries what `goal|mode` carried in v1, so
the key is `cohort|family`. **32 jobs resolve to 11 pairs.** That is the number
to hold, and it is already inside the v1 budget.

---

## What makes a subgoal work

1. **It is a situation.** A moment with a room, a person and a stake — not a
   skill. "Speak up in meetings", never "improve fluency".
2. **The user has lived it.** They should recognise a specific time it went
   badly. Recognition is what makes the pick feel personal.
3. **It stays inside its cohort's judge.** Every job below is a variation on one
   judge's world. A job implying a different judge belongs to a different cohort.
4. **It carries a family.** The label is written for a human; the family is
   written for the copy system. Never show the family.

Each cohort gets **four**. Four scans in a chat bubble; five reads like a form.
Order matters — the first option takes a disproportionate share of picks.

---

## The families

Eight, adapted from v1's nine. `customer` folds into `pitch` and `services`;
`fastspeech` is dropped as out of activation scope; `fluency` is new.

| Family | What it is |
|---|---|
| `exam` | Timed, scored, against a rubric |
| `fluency` | The internal blocker — freezing, fillers, dead air |
| `interview` | Evaluated by one person who is deciding about you |
| `meetings` | Speaking into a group that already knows you |
| `pitch` | Selling your own work, price or worth |
| `smalltalk` | Opening and sustaining talk with no agenda |
| `services` | A transactional exchange to get something done |
| `family` | Speaking for your family to someone who holds something they need |

---

## C1 — Exam
Judge: an examiner with a rubric and a clock.

| # | Job to be done | Family |
|---|---|---|
| 1 | Get through the long turn without drying up | `exam` |
| 2 | Answer the follow-ups without one-word replies | `exam` |
| 3 | Cut the pauses and fillers that cost marks | `fluency` |
| 4 | Sound natural instead of memorised | `fluency` |

**How this varies by exam.** The judge never changes, so the cohort holds. Job 1
is format-specific:

| Exam | Job 1 becomes |
|---|---|
| IELTS Academic | Get through the long turn without drying up |
| IELTS General | Talk about everyday topics without running short |
| TOEFL | Answer in 45 seconds with no time to plan |
| PTE | Repeat and retell without losing the thread |
| TOEIC | Read aloud and describe a photo without stumbling |

Jobs 2–4 hold across all five. Academic and General differ in the *topics* they
sustain — abstract versus everyday — which is a copy difference inside one pair,
not a new pair.

## C2 — Interview
Judge: a hiring manager deciding in real time.

| # | Job to be done | Family |
|---|---|---|
| 1 | Answer "why should we hire you" without hedging | `interview` |
| 2 | Explain a gap in my history without apologising | `interview` |
| 3 | Talk about what I am good at without shrinking | `interview` |
| 4 | Ask my own questions at the end | `interview` |

Job 2 earns its place for `career break`, `homemaker` and `looking for work` —
the three occupations that route here carrying a gap.

## C3 — At Work
Judge: colleagues who already hired you.

| # | Job to be done | Family |
|---|---|---|
| 1 | Give my update without rambling | `meetings` |
| 2 | Explain my work to someone outside my team | `meetings` |
| 3 | Disagree without sounding rude | `meetings` |
| 4 | Say I need more time, or help | `meetings` |

## C4 — Own Boss
Judge: a customer deciding whether to hire you.

| # | Job to be done | Family |
|---|---|---|
| 1 | Say what my business does in one breath | `pitch` |
| 2 | Say my price without softening it | `pitch` |
| 3 | Answer "why are you more expensive?" | `pitch` |
| 4 | Follow up without sounding desperate | `pitch` |

`freelancer` reads "my work" for "my business" throughout.

## C5 — Belonging
Judge: nobody, and that is the problem.

| # | Job to be done | Family |
|---|---|---|
| 1 | Say more than three words and stop | `smalltalk` |
| 2 | Keep it going past the first exchange | `smalltalk` |
| 3 | Join a group that is already talking | `smalltalk` |
| 4 | Talk to someone new without rehearsing first | `smalltalk` |

## C6 — Travel
Judge: a stranger with thirty seconds.

| # | Job to be done | Family |
|---|---|---|
| 1 | Be understood the first time | `services` |
| 2 | Ask a stranger for help without freezing | `services` |
| 3 | Sort it out when something goes wrong | `services` |
| 4 | Keep chatting after the practical part is done | `smalltalk` |

## C7 — School
Judge: a teacher and a room of classmates.

| # | Job to be done | Family |
|---|---|---|
| 1 | Answer when the teacher calls on me | `meetings` |
| 2 | Explain my work to the class | `meetings` |
| 3 | Ask a question without feeling stupid | `meetings` |
| 4 | Hold my part in a group project | `meetings` |

Job 3 is the quiet one and probably the most common. Students do not ask because
asking exposes them twice — once for not knowing, once for how they sound.

## C8 — Household
Judge: a professional who holds something the family needs.

| # | Job to be done | Family |
|---|---|---|
| 1 | Speak up at a parent-teacher meeting | `family` |
| 2 | Handle the school office on my own | `services` |
| 3 | Get through a clinic or doctor visit | `services` |
| 4 | Sort out a bill, a bank, or an office problem | `services` |

---

## The pairs

Every job resolves here. This is the build list.

| # | Pair | Jobs | Means |
|---|---|---:|---|
| 1 | `C1\|exam` | 2 | Under the clock, against a rubric |
| 2 | `C1\|fluency` | 2 | The freezing that costs marks |
| 3 | `C2\|interview` | 4 | Claiming competence while being judged for it |
| 4 | `C3\|meetings` | 4 | Being listened to by people who already hired you |
| 5 | `C4\|pitch` | 4 | Selling your own worth |
| 6 | `C5\|smalltalk` | 4 | Talk with no agenda and no judge |
| 7 | `C6\|services` | 3 | Being understood by an impatient stranger |
| 8 | `C6\|smalltalk` | 1 | The warm bit after the practical bit |
| 9 | `C7\|meetings` | 4 | Being followed by a teacher and a room |
| 10 | `C8\|family` | 1 | Speaking for your child |
| 11 | `C8\|services` | 3 | Institutions, on your own |

**32 jobs → 11 pairs.** Inside v1's budget of 12.

`meetings` appears twice and `smalltalk` twice, under different cohorts — which
is the whole reason the key is `cohort|family` and not family alone. Being
followed by classmates is not being listened to by colleagues.

With a v1-style fallback chain, several of the eleven could resolve to a family
default rather than bespoke copy. That decision belongs to step 3, once we know
what the activation event does with the pick.

---

## What is deliberately absent

**`fastspeech`** — "understand fast speakers", "keep up with fast lectures". One
of the most commonly named problems, and reachable from five goals in v1. Left
out because it is a *listening* problem served by a speaking task, and it needs
no microphone — which per the source doc makes it the natural fallback for
anyone who abandons at the mic. A feature, not a subgoal.

**Interject** — "speak up in meetings", "answer in class". No longer homeless:
C3 job 1 and C7 job 1. The activation event does not test it, since breaking
into a conversation needs audio to break into, but the user can still name it.

---

## Counts

| | |
|---|---|
| Cohorts | 8 |
| Jobs to be done | 32 |
| Families | 8 |
| `cohort\|family` pairs | 11 |
| Activation questions | 8, plus 4 exam format variants |

---

## Still to come

3. The activation event per cohort — what happens after the pick.
