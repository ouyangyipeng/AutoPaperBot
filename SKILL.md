---
name: academic-paper-writing
description: |
  Guides AI agents to write high-quality academic papers following top-tier conference standards. 
  
  Use this skill when:
  - Writing or drafting academic papers for AI/systems conferences
  - Designing paper structure, sections, or experimental methodology
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

Guide agents through the complete academic paper writing process, from initial draft to final submission.

## Core Philosophy

**Writing = Building Arguments, Not Recording Work**

Papers must construct an irrefutable argument system, not simply document what was done. The goal: make reviewers conclude "this problem is important, this method is sound, these results are credible."

### The Argument Loop

```
Observation → Insight → Design → Evidence
```

Every section must form a verifiable takeaway that closes this loop.

## Reviewer Psychology

### Four Axioms

1. **Default Distrust**: Reviewers assume most papers are poor quality
2. **Limited Patience**: Key information must appear early; conclusions go first
3. **Emotional Judgment**: Visual presentation directly affects acceptance decisions
4. **Logical Closure**: Arguments must be self-consistent; gaps invite rejection

> Reviewers seek reasons to REJECT. Give them reasons to FIGHT for your paper.

## Writing Workflow

### Three-Phase Process

| Phase | Goal | Actions |
|-------|------|---------|
| **Fast Output** | Capture all ideas | Don't polish; write in Chinese then translate with LLM |
| **Restructure** | Rebuild logic | ~80% rewrite; refine figures; produce abstract and draft |
| **Refine** | Polish details | Adjust wording; add citations; fill pages; proofread |

### Time Budget

| Work Type | Comfortable | Minimum |
|-----------|-------------|---------|
| New work | 1 month | 2 weeks |
| Incremental | 3 weeks | 1 week |
| Resubmission | 1 week | 1 day |

### Role Transition

```
Early phase: Engineer (deep in details)
Late phase: Researcher (above details)
```

> Kill the Engineer in you; wake up the Researcher.

## Paper Structure

### Critical Sections (The Target)

These three sections define the problem and build consensus:

- **Abstract**: Mini Introduction; spend up to half on problem/motivation; show concrete numbers
- **Introduction**: Make reviewers want to read; structure: problem → gap → insight → contributions
- **Background + Motivation**: Not a tutorial; purposeful introduction; three-layer structure: Observation → Limitation → Opportunity

### Supporting Sections

- **Design**: Explain trade-offs, not describe flow; modular presentation; abstract method, not implementation
- **Implementation**: Credibility boost, not workload display; keep brief
- **Evaluation**: Setup → Main results → Ablation → Supplementary; use concrete numbers in text
- **Related Work**: Categorize and contrast; highlight necessity of your approach
- **Conclusion**: Fill to full page; can include future work

### Key Requirements

- Front two pages: include intuitive figures explaining the problem
- Design: minimum 3 points for top-tier; must cover all stated problems
- Evaluation: must close the loop—cover all design points and initial questions

## Expression Standards

### Paragraph Flow

> Paragraphs should be like prayer beads—round, smooth bodies connected by a thread.

Each paragraph:承上 (connect up) → body → 启下 (connect down)

- Uniform length; no isolated short paragraphs
- Reader should flow through without thinking

### Sentence Rules

| Problem | Fix |
|---------|-----|
| Clause trains | `... which ... which ...` → `.... It .... This ...` |
| Head-heavy | Move long subject to `It is common to see...` |
| Colloquial | `piece of cake` → `trivial to do` |

### Word Choice

| Avoid | Reason |
|-------|--------|
| `most`, `best` | Extreme unless theoretically proven |
| `clever`, `genius` | Subjective exaggeration |
| Rare terms | Unless domain-standard |
| Inconsistent naming | One term = one concept throughout |

**Positive framing**: `fails to` → `is limited by` → `is designed for`

## Figure Standards

### Information Density

- Compact layout; avoid "padding" accusations
- Unified color scheme across all figures
- Consider black-white printing; use textures

### Dimensions

- Single column: `4inch × 100dpi = 400pt`
- Double column: 7 inches wide
- Reserve 1-2 double-column figures for page filling

### Data Visualization

- Global color palette; explicit color in all code
- Must show average/mean values
- Caption explains figure; self-contained understanding
- Matplotlib: `bbox_inches='tight', pad_inches=0`

## Experimental Rigor

### Structure

```
Setup → Main Experiment → Ablation → Supplementary
```

### Analysis Formula

```
Phenomenon → Cause → Design Connection → Implication
```

### Requirements

- **SOTA comparison required**: No strong baseline = unverifiable paper
- **Ablation required**: Prove gains come from design
- **Anomaly analysis**: Surprising/negative results need deep explanation
- **Numbers in text**: Don't make readers hunt in figures

> Analysis should be thorough enough that reviewers don't want to read it.

## Submission Process

### Pre-submission

- Verify template (font size errors are fatal)
- Remove copyright information
- Collect all ORCID IDs early

### Rebuttal Workflow

```
List questions → Answer each → Merge similar → Assign responsibility
```

### Camera-ready

- Fix reviewer-identified issues
- Add copyright, authorship, acknowledgments
- Watch for page count changes

## Common Pitfalls

### Content Errors

| Mistake | Correct Approach |
|---------|------------------|
| Writing as tutorial | Purposeful intro; highlight connection to your work |
| Writing as engineering report | Build argument system |
| Implementation dumping | Abstract method, not details |

### Experiment Errors

| Mistake | Correct Approach |
|---------|------------------|
| Data dumping | Guide understanding with text |
| Unattributed gains | Prove source is your design |
| Missing baseline | SOTA comparison mandatory |

### AI Tool Usage

- LLM translation shows detectable patterns
- Use LLM for translation + polish, but apply your own voice
- Writing experience beats observation

## Self-Check List

### Format

- [ ] Template correct?
- [ ] Looks like a paper?
- [ ] Last page full?

### Content

- [ ] Background/Related Work written as tutorial?
- [ ] Design covers all stated problems?
- [ ] Evaluation covers all Design points?

### Structure

- [ ] No isolated paragraphs?
- [ ] No short paragraphs?
- [ ] No long sentences?

### Data

- [ ] Concrete numbers in abstract/text?
- [ ] Average values on figures?

### Consistency

- [ ] Terms consistent throughout?
- [ ] Figure colors unified?

## Resources

- Technical paper writing: https://homes.cs.washington.edu/~mernst/advice/write-technical-paper.html
- Technical presentations: https://homes.cs.washington.edu/~mernst/advice/giving-talk.html
- Conference acceptance rates: https://csconferences.org/

---

> Papers are labels you attach to yourself. What kind of person writes what kind of paper, and what kind of paper defines what kind of person.