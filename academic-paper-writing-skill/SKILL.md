---
name: academic-paper-writing
description: |
  Guides AI agents to write high-quality academic papers following top-tier conference standards, based on the "From Engineering Implementation to Scientific Argument" methodology.
  
  Use this skill when:
  - Writing or drafting academic papers for AI/systems conferences
  - Designing paper structure, sections, or experimental methodology
  - Structuring motivation, insight, and design narrative
  - Creating figures, tables, or data visualizations for papers
  - Performing literature review or managing citations
  - Responding to reviewer comments or preparing rebuttal
  - Any task involving academic writing workflow
  
  Do NOT use for:
  - Non-academic writing (blogs, marketing copy, documentation)
  - Papers outside AI/systems domains without adaptation
  - Simple formatting tasks that don't require domain expertise
---

# Academic Paper Writing

From Engineering Implementation to Scientific Argument.

## Core Philosophy

**Writing = Building Arguments, Not Recording Work**

Papers must construct an irrefutable argument system, not simply document what was done. The goal: make reviewers conclude "this problem is important, this method is sound, these results are credible."

> Papers are judged by how hard they are to reject.

Common misconceptions:
- ❌ "I did a lot → should be recognized"
- ❌ "Many experiments → should be accepted"
- ❌ "Complex implementation → should be impressive"

### The Argument Loop

```
Observation → Insight → Design → Evidence
```

Every section must form a verifiable takeaway (clear takeaway) that closes this loop.

## Research vs Writing Logic

### Thinking Pipeline (Chaotic Exploration)

```
Scenario → Problem → Insight → Idea → Design → Evaluation
```

- Exploratory: divergent, iterative, "trial"-driven
- Usually de-emphasizes insight

### Writing Pipeline (Linear Storytelling)

```
Problem → Motivation(+Insight+idea-hint) → Design(+idea-expanded) → Evaluation
```

- Narrative: convergent, linear, "insight"-driven
- Tells a clean story, looks like natural derivation
- Extremely强化 insight

> Writing requires logic reconstruction! Reduce entropy from "chaotic exploration" to "ordered narrative."

### The Chain of Impact

```
Problem makes the paper meaningful
Insight makes the paper attractive
Idea makes the paper natural
Design makes the paper practical
Evaluation makes the paper undeniable
(Writing determines the outcome: same content, expression determines success)
```

> Research discovers truth; writing makes truth appear inevitable.

## Reviewer Psychology

### Four Axioms

1. **Default Distrust**: Reviewers assume most papers are poor quality
2. **Limited Patience**: Key information must appear early; conclusions go first
3. **Emotional Judgment**: Visual presentation directly affects acceptance decisions
4. **Logical Closure**: Arguments must be self-consistent; gaps invite rejection

> Reviewers seek flaws to REJECT. Give them reasons to ADVOCATE.

### Key Insight

- Senior reviewers: won't over-focus on evaluation (insight/idea matter most)
- **Young researchers will!** ("Why can't I reproduce this effect?!")

## Writing Workflow

### Three-Phase Process

| Phase | Goal | Actions |
|-------|------|---------|
| **Fast Output** | Capture all ideas | Don't polish; write in Chinese then translate |
| **Restructure** | Rebuild logic | ~80% rewrite; refine figures; produce draft |
| **Refine** | Polish details | Adjust wording; add citations; fill pages; proofread |

> Drafts are meant to be推翻; revision is the real creation. But the draft is the critical transition from "exploration" logic to "narrative" logic.

### Role Transition

```
Early: Engineer (deep in details) → Late: Researcher (above details)
```

> Engineer builds the system; Researcher builds the argument.
> Hide the Engineer's pride, but keep the Engineer's rigor.

### Mindset

- Don't overestimate your writing ability
- Don't pursue perfection (no paper is perfect)
- Self-satisfaction is baseline; peer-satisfaction is the goal
- Strive to: **make misunderstanding impossible; make rejection difficult**
- Writing is not a talent — it is a trained discipline

## Paper Structure

### Critical Sections (The Target)

These sections define the problem and build consensus:

**Abstract**: Mini Introduction; spend up to half on problem/motivation; show concrete numbers (`improved by 80%` not `greatly improved`)

**Introduction**: Not "introduction" but "strategic map" — make reviewers decide to read seriously
> If intro fails, the paper fails.

Structure template:
```
Problem: X is important because ...
Gap: Existing works fail because ...
Insight: We observe that ...
Approach: We propose ...
Contributions: Idea/Design/Results
```

> Reviewer starts considering acceptance here.

**Background + Motivation**: Purposeful, selective (not wiki/textbook)

Motivation three-layer structure:
```
Observation(measurable) → Limitation(inevitable) → Opportunity(actionable)
```

> "Premature solutions kill insights." State "why" first, then "how."
> The solution should feel inevitable after reading Motivation.

Structure template:
```
We observe that existing ...
This is problematic because ...
Existing approaches fail to address ...
This opens an opportunity to ...
```

### Supporting Sections

**Design**: Explain trade-offs, not describe flow; modular (module-by-module); abstract method over implementation. Maintain separation between Problem Statement (Moti) and Solution Space (Design).

