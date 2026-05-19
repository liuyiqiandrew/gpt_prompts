You are my Pro-level paper-reading research operator.

I am using GPT Pro because I want more than a summary. I want a multi-pass technical reading that helps me decide what this paper means, whether I should trust it, how it connects to my work, and what I should do next.

My background:
I am a Physics PhD student working on CMB cosmology, foreground modeling, component separation, Bayesian/statistical inference, covariance modeling, and scientific computing.

Paper:
[Upload PDF or paste arXiv link]

My reading objective:
[Choose one or more:
- fast triage,
- deep technical understanding,
- implementation/reproduction,
- critique,
- literature positioning,
- advisor-facing summary,
- relevance to my own research.]

My specific research context:
I care about ideas relavent to component separation in general. In particular, modelling and mitigation approaches that leads to better foreground simulations, or more robust foreground and covariance modeling. The ultimate goal is achieving low-bias low-uncertainty constraint for the tensor-to-scalar ratio r.

Please run the analysis in the following passes.

# Pass 1: Triage and orientation

Give me:
1. The paper’s main contribution in one precise paragraph.
2. The problem it solves.
3. Why the problem is technically hard.
4. The claimed novelty.
5. Whether this paper deserves:
   - ignore,
   - skim,
   - read carefully,
   - reproduce,
   - cite,
   - discuss with advisor.

Be explicit about your confidence level.

# Pass 2: Paper-internal reconstruction

Reconstruct the paper from the inside.

Explain:
1. The physical/statistical/computational problem setup.
2. The data, simulations, or benchmarks used.
3. The model or method.
4. The key equations.
5. The inference, optimization, or training procedure.
6. The assumptions behind each major modeling choice.

For every important equation:
- Define every symbol.
- Explain what the equation is doing.
- State what assumption it encodes.
- State what would break if that assumption is false.

# Pass 3: Evidence audit

Do not just report the results. Audit the evidence.

Create a table with columns:
- Claim made by the authors.
- Evidence provided.
- Figure/table/section supporting it.
- How strong the evidence is.
- What alternative explanation could exist.
- What additional test would make the claim stronger.

Separate:
1. Claims clearly demonstrated by the paper.
2. Claims that are plausible but under-tested.
3. Claims that are speculative or overstated.

# Pass 4: Assumption and failure-mode ledger

Create an assumption ledger.

For each major assumption, give:
- The assumption.
- Why the authors need it.
- Whether it is physical, statistical, computational, or empirical.
- How serious the assumption is.
- How I would test sensitivity to it.
- Whether this assumption would be dangerous in my CMB foreground/component-separation context.

# Pass 5: Literature positioning

Place the paper in the literature.

Use external sources if available. Distinguish clearly between:
- What this paper contributes.
- What earlier papers already did.
- What this paper improves.
- What this paper does not address.

Give me:
1. Three closely related papers I should know.
2. One older foundational paper or method.
3. One recent follow-up or competing approach, if available.
4. How this paper fits into the field in one paragraph.

# Pass 6: Relevance to my work

Analyze relevance to my CMB foreground research.

Create three categories:

## Directly relevant
Ideas I could plausibly use in CMB foreground modeling, component separation, frequency decorrelation, SED fitting, covariance modeling, or parameter inference.

## Indirectly relevant
Transferable statistical, computational, or software ideas.

## Not relevant
Parts that are probably not worth my time.

For each relevant idea, say:
- Why it matters.
- How it maps onto my work.
- What would need to be modified.
- What minimal test I could run.

# Pass 7: Implementation/reproduction plan

Suppose I want to reproduce or adapt the core method.

Give me:
1. Minimal toy problem.
2. Required inputs.
3. Required outputs.
4. Core algorithm in pseudocode.
5. Main implementation risks.
6. What I should implement first.
7. What can be ignored in the first prototype.
8. A one-day, three-day, and one-week implementation plan.

# Pass 8: Advisor-facing output

Prepare a concise advisor-facing summary:

1. Three-sentence summary.
2. Why this paper matters.
3. What I learned.
4. One technical concern.
5. One possible connection to my project.
6. One concrete next step.

Keep this section short and meeting-ready.

# Pass 9: Research notebook entry

Produce a reusable literature-catalog entry:

- Citation:
- Tags:
- Verdict:
- One-sentence contribution:
- Problem:
- Method:
- Key equations:
- Main result:
- Assumptions:
- Weaknesses:
- Relevance to my work:
- Follow-up ideas:
- Read again? yes/no:
- Priority: low/medium/high

# Style requirements

Be precise and technical.
Do not write generic praise.
Do not hide uncertainty.
Clearly distinguish:
- paper claims,
- demonstrated results,
- your interpretation,
- external context,
- possible extensions.

When possible, cite paper sections, equations, figures, or external sources.