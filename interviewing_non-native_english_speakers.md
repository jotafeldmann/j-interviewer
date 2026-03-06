# Interviewing Non-Native English Speakers

Auhtor: Jorge Feldmann
AI fair usage: drafted with Claude, edited by the author.

## Core Principle

Separate language fluency from technical reasoning. Unless the role requires advanced client-facing English, technical ability should remain the primary signal.

⚠️ Main goal: **Evaluate reasoning quality — not accent, speed, or verbosity.**

---

## 1. Hesitation, Pauses, and Fillers

**Common Signals**
- Long pauses before answering
- "Uh…", "So…", "Let me think…"
- Restarting sentences

**Example**

> *Interviewer:* "How would you detect a cycle in a graph?"
> *Candidate:* "So… uh… we can maybe… I mean… we could use… DFS and… keep track of visited… nodes…"

**What to Evaluate**
- Is the algorithm correct?
- Is the reasoning coherent once expressed?

**Helpful Prompts**
- "Take your time."
- "Walk me through it step by step."

---

## 2. Wavering / Over-Softening

**Common Signals**
- "I think maybe…"
- "Perhaps we could…"
- Correct answers framed as guesses

**Example**

> *Candidate:* "Maybe we could add an index on that column… I'm not sure but I think that would improve performance."
> *(They are correct — indexing is the right solution.)*

**What to Evaluate**
- Is the solution technically sound?
- Can they justify the choice when asked?

**Helpful Prompts**
- "Would you choose that approach?"
- "If you had to decide, what would you implement?"

---

## 3. Short or Minimal Explanations

**Common Signals**
- Brief answers
- No mention of trade-offs
- No edge cases discussed

**Example**

> *Interviewer:* "How would you design a URL shortener?"
> *Candidate:* "We need a database, generate unique IDs, map them to URLs."

**Before Concluding, Ask:**
- "What happens if two users generate at the same time?"
- "How would this scale to millions of requests?"
- "What are the bottlenecks?"

Often depth appears after prompting.

---

## 4. Vocabulary Gaps

**Common Signals**
- Describing around a term
- Slightly incorrect terminology

**Example**

> *Candidate:* "If two threads try to change the value at the same time… it can… conflict and cause incorrect result."
> *(They mean a race condition.)*

**Helpful Intervention**

"Do you mean a race condition?" — then continue evaluating their understanding of concurrency.

**What to Evaluate**
- Do they understand synchronization strategies?
- Can they explain prevention mechanisms?

---

## 5. Slower Verbal Problem Solving

**Common Signals**
- Writing first, speaking later
- Long pauses before discussing trade-offs

**Example**

> Candidate silently writes pseudo-code for 90 seconds, then explains clearly.

**What to Evaluate**
- Structure of solution
- Correctness
- Edge case handling

Avoid interrupting mid-thought.

---

## 6. Literal Interpretation of Questions

**Common Signals**
- Answering exactly what was asked
- Missing implied expansion

**Example**

> *Interviewer:* "Would this scale?"
> *Candidate:* "Yes." *(They interpret it literally.)*

**Better Prompts**
- "Assume traffic increases 100x. What breaks?"
- "What would you redesign to handle global usage?"

---

## 7. Reduced Small Talk or Warmth

**Common Signals**
- Formal tone
- Minimal personal anecdotes
- Limited casual back-and-forth

**Example**

> *Interviewer:* "How was your weekend?"
> *Candidate:* "It was good. I studied distributed systems."

Do not equate extroversion with team fit.

**Evaluate Instead**
- Do they collaborate during problem solving?
- Do they respond well to hints?
- Do they adjust when constraints change?

---

## 8. Confidence Signals May Look Different

**Common Signals**
- Softer voice
- Less eye contact
- Not challenging assumptions

**Example**

> Interviewer introduces a flawed constraint. Candidate proceeds without questioning it.

**Probe**
- "Do you see any issue with this assumption?"
- "Would you change any requirement?"

Evaluate technical judgment when explicitly invited.

---

## Structured Interview Adjustments

### Use Explicit Prompts

Instead of: "Is this good?" / "Would this work?"

Ask:
- "What are the trade-offs?"
- "What are the bottlenecks?"
- "How would this behave under high concurrency?"

### Normalize Clarification

Early in the interview: *"Feel free to ask me to repeat or rephrase anything."*

### Encourage Visual Thinking

Allow diagrams, pseudo-code, and structured bullet reasoning. Written clarity often exceeds spoken fluency.

### Probe Before Scoring

If an answer feels shallow, ask:
1. One depth follow-up
2. One constraint-based follow-up
3. One trade-off follow-up

Only then evaluate depth.

### Separate Scoring Dimensions

Score independently:
- Problem solving
- System design
- Code quality
- Trade-off reasoning
- Collaboration
- Communication clarity *(only weighted according to role needs)*

Do not blend fluency into technical scoring unless explicitly required.

---

## Strong Signals That Transcend Language

Regardless of English fluency, strong candidates:

- Break down problems clearly
- Identify constraints
- Discuss trade-offs
- Surface edge cases
- Adapt to new information
- Ask clarifying questions
- Maintain logical consistency