**Implementation**: Credibility boost, not workload display; keep brief; focus on core parts and key tricks.

**Evaluation**: Not "running experiments" but verifying propositions:
- Claim 1: faster → latency/throughput
- Claim 2: more efficient → cost/utilization  
- Claim 3: more general → workload diversity
- Claim 4: design effective → ablation

Analysis formula:
```
Result → Cause → Attribution → Implication
```

Template:
```
We observe that ...
This is because ...
This validates that ...
This implies ...
```

> Reviewer decides acceptance here.

**Related Work**: Categorize and contrast; highlight necessity of your design. Three comparison types:
- Fundamentally Different: brief mention
- Orthogonal/Complementary: can combine
- Optimized: quantitative comparison

**Conclusion**: Fill to full page; can include future work.

## Expression Standards

### Paragraph Flow

> Paragraphs like prayer beads—round, smooth bodies connected by a thread.

Each paragraph: connect up → body → connect down. Uniform length; no isolated short paragraphs.

### Cognitive Load Minimization

> Writing goal: use simplest logic to help Reviewer understand complex work.
> If you can't explain it simply, you don't understand it well enough.

- Every reading obstacle (vague pronouns, long clauses, messy figures) consumes Reviewer goodwill
- If idea/design can't be stated simply, likely not well understood or not well formed
- Complexity in system should NOT translate to complexity in writing
- Say NO to your "code-writing self": delete anything not contributing to core argument
- A good paper is NOT a collection of facts; it is a chain of logically linked arguments

### 10-Second Rule

> If reviewer can't roughly understand a figure in 10 seconds, it's likely a negative asset.

Figures must be self-explanatory; reviewer only viewing figures + captions should understand 80%.

### Word Choice

| Avoid | Reason |
|-------|--------|
| `most`, `best` | Extreme unless theoretically proven |
| `clever`, `genius` | Subjective exaggeration |
| `precise`, `optimal` | Overclaim risk |
| Inconsistent naming | One term = one concept throughout |

**Positive framing**: `fails to` → `is limited by` → `is designed for`

## Four-Dimensional Evaluation Framework

### ① Problem Criticality — "Is the problem key?"

| Check | Question |
|-------|----------|
| Existence | Is the problem real? |
| Impact | Is it a critical bottleneck? |
| Gap | Is it unsolved? |

→ Reviewer concludes: "This is a real and critical problem."

### ② Insight Validity — "Is the insight valid?"

| Check | Question |
|-------|----------|
| Essence | Does it reveal deep causes behind surface phenomena? |
| Applicability | Is the viewpoint general, not specific? |
| Novelty | Does it challenge common sense or provide new perspective? |

→ Reviewer concludes: "This is a compelling and non-trivial insight."

### ③ Design Inevitability — "Is the design inevitable?"

| Check | Question |
|-------|----------|
| Continuity | Is it a natural derivation from insight? |
| Trade-off | Is there clear trade-off reasoning? |

→ Reviewer concludes: "This is a logical and well-justified design."

### ④ Evidence Sufficiency — "Is evidence sufficient?"

| Check | Question |
|-------|----------|
| Completeness | Is it comprehensive? (SOTA/ablation/sensitivity) |
| Explanation | Is analysis in-depth? (why, not just what) |

→ Reviewer concludes: "The claims are convincingly supported."

### Core Principles

```
Argument-driven  论证驱动
Reviewer-centric 面向评审
Logic-closed     逻辑闭环
Insight-led      洞察主导
```

## Common Rejection Reasons

> Papers are rejected not because they are bad, but because they create doubts.

| Reason | Question | Fix |
|--------|----------|-----|
| Unclear problem | "Why should I care?" | Clarify where/what/why |
| Weak motivation | "Is this problem real?" | Data-driven support |
| No clear insight | "Just engineering" | Abstract core idea |
| Unjustified design | "Why this design?" | Trade-offs under constraints |
| Weak evaluation | "I don't believe results" | SOTA + ablation + explanation |
| Poor presentation | "Hard to read" | Cognitive load minimization |
| Overclaim | "Exaggerating" | Be modest and rigorous |

## Submission Checklist

> If any box is unchecked, a reviewer likely will too.

- [ ] Problem is real, important, and clearly defined?
- [ ] Motivation has data and solid?
- [ ] Key insight is explicitly stated and non-trivial?
- [ ] Design choices are well-justified?
- [ ] Evaluation is complete?
- [ ] Results are explained, not just presented?
- [ ] Figures are self-explanatory with clear captions?
- [ ] Claims are adequately supported by evidence?
- [ ] Writing is clear, concise and easy to follow?
- [ ] Paper forms a logical loop?
- [ ] Each section delivers a clear takeaway?
- [ ] Terminology and concepts are consistent?
- [ ] Put yourself in reviewer's shoes?

## Resources

- Technical paper writing: https://homes.cs.washington.edu/~mernst/advice/write-technical-paper.html
- Technical presentations: https://homes.cs.washington.edu/~mernst/advice/giving-talk.html
- Conference acceptance rates: https://csconferences.org/

---

> 法无定法，师其意而不泥其形｜No fixed rules—grasp the principle, not the form.
> Writing is not a talent — it is a trained discipline.