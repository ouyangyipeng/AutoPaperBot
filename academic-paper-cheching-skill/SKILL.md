---
name: academic-paper-checking
description: |
  Checks a completed academic paper against top-tier conference standards and the "From Engineering Implementation to Scientific Argument" methodology. Produces a detailed scoring report with specific scores per dimension, identified issues, and actionable improvement suggestions.
  
  Use this skill when:
  - Reviewing or checking a completed academic paper for quality
  - Evaluating a paper draft before submission
  - Performing self-check or peer-review on a paper
  - Identifying weaknesses and gaps in a paper
  - Scoring a paper against four-dimensional evaluation framework
  - Generating improvement suggestions for a paper
  - Any task involving paper quality assessment or review
  
  Do NOT use for:
  - Writing a new paper (use academic-paper-writing skill instead)
  - Non-academic document review
  - Simple grammar or formatting checks without domain expertise
---

# Academic Paper Checking

Systematically evaluate a completed paper against top-tier conference standards. Produce a structured scoring report with per-dimension scores, issue identification, and actionable suggestions.

## Evaluation Methodology

### Four-Dimensional Framework

Evaluate the paper across four dimensions, each scored 0-10:

**① Problem Criticality (问题关键性)** — "Is the problem key?"
- Existence: Is the problem real and observable?
- Impact: Is it a critical bottleneck with significant consequences?
- Gap: Is it genuinely unsolved by existing work?

**② Insight Validity (洞察有效性)** — "Is the insight valid?"
- Essence: Does it reveal deep causes behind surface phenomena?
- Applicability: Is the viewpoint general, not specific to one case?
- Novelty: Does it challenge common sense or provide new perspective?

**③ Design Inevitability (设计必然性)** — "Is the design inevitable?"
- Continuity: Is it a natural derivation from the stated insight?
- Trade-off: Is there clear reasoning for why this design over alternatives?

**④ Evidence Sufficiency (验证充分性)** — "Is evidence sufficient?"
- Completeness: SOTA comparison? Ablation? Sensitivity analysis?
- Explanation: Are results explained (why), not just presented (what)?

### Presentation Quality (表达质量)

Additional dimensions covering writing and visual standards:

**⑤ Logical Closure (逻辑闭环)** — "Does the paper form a closed loop?"
- Does Observation → Insight → Design → Evidence form a complete chain?
- Are there logical gaps or dangling arguments?

**⑥ Cognitive Load (认知负荷)** — "Is the paper easy to read?"
- Are key conclusions placed early and prominently?
- Is there unnecessary complexity in expression?
- Can figures be understood in 10 seconds?

**⑦ Professional Rigor (专业严谨)** — "Is the paper academically rigorous?"
- Are claims adequately supported by evidence?
- Is terminology consistent throughout?
- Are extreme/absolute words used carefully?

## Checking Procedure

When invoked, follow this exact procedure:

### Step 1: Read the Paper Thoroughly

Read every section of the paper. Take notes on:
- What problem is claimed
- What insight is stated
- What design is proposed
- What evidence is presented
- How the narrative flows

### Step 2: Dimension-by-Dimension Evaluation

For each of the 7 dimensions, evaluate the paper and assign a score (0-10).

#### Scoring Guide

| Score | Meaning |
|-------|---------|
| 9-10 | Excellent. Meets top-tier standard with no significant issues. |
| 7-8 | Good. Mostly meets standard with minor room for improvement. |
| 5-6 | Adequate. Meets basic requirements but has noticeable weaknesses. |
| 3-4 | Weak. Significant issues that would likely concern reviewers. |
| 1-2 | Critical. Major deficiencies that would likely lead to rejection. |
| 0 | Absent. The dimension is completely missing from the paper. |

### Step 3: Detailed Issue Identification

For each dimension, list specific issues found in the paper. Use this format:

```
[Dimension Name] — Score: X/10

Issues:
1. [Specific issue with location reference]
2. [Specific issue with location reference]
...

Strengths:
1. [Specific strength observed]
...
```

### Step 4: Generate Improvement Suggestions

For each issue, provide actionable suggestions:

```
Issue: [description]
Suggestion: [specific, actionable fix]
Priority: [Critical/High/Medium/Low]
```

### Step 5: Overall Assessment

Calculate the overall score and provide a final verdict.

## Output Format

ALWAYS produce the report in this exact format:

```
# Paper Quality Assessment Report

**Paper Title:** [title from the paper]
**Evaluation Date:** [date]
**Evaluator:** AI Agent (academic-paper-checking skill)

---

## Overall Score: X/10

| Dimension | Score | Status |
|-----------|-------|--------|
| ① Problem Criticality | X/10 | [Excellent/Good/Adequate/Weak/Critical] |
| ② Insight Validity | X/10 | [Excellent/Good/Adequate/Weak/Critical] |
| ③ Design Inevitability | X/10 | [Excellent/Good/Adequate/Weak/Critical] |
| ④ Evidence Sufficiency | X/10 | [Excellent/Good/Adequate/Weak/Critical] |
| ⑤ Logical Closure | X/10 | [Excellent/Good/Adequate/Weak/Critical] |
| ⑥ Cognitive Load | X/10 | [Excellent/Good/Adequate/Weak/Critical] |
| ⑦ Professional Rigor | X/10 | [Excellent/Good/Adequate/Weak/Critical] |

**Overall Verdict:** [Ready for submission / Needs revision before submission / Major rewrite needed / Not submission-ready]

---

## Detailed Findings

### ① Problem Criticality — Score: X/10

**Existence Check:**
- [Findings on whether problem is real and observable]

**Impact Check:**
- [Findings on whether problem is a critical bottleneck]

**Gap Check:**
- [Findings on whether problem is genuinely unsolved]

**Issues:**
1. [Specific issue — Section X, Paragraph Y]
2. ...

**Strengths:**
1. [Specific strength]
2. ...

**Suggestions:**
1. [Actionable suggestion] — Priority: [level]
2. ...

---

### ② Insight Validity — Score: X/10

[Same sub-structure as above]

---

### ③ Design Inevitability — Score: X/10

[Same sub-structure as above]

---

### ④ Evidence Sufficiency — Score: X/10

[Same sub-structure as above]

---

### ⑤ Logical Closure — Score: X/10

**Loop Check:**
- Observation → Insight: [Connected? Gap?]
- Insight → Design: [Connected? Gap?]
- Design → Evidence: [Connected? Gap?]
- Evidence → Observation: [Does it close the loop?]

**Dangling Arguments:**
- [Any claims not supported? Any evidence not connected to claims?]

[Issues/Strengths/Suggestions as above]

---

### ⑥ Cognitive Load — Score: X/10

**10-Second Rule Check:**
- [Can each figure be understood in 10 seconds?]

**Conclusion Placement:**
- [Are key conclusions placed early?]

**Unnecessary Complexity:**
- [Are there overly complex expressions that could be simplified?]

[Issues/Strengths/Suggestions as above]

---

### ⑦ Professional Rigor — Score: X/10

**Claim Verification:**
- [Are all claims supported by specific evidence?]

**Terminology Consistency:**
- [Are terms used consistently throughout?]

**Absolute Language:**
- [Are extreme words used appropriately?]

[Issues/Strengths/Suggestions as above]

---

## Priority Action Items

List all suggestions sorted by priority:

### Critical (Must fix before submission)
1. [Item]
2. ...

### High (Strongly recommended)
1. [Item]
2. ...

### Medium (Recommended for improvement)
1. [Item]
2. ...

### Low (Optional polish)
1. [Item]
2. ...

---

## Submission Readiness Assessment

**Can a skeptical reviewer understand and believe this paper?**

| Checklist Item | ✅ Pass | ❌ Fail |
|---------------|---------|---------|
| Problem is real, important, clearly defined | | |
| Motivation has data and solid | | |
| Key insight explicitly stated and non-trivial | | |
| Design choices well-justified | | |
| Evaluation is complete | | |
| Results explained, not just presented | | |
| Figures self-explanatory with clear captions | | |
| Claims adequately supported by evidence | | |
| Writing clear, concise, easy to follow | | |
| Paper forms a logical loop | | |
| Each section delivers a clear takeaway | | |
| Terminology and concepts consistent | | |
| Reviewer perspective adopted | | |

**Note:** If any item is unchecked, a reviewer likely will too.

---

*Report generated by academic-paper-checking skill*
*Based on "From Engineering Implementation to Scientific Argument" methodology*
```

