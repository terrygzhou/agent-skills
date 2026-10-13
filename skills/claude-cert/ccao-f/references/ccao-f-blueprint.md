# CCAO-F Blueprint (exam guide v1.0, effective July 2026)

- **Exam code**: CCAO-F (Claude Certified Associate - Foundations)
- **Audience**: professionals who use Claude as a day-to-day productivity tool - operations,
  marketing, project management, education, communications, general knowledge work. No
  API or software-development experience needed; credential awarded on exam performance alone.
- **Format**: 60 items, standalone multiple-choice + multiple-response (each item states how
  many answers to pick). 120 min. Pass 720/1000. Fee $99 USD. Valid 12 months.
- **Does not count** toward Claude Partner Network tier eligibility (unlike the other three).
- **Prerequisites**: none. Recommended: regular hands-on Claude use in a professional setting.

## Seven domains (official weights)

| # | Domain | Weight |
|---|---|---|
| 1 | Prompting and Task Execution | 14% |
| 2 | Output Evaluation and Validation | 21% |
| 3 | Product and Model Selection | 12% |
| 4 | Workflow Integration and Solution Design | 16% |
| 5 | Configuration and Knowledge Management | 12% |
| 6 | Governance, Risk, and Responsible Use | 15% |
| 7 | Troubleshooting and Optimisation | 10% |

**Domains 2 + 4 + 6 = 52%** - judging output, integrating into workflows, and responsible
use are the spine. Prompting + Model Selection + Configuration = 38%. Troubleshooting = 10%.

## Sub-topics per domain

**D1 Prompting and Task Execution (14%)**
1.1 create effective prompts for business and technical tasks - 1.2 task decomposition for
complex requests - 1.3 iterative prompt refinement - 1.4 adapt prompting strategy by task
type (analysis, research, drafting, brainstorming)

**D2 Output Evaluation and Validation (21%)**
2.1 evaluate outputs for accuracy and completeness - 2.2 identify hallucinations,
inconsistencies, biases - 2.3 fact-checking and validation techniques - 2.4 decide when
human review / additional verification is required - 2.5 edit, adapt, refine, compare
outputs for the intended audience - 2.6 organise and curate information; choose output
formats (artifacts, inline, structured data)

**D3 Product and Model Selection (12%)**
3.1 select Claude product features (Projects, research mode, chat, artifacts) - 3.2
differentiate model tiers (Haiku, Sonnet, Opus) - 3.3 align model to task requirements
(cost, speed, quality) - 3.4 manage context limits and memory (when to restart,
summarise, or persist)

**D4 Workflow Integration and Solution Design (16%)**
4.1 analyse requirements and use cases with Claude - 4.2 Claude for research, planning,
process optimisation - 4.3 Claude in solution design, development, iteration - 4.4
integrate Claude into existing workflows (augment or redesign) - 4.5 communicate Claude's
value and limitations to stakeholders

**D5 Configuration and Knowledge Management (12%)**
5.1 configure Claude Projects with instructions and knowledge sources - 5.2 manage
uploaded knowledge and connectors (e.g. Google Drive, Gmail) - 5.3 write effective
system-level instructions - 5.4 inform, maintain, update configurations, knowledge
sources, and instructions over time

**D6 Governance, Risk, and Responsible Use (15%)**
6.1 identify appropriate vs inappropriate use cases - 6.2 data sensitivity, regulatory and
privacy considerations - 6.3 follow organisational AI policy and governance standards -
6.4 understand ethical implications of AI use

**D7 Troubleshooting and Optimisation (10%)**
7.1 identify, diagnose, resolve underperforming prompts / poor outputs - 7.2 adjust
approach based on feedback and results - 7.3 optimise workflows for efficiency and
effectiveness

## The decision, not the fact (per domain)

- **Prompting**: a repeatable component framework (task, context, constraints, output
  format, audience). Decompose first, prompt per step. Iterate diagnostically: find which
  component is failing, fix that one.
- **Evaluation**: the default stance is suspicion. Every output is checked for accuracy,
  completeness, provenance, and bias before it ships. Record what was verified and how;
  name what still needs a human.
- **Model/product**: match tier to constraint. Haiku = cheap + fast for volume; Sonnet =
  default balanced; Opus = when quality is the binding constraint. Restart vs summarise
  vs persist: persist durable knowledge in a Project; summarise when context gets long;
  restart when the conversation has drifted.
- **Workflow**: delegate the repetitive middle, keep the judgement and the accountability
  steps human. State which steps Claude owns per workflow.
- **Configuration**: the Project is the unit of reuse. Instructions + knowledge that stay
  current; stale instructions are a silent quality failure.
- **Governance**: check data sensitivity, privacy, and policy fit BEFORE first use, not
  after. Escalate what is outside your remit.
- **Troubleshooting**: root-cause taxonomy = prompt defect / missing context / wrong
  model or feature / task-model mismatch. Fix the cause; verify the fix persists.

## Study plan shape (4 weeks, ~30-40 min/day)

- **Week 1**: D2 + D6 (36%): evaluation discipline, validation techniques, governance
  checks. Drill: take 10 real outputs you produced, grade each on accuracy/completeness/
  provenance/bias, write the rejection criteria.
- **Week 2**: D1 + D4 + D3 (42%): prompting framework, workflow delegation maps, model
  tier selection. Build one real workflow with a delegation table (step -> owner:
  Claude/human).
- **Week 3**: D5 + D7 (22%): stand up a Claude Project with instructions + knowledge;
  break prompts on purpose, diagnose, fix, verify.
- **Week 4**: full 60-item timed mocks at real pace (target 900+), review every
  wrong-answer rationale; exam day.

## Recurring themes

- Judgement over recall: the Associate is the programme's "know when it is good enough"
  credential; questions reward defensible evaluation calls, not trivia.
- Provenance: a usable output is one you can point at the source for; fluency without
  sources is a red flag.
- Human-in-the-loop: irreversible / high-stakes / external outputs get human verification;
  the skill is knowing the line.
- Context as budget: the four pre-prompt decisions (entry point, feature, model, context)
  set the quality ceiling; most "bad prompt" failures are actually context failures.
- Stale config: a Project that stopped being updated silently degrades; maintenance is
  part of the skill.

## Free prep (official, free registration on the Skilljar portal)

- CCAO-F prep course: Claude Platform & Model Foundations; Prompting & Task Execution;
  Evaluating & Validating Claude's Output; Workflow Integration & Solution Design;
  Configuration & Knowledge Management; Governance, Risk & Responsible Use;
  Troubleshooting & Optimization; Course Summary & Next Steps.
- Prerequisite courses recommended: Claude 101, AI Fluency: Framework & Foundations, AI
  Capabilities and Limitations.
- Full third-party prep track at claudecertificationguide.com was "coming soon" as of
  2026-10-13; the free CCAR-F track covers the technical spine but is developer-aimed.
