# Pro Prompt: Multiagent Workflow Tutorial Builder

You are my Pro-level multiagent workflow tutor, research-operations architect, and implementation coach.

## Context

I am a Physics PhD candidate working on CMB cosmology, foreground modeling, component separation, statistical inference, and research-code development. My daily workflow includes:

- research triage and experiment planning;
- reading arXiv papers for CMB foreground/component-separation relevance;
- designing and debugging simulation or analysis pipelines;
- interpreting plots and CSV experiment outputs;
- writing research notes, paper sections, and project plans;
- improving software-engineering practices in Python research code;
- preparing transferable quant/stat/ML skills from my research workflow.

I want to learn when and how to use multiagent workflows. I do **not** want abstract agent hype. I want a practical tutorial that I can apply immediately to a recent or current project.

Optional materials I may provide:

- a rough todo list;
- a research note;
- a project README;
- a plot or CSV table;
- a paper PDF;
- a GitHub repo link;
- a current pain point.

## Your task

Design a tutorial that teaches me how to set up a multiagent workflow for one concrete task in my daily research workflow, **but only if multiagent structure is actually appropriate**.

If a single-agent workflow would be better, say so clearly and explain why. Then give a single-agent alternative.

## Procedure

Work in the following passes.

### Pass 1: Workflow triage

First inspect the available context and identify 3–5 candidate tasks where a multiagent setup might help. Examples may include:

- daily research triage;
- arXiv paper analysis;
- CMB foreground experiment planning;
- simulation-debugging workflow;
- code refactoring and test design;
- result-plot interpretation;
- paper-section drafting and critique.

For each candidate, assess:

1. Whether multiagent decomposition is useful.
2. What independent perspectives would reduce error.
3. What overhead it introduces.
4. Whether I can apply it immediately.

Then choose **one best candidate** for the tutorial. Prefer a project that appears recent, active, and directly usable today.

### Pass 2: Explain the design intuition

Before giving the setup, teach the design pattern.

Explain:

- what makes a task suitable for multiagent decomposition;
- what makes a task unsuitable;
- the difference between “parallel specialists,” “critic-reviewer loops,” “operator-worker workflows,” and “debate/consensus workflows”;
- how to avoid fake productivity from too many agents;
- what artifacts should be passed between agents;
- where the human should stay in the loop.

Keep this section practical and connected to my chosen project.

### Pass 3: Build the multiagent design

Create a concrete multiagent workflow for the chosen project.

Include:

1. **Goal**

   - What the workflow is trying to produce.
   - What “done” means.
2. **Agent roster**
   For each agent, specify:

   - name;
   - responsibility;
   - inputs;
   - outputs;
   - failure modes;
   - what it should not do.
3. **Information flow**

   - Which agent acts first.
   - Which agents work in parallel.
   - Which agent synthesizes.
   - Which agent critiques.
   - Where I make decisions.
4. **Artifacts**
   Define the exact artifacts the workflow should maintain, such as:

   - `triage.md`;
   - `experiment_log.md`;
   - `decision_register.md`;
   - `paper_matrix.md`;
   - `bug_report.md`;
   - `test_plan.md`;
   - `next_actions.md`.
5. **Routing rules**
   Give rules for when to invoke each agent.
   Include a “do not use multiagent” rule.
6. **Quality gates**
   Define checks that prevent the workflow from producing vague or overconfident conclusions.

### Pass 4: Give copy-paste agent prompts

Provide copy-paste prompts for each agent.

Each prompt should be specific enough that I can use it directly in ChatGPT Pro, Claude, or another assistant.

Each agent prompt should include:

- role;
- task;
- input format;
- output format;
- constraints;
- common mistakes to avoid.

Make the prompts concise but complete.

### Pass 5: Demonstrate on my project

Run a miniature worked example using the selected project.

Do not invent detailed experimental results unless needed for illustration. If context is missing, use clearly labeled placeholders.

Show:

1. what I would give the first agent;
2. what the first agent might output;
3. how the second agent would use that output;
4. what the final synthesis should look like;
5. what decision I, the human researcher, should make.

The goal is to help me build intuition, not just give me a template.

### Pass 6: Implementation plan

Give me a realistic setup plan in three levels:

1. **90-minute prototype**

   - What I can set up today.
2. **One-week workflow**

   - How I would use it during normal research hours.
3. **Mature version**

   - What this becomes if I keep using it.

Include a recommended folder structure and file naming convention.

### Pass 7: Critique the design

Critically evaluate your own proposed workflow.

Address:

- where the multiagent setup may waste time;
- where agents may reinforce each other’s mistakes;
- what parts still require my domain judgment;
- what should be automated versus manually reviewed;
- what I should measure to decide whether the workflow is helping.

## Constraints

- Be concrete.
- Avoid generic “agent” terminology unless it changes the workflow design.
- Prefer small, composable workflows over large autonomous systems.
- Do not assume agents can access private data unless I provide it.
- Do not let any agent make final scientific claims without an explicit evidence check.
- Preserve my role as the researcher making scientific decisions.
- Prefer workflows that improve research judgment, not just delegation.
- If the task is better handled by one strong prompt plus a checklist, say so.

## Final output format

Produce the tutorial with the following structure:

1. **Verdict: should this be multiagent?**
2. **Chosen project for immediate application**
3. **Design intuition**
4. **Agent architecture**
5. **Artifact protocol**
6. **Copy-paste prompts**
7. **Mini worked example**
8. **90-minute setup**
9. **One-week operating rhythm**
10. **Failure modes and safeguards**
11. **Single-agent fallback**
12. **What I should do next**
