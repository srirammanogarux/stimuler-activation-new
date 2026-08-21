# What v1 actually had — the full JTBD inventory

Reference, not a proposal. Extracted from
[srirammanogarux/usa-onboarding](https://github.com/srirammanogarux/usa-onboarding)
`content.js` — `GOALS[].jtbd`, `JTBD_MODE`, `OCC_EXTRA`.

**47 distinct labels · 9 families · 17 lists.**

---

## How the 47 got there

Occupation collapses to a **work mode** (8 → 7), and only two goals define
mode overrides. The rest show one list to everyone.

| Goal | Base list | Mode overrides |
|---|---:|---|
| `ielts` | 3 | none |
| `career` | 5 | ownboss (4) · jobhunt (4) · student (3) · athome (4) · careerbreak (4) |
| `convo` | 4 | ownboss (4) · student (3) · athome (4) · jobhunt (4) · careerbreak (4) · office (4) |
| `travel` | 3 | none |
| `school` | 4 | none |
| `other` | 4 | none |

**17 lists in total**, and no user ever sees more than 5 options.

> **The important part.** Most of the 47 are not different jobs. They are the
> *same job re-worded for a persona*. Under `interview`: "Ace a job interview",
> "Land an internship", "Speak up in interviews" and "Start working again" are
> one job in four voices — job-seeker, student, student again, homemaker. Under
> `smalltalk`, "Make friends on campus", "at the school gate", "at a new
> workplace" and "while traveling" are one job in four settings.
>
> Deduplicated by actual work, **47 labels are roughly 18–20 distinct jobs** —
> which is exactly why the copy resolves to 20 `goal|family` pairs.

---

## The 47, by family

### `interview` — 9

| Label | Where it appears |
|---|---|
| Ace a job interview | career base · jobhunt · careerbreak |
| Answer "tell me about yourself" | career/jobhunt |
| Explain a gap in my CV | career/careerbreak |
| Land an internship | career/student |
| Speak up in interviews | career/student |
| Start working again | career/athome |
| Talk about skills I built at home | career/athome |
| Talk to my boss with confidence | career base |
| Be ready when opportunity knocks | other base |

### `smalltalk` — 14

| Label | Where it appears |
|---|---|
| Make small talk feel natural | convo base · ownboss · student · jobhunt · office |
| Meet new people and make friends | convo base · jobhunt · careerbreak |
| Meet new people at events | convo/ownboss |
| Make friends on campus | school base · convo/student |
| Make friends at the school gate | convo/athome |
| Make friends at a new workplace | career/athome |
| Make friends while traveling | travel base |
| Chat with colleagues outside work | convo/office |
| Get back into everyday chat | convo/careerbreak |
| Handle work small talk again | career/careerbreak |
| Network on campus | career/student |
| Network to find openings | career/jobhunt |
| Speak without overthinking | other base |
| Start conversations anywhere | other base |

### `pitch` — 5

| Label | Where it appears |
|---|---|
| Win a new client | career/ownboss |
| Explain and defend my price | career/ownboss |
| Chase a late payment | career/ownboss |
| Pitch on a client call | OCC_EXTRA: freelancer |
| Negotiate the offer | career/jobhunt |

### `fastspeech` — 5

| Label | Where it appears |
|---|---|
| Understand fast coworkers | career base |
| Understand fast clients | career/ownboss |
| Understand fast native audio | ielts base |
| Keep up with fast lectures | school base |
| Understand native speakers at full speed | other base |

### `services` — 4

| Label | Where it appears |
|---|---|
| Handle doctors and offices solo | convo base · ownboss · student · jobhunt · careerbreak · office |
| Talk to teachers and doctors solo | convo/athome |
| Breeze through airports and hotels | travel base |
| Sort out any mix-up abroad | travel base |

### `exam` — 3

| Label | Where it appears |
|---|---|
| Pass the speaking test | ielts base |
| Speak two minutes without freezing | ielts base |
| Pass my speaking exam | school base |

### `meetings` — 3

| Label | Where it appears |
|---|---|
| Speak up in meetings | career base · athome |
| Speak up in meetings again | career/careerbreak |
| Speak up in class discussions | school base |

### `customer` — 2

| Label | Where it appears |
|---|---|
| Handle customer calls | career base |
| Handle a walk-in customer | OCC_EXTRA: business |

### `family` — 2

| Label | Where it appears |
|---|---|
| Win over my partner's family | convo base · ownboss · athome · jobhunt · office |
| Support my kids at school | convo/athome · careerbreak |

---

## What v1 has that the current 31 does not

Adopt candidates, strongest first.

| v1 label | Where it would go | Why it earns a place |
|---|---|---|
| **Win over my partner's family** | C5 | In-laws. Emotionally the biggest job in the whole v1 set and we have nothing like it. |
| **Talk about skills I built at home** | C2 | The *positive* framing of the gap. We only have "explain my gap", which is defensive. |
| **Chase a late payment** | C4 | Very real for freelancers, and a `request` act — which C4 currently lacks. |
| **Negotiate the offer** | C2 | A `disagree` act in an interview, which C2 currently lacks. |
| **Make friends at the school gate** | C8 | The one v1 label written for the homemaker's social world. |
| **Handle a walk-in customer** | C4 | Business owners only. v1 kept it as an `OCC_EXTRA` prepend rather than a list item. |
| **Land an internship / Network on campus** | C7 or C2 | Student-specific career jobs we route to a generic C2. |

---

## What the current 31 has that v1 does not

**Conflict.** Almost every v1 job is *presenting yourself well* — introduce,
explain, pitch, befriend. Only 3 of 47 involve holding ground: "Explain and
defend my price", "Negotiate the offer", "Chase a late payment". There is
nothing about being refused, contradicted, or having to insist.

The current set adds `disagree` and `repair` as first-class acts: push back on a
plan, flag a problem early, handle an unhappy customer, push back when told no,
disagree with a classmate.

Also new: C1 split by exam part rather than one lump; C8 as a real cohort where
v1 had two `family` labels.

---

## The technique worth stealing

v1 personalises the **label**, not the job. `career|interview` is one job that
speaks four ways depending on who is reading it.

The cohort model currently drops this — everyone routing to C2 sees the same
four labels, so a student and a returning parent read identical copy.

That is a copy layer, not a structural change: keep the 31 jobs and let
occupation re-word them. Cheap, and it recovers the thing that makes the v1 set
feel written for you.

| Job | `jobseek` | `student` | `homemaker` |
|---|---|---|---|
| Tell my story without rambling | Answer "tell me about yourself" | Talk about myself in an interview | Talk about the skills I built at home |

---

## One thing to decide

`fastspeech` is 5 of v1's 47 and reachable from five of six goals — one of the
most-offered jobs in the product. The current set drops it entirely as a
listening problem that needs no microphone.

That is either the right call or the biggest omission in the set. Worth settling
explicitly rather than by default.
