# Activation subgoals — jobs to be done

> ⚠️ **Superseded pending cohort convergence.** This draft was built goal-first.
> The model has since moved to **cohort-first** (`goal × occupation`), goals have
> been renamed, and Exam has become a branch rather than a leaf. Roughly half the
> jobs below are affected — `meetings`, `presentation` and `fastspeech` are ruled
> out of activation scope, and School yields no cohort of its own. Kept for the
> family analysis and the four-part test, both of which still hold. Rewrite comes
> after the cohorts are settled.

Draft for review. **Nothing here is in the build yet.**

One question after the goal. The user picks a single situation they want to gain
confidence in, and that pick is what the activation experience gets built around.

Starting point: the `GOALS` block in
[srirammanogarux/usa-onboarding](https://github.com/srirammanogarux/usa-onboarding)
· `content.js:78`, where it is called JTBD.

| | |
|---|---|
| Goals | 6 |
| Jobs to be done | 30 |
| Content families | 9 |
| Options per goal | 5 |

---

## What makes a subgoal work

The test these were written against. Anything that fails one of the four is a
category, not a job.

1. **It is a situation.** A moment with a room, a person and a stake — not a
   skill. "Speak up in meetings", never "improve fluency".
2. **The user has lived it.** They should recognise a specific time it went
   badly. Recognition is what makes the pick feel personal.
3. **One experience fits it.** You can build a single focused practice around it.
   If it needs three, it is still a goal.
4. **It beats its neighbours.** Distinct enough that picking it rules the others
   out. Overlapping options make the choice feel arbitrary.

---

## The six goals

Order matters — the first option takes a disproportionate share of picks, so each
list opens with the most-wanted situation for that goal. **Bold** families are
ones the USA set does not have.

### IELTS — `ielts`

| # | Job to be done | Family |
|---|---|---|
| 1 | Get through the two-minute long turn | `exam` |
| 2 | Hold my own in the Part 3 discussion | `exam` |
| 3 | Stop freezing in the middle of an answer | **`fluency`** |
| 4 | Keep up with fast native audio | `fastspeech` |
| 5 | Sound natural instead of rehearsed | **`fluency`** |

### Improve my career — `career`

| # | Job to be done | Family |
|---|---|---|
| 1 | Ace a job interview | `interview` |
| 2 | Speak up in meetings | `meetings` |
| 3 | Present to a room without freezing | **`presentation`** |
| 4 | Network without going blank | `networking` |
| 5 | Talk to my manager with confidence | `interview` |

### Everyday conversations — `daily`

| # | Job to be done | Family |
|---|---|---|
| 1 | Make small talk feel natural | `networking` |
| 2 | Meet new people and make friends | `networking` |
| 3 | Handle appointments and offices on my own | `services` |
| 4 | Keep up when people talk fast | `fastspeech` |
| 5 | Talk easily with my partner's family | `family` |

### Travel — `travel`

| # | Job to be done | Family |
|---|---|---|
| 1 | Get through airports and hotels | `services` |
| 2 | Order and shop with confidence | `services` |
| 3 | Sort out a mix-up when plans break | `services` |
| 4 | Make friends on the road | `networking` |
| 5 | Understand fast local English | `fastspeech` |

### Excel at my school — `school`

| # | Job to be done | Family |
|---|---|---|
| 1 | Pass my speaking exam | `exam` |
| 2 | Speak up in class discussions | `meetings` |
| 3 | Present my project to the class | **`presentation`** |
| 4 | Keep up with fast lectures | `fastspeech` |
| 5 | Make friends on campus | `networking` |

### Any other goal — `other`

| # | Job to be done | Family |
|---|---|---|
| 1 | Speak without overthinking every word | **`fluency`** |
| 2 | Start a conversation with anyone | `networking` |
| 3 | Understand native speakers at full speed | `fastspeech` |
| 4 | Stop translating in my head first | **`fluency`** |
| 5 | Be ready when the opportunity comes | `interview` |

---

## Where the build weight lands

Thirty options is thirty only on the screen. Underneath they resolve to nine
families, and a family is what you actually build once.

| Family | Jobs | Fed by |
|---|---:|---|
| `networking` | 6 | career · daily ×2 · travel · school · other |
| `fastspeech` | 5 | ielts · daily · travel · school · other |
| `services` | 4 | daily · travel ×3 |
| `fluency` | 4 | ielts ×2 · other ×2 |
| `exam` | 3 | ielts ×2 · school |
| `interview` | 3 | career ×2 · other |
| `meetings` | 2 | career · school |
| `presentation` | 2 | career · school |
| `family` | 1 | daily |

Three families — `networking`, `fastspeech` and `services` — absorb half of every
pick. Build those three properly and the majority of users meet a well-made
experience on their first run.

`family` sits at one job and is the obvious candidate to merge into `networking`
or cut.

---

## How this differs from the USA set

The USA JTBD block holds up. These are the deliberate departures.

**Added**

- **`presentation`** — sustained solo talk to a room. It was in your own
  workplace example and the USA set has no family for it; a presentation is not
  a meeting.
- **`fluency`** — the internal blocker rather than a room. Freezing,
  overthinking, translating in your head. It breaks rule 1 above by not being a
  situation, but it is what most learners name first when asked what stops them,
  so it is here to be argued about rather than quietly dropped.

**Merged**

- `customer` and `pitch` folded into `services` and `interview`. Both existed in
  the USA file only to serve the work-mode branch, which activation does not have.
- `smalltalk` renamed `networking` — same family, but the name now covers the
  work-event case as well as the neighbour case.

**Held back**

- No country variation yet, per your call. The situations are written to travel;
  if Mexico needs its own cut, that is a pass after this one.
- No Spanish yet — worth translating once the English is settled rather than twice.

---

## Open questions

1. **Does the family drive a different experience, or only different copy?**
   Nine families means nine practice experiences to build. If the subgoal only
   personalises Sarah's wording and the practice stays the same, this is a small
   build. If each family gets its own activation moment, it is the whole project.
2. **Five options, or fewer?** Five is a lot to read in a chat bubble on a phone.
   Four scans faster and pushes the fifth into a catch-all. I would cut to four
   per goal if you want the step to feel quick.
3. **Does IELTS keep its own shape?** IELTS users arrive with an exam date and a
   target band. Its subgoals are exam mechanics rather than life situations,
   which may argue for a different treatment than the other five goals.
4. **Should the pick be visible later in the flow?** The strongest version calls
   back to it — the speech meter, the graph and the paywall headline all naming
   the situation the user chose. That is a bigger change than the subgoal step
   itself.

---

## Where it goes in the flow

Between the goal step and the testimonials, which are unchanged.

```
… → goal → SUBGOAL (new) → testimonials → notifications → level → reading test → …
```

The reading test is untouched and stays that way until we get to it.