## Specific Checks Per Dimension

### Problem Criticality Checks

1. **Is the problem explicitly stated?** Find the sentence that defines the problem. Is it clear, specific, and verifiable?
2. **Is there data supporting problem existence?** Are there measurements, benchmarks, or studies showing the problem is real?
3. **Is the problem impact quantified?** "Performance drops by 10×" vs "performance is sometimes slow"
4. **Is the gap clearly identified?** Does the paper explain what existing work fails to address?
5. **Scenario → Problem convergence**: Does the paper narrow from a broad scenario to a specific, solvable problem?

### Insight Validity Checks

1. **Is insight explicitly stated?** Can you find a clear sentence articulating the key insight? Or is it buried/implicit?
2. **Does insight go beyond surface?** Is it "X is slow" (surface) or "X is slow because of I/O-bound nature rather than compute-bound" (deep)?
3. **Is insight generalizable?** Does it apply beyond the specific system/dataset studied?
4. **Does insight explain why existing methods fail?** Not just "they don't work" but "they fail because they ignore cross-layer dependencies"
5. **Premature solution check**: Does motivation present solutions before establishing insight?

### Design Inevitability Checks

1. **Design-insight connection**: Can you trace each design decision back to the stated insight? Is the path logical?
2. **Trade-off reasoning**: Does the paper explain WHY this design choice over alternatives? Or just describes WHAT was chosen?
3. **Motivation-design separation**: Is problem statement clearly separated from solution space? Or do they blur together?
4. **Design covers all problems**: Does every stated problem/challenge have a corresponding design component addressing it?
5. **Module-by-module clarity**: Can each design module be understood independently?

### Evidence Sufficiency Checks

1. **SOTA comparison**: Is there comparison with state-of-the-art methods? If not, this is a hard flaw.
2. **Ablation study**: Is there evidence that each design component contributes to the overall result?
3. **Sensitivity analysis**: Are results shown across varying parameters/conditions?
4. **Generality**: Are results shown across diverse workloads/datasets/scenarios?
5. **Results explained**: For each result, is there analysis of WHY (not just WHAT)?
6. **Anomaly handling**: Are surprising/negative results acknowledged and explained?
7. **Claim-evidence mapping**: Can each claim be traced to specific experimental evidence?

### Logical Closure Checks

1. **Full loop**: Observation → Insight → Design → Evidence → (back to) Observation
2. **No dangling claims**: Every claim has supporting evidence
3. **No orphan evidence**: Every experiment connects back to a design choice or problem
4. **Consistent narrative**: The story doesn't contradict itself across sections
5. **Section takeaways**: Each section has a clear conclusion that advances the argument

### Cognitive Load Checks

1. **10-second figure rule**: Can each figure be roughly understood in 10 seconds?
2. **Front-loading**: Are key conclusions and qualitative statements placed early in paragraphs/sections?
3. **No clause trains**: Are sentences reasonably short? No `... which ... which ... which ...`
4. **No isolated paragraphs**: Are all paragraphs substantial and connected?
5. **Self-explanatory figures**: Can figures + captions alone convey 80% of the message?
6. **Unnecessary detail removed**: Is implementation detail that doesn't serve the argument removed?

### Professional Rigor Checks

1. **No overclaim**: Are extreme words (best, optimal, most) used only with theoretical backing?
2. **Consistent terminology**: Same concept = same term throughout
3. **Positive framing**: Uses "is designed for" rather than "fails to"
4. **Acknowledged limitations**: Does the paper admit its own limitations?
5. **Correct citations**: Are referenced works real and correctly cited?
6. **Reproducibility**: Are experimental setups described sufficiently for reproduction?

## Important Notes

- This skill evaluates, not fixes. Point out issues and suggest fixes, but don't rewrite the paper.
- Be specific: reference section numbers, paragraph locations, figure numbers.
- Be constructive: every issue should have an actionable suggestion.
- Be honest: don't inflate scores. A skeptical reviewer would be harsh; mirror that.
- Consider domain: systems papers have different expectations than ML theory papers. Adapt criteria accordingly.
- The four-dimensional framework (Problem/Insight/Design/Evidence) is the backbone; Presentation dimensions (Logic/Cognitive/Rigor) support it.