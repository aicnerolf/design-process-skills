---
name: problem-framing-and-planning
description: >
  Frame design problems and plan how to approach them before any design work begins.
  Covers: defining the business and user problem, setting success metrics, identifying
  constraints, mapping stakeholders, scoping what's in and out, and phasing the approach.
  Trigger on: new projects, project kickoffs, "help me frame this," "what should we solve,"
  "how should we approach this," "what's the plan," defining goals, setting metrics,
  scoping a feature, phasing work, writing a brief, or any moment where design direction
  needs to be established before jumping into solutions. Also trigger when someone says
  "I'm starting a new project," "we need to figure out what to build," or "what should
  we prioritize." Use this skill broadly; any time a design problem needs framing or a
  project needs a plan, this skill applies.
---

# Problem framing and planning

## What this skill does

This skill establishes clarity before design work begins. It ensures that every project starts with a well-articulated understanding of the problem, its significance, the criteria for success, and a deliberate plan for how to approach it.

Framing and planning are not sequential activities. Defining the problem shapes the approach, and early planning frequently reveals that the problem itself needs reframing. They evolve together.

## Core principle

Every design project must begin by answering one question with precision: what does the user need in order to achieve their goal? Not what features they request. Not what the business wishes they would do. What goal are they pursuing, and what stands between them and that goal? If this cannot be clearly articulated, pause and resolve it before proceeding. Ambiguity here is the most common reason design work drifts.

## Conceptual toolkit

These are the analytical lenses that should inform how problems are framed. They are practical instruments, not abstract theory. For expanded context on each, consult `references/design-principles.md`.

**Jobs to be done.** Frame problems around the job the user is trying to accomplish, not around features or tasks. A to-do application is not about "managing tasks"; the job might be "maintaining confidence that nothing important will be overlooked." Always interrogate: what job is the user hiring this product to do? What are they currently relying on, and where does it fall short?

**Mental models.** Users arrive with expectations shaped by every other product they have used. These expectations constitute their mental model of how systems work. Framing a problem without accounting for the user's existing mental model produces solutions that are internally coherent but externally confusing. Ask: what does the user already expect, and where will those expectations collide with what we are building?

**The interfaces ecosystem.** No product exists in isolation. Users construct their mental models from the entire constellation of tools they interact with. These adjacent products establish conventions around interaction patterns, terminology, information architecture, and visual language. Understanding the ecosystem is not supplementary research; it is foundational context.

**Interface paradigm and metaphor.** Every product rests on a foundational metaphor: canvas, document, feed, conversation, dashboard. This metaphor carries structural implications that govern what users expect the product to do and how they anticipate interacting with it. During framing, identify which metaphor the current experience relies on and interrogate whether it still serves users. A paradigm that functioned at one scale or context may fracture at another.

**Norman's three levels.** Products operate simultaneously on three levels: visceral (immediate sensory response), behavioral (the quality of interaction; ease, effectiveness, satisfaction), and reflective (meaning, identity, self-perception). When framing, discern which level is most consequential for the project. A medical device and a journaling app carry fundamentally different emotional mandates, even when they share interaction patterns. Misidentifying the level leads to solving the wrong problem.

**Interfaces have meaning.** Every interface communicates, whether deliberately or not. A significant number of problems framed as "users cannot do X" are more accurately described as "the interface fails to communicate that X is possible." Position, label, color, scale, whitespace; these are all signs that users interpret. When framing, distinguish between functionality problems and communication problems. The distinction reshapes the solution.

**Garrett's layers as diagnostic.** When a problem resists clear definition, identify which layer of the experience it inhabits: strategy (misaligned goals), scope (incorrect feature set), structure (flawed organization or interaction model), skeleton (ineffective layout or navigation), or surface (inadequate visual treatment). Addressing a structural problem with a surface intervention is wasted effort.

## When starting a new project

### Step 1: Gather evidence first

Before forming any position, assemble everything that already exists about this problem or idea. Draw from all available sources:

- Prior design work, prototypes, or explorations
- User research, support inquiries, feedback
- Analytics and behavioral data
- Business context (strategy documents, OKRs, roadmaps)
- Stakeholder perspectives and historical decisions

This step is non-negotiable. Building on existing knowledge prevents redundant work and surfaces constraints before they become obstacles.

### Step 2: Answer the framing questions

Work through each of these deliberately. Every one carries weight; omitting any of them invites regret later.

- **What job is the user trying to accomplish?** Not the feature, not the task; the underlying goal and motivation. What outcome are they pursuing? What are they relying on today, and where does it fall short?
- **What is the business context?** Where does this initiative sit within the company's strategy, objectives, or roadmap? What is the market landscape? Why is this timely?
- **What problem does this solve?** Articulate it in terms of the user's experience, not the feature. "Users cannot locate their team's work" rather than "we need better search." Probe further: is this a functional problem (inability to act), a communicative problem (failure to understand), or an emotional problem (something feels wrong)?
- **What is the opportunity?** What changes if we resolve this? Quantify wherever possible.
- **Why does this warrant the investment?** Connect to business objectives. If this case cannot be made compellingly, the project is vulnerable to deprioritization.
- **How are others addressing this?** Benchmark against competitors, adjacent products, and analogous solutions across industries. What is the ecosystem of tools users already inhabit, and what expectations has that ecosystem established?
- **Where will we differentiate?** Where do existing solutions fall short of the user's actual job? How will we address that gap in a way that is meaningfully superior, not merely novel?
- **Who will use this?** Specify precisely. Which users, in what context, with what degree of expertise? What mental models do they carry from their experience with other tools?
- **How might this fail?** Identify risks: technical constraints, adoption barriers, organizational dependencies, incorrect assumptions about user behavior. Consider also: could this resolve the functional problem while failing emotionally? Could it serve existing users while alienating new ones?
- **What resources are available?** Team composition, timeline, technical capacity, existing systems to leverage or navigate.
- **Who are the stakeholders?** Who holds decision-making authority, who must be consulted, who should be informed.

### Step 3: Define success metrics

Establish measurable objectives before any design work begins. They serve two purposes: focusing design effort on what genuinely matters, and providing the basis for evaluating whether the work succeeded.

Effective metrics are:

- Anchored to the user's ability to achieve their goal (not exclusively to business KPIs)
- Measurable with existing or attainable instrumentation
- Time-bound (when will evaluation occur?)
- Specific enough to drive decisions ("increase activation rate from 32% to 45%" rather than "improve onboarding")

### Step 4: Plan the approach

**Phasing.** Determine what to address first:

- Begin with whatever reduces the most consequential uncertainty.
- Target what moves the most significant metric.
- Constrain the initial phase to a scope small enough to learn from. Ship, measure, expand.
- Defer what can wait without impeding learning.

**Scoping.** Define inclusions and exclusions explicitly. Document the reasoning behind deferrals, not merely the fact of them. "Deferred to phase 2 because it depends on API work beginning in Q3" is useful. "Phase 2" alone is not.

**Approach.** Define how the team will navigate this work. What requires research first? Where can momentum be built quickly? What demands cross-functional alignment before proceeding? Tailor the process to the project; not every initiative requires identical steps.

**Dependencies.** Name what this project relies on: other teams, infrastructure, data availability, stakeholder decisions. Surface these early; concealed dependencies are where timelines collapse.

## Strategic context and scalability

Rigorous framing does not stop at the project boundary. Every problem exists within a larger system, and the strongest framing accounts for that context.

- **Surface problems proactively.** Rather than waiting for assignments, examine the product and organization for problems that are quietly eroding user experience or business outcomes, and frame them before they escalate.
- **Connect to the product vision.** Every project should align with where the product is heading over the coming quarters. If the connection is absent, either the project needs reconsideration or the vision does.
- **Evaluate leverage.** Among everything the team could pursue, is this the highest-leverage problem? Frame not only the problem itself but its relative priority against alternatives.
- **Think across boundaries.** How does this problem affect adjacent teams? Could the solution extend beyond a single team's domain? Are there underlying patterns that, if resolved here, would strengthen the product systematically?
- **Design for scalability and extensibility.** Frame problems in a way that yields solutions with lasting value. A fix for one team's workflow is useful; a framework that generalizes across teams is substantially more valuable. Ask: will this framing produce something reusable, or something disposable?

## Output format

When producing a problem frame and plan, employ this structure:

```
## Problem statement
[What problem are we solving? Articulated in terms of the user's ability to achieve their goal.]

## Job to be done
[What job is the user trying to accomplish? What outcome are they pursuing? What are they relying on today and where does it fall short?]

## Business context
[Where does this sit within the company's strategy? Market dynamics? Why now?]

## Opportunity
[Why does this matter? What changes if we resolve it? Connection to business objectives.]

## Benchmark and landscape
[How are others addressing this? What patterns exist? What expectations has the ecosystem established?]

## Differentiation
[Where is the opportunity to be meaningfully superior? What will make our approach compelling?]

## Success metrics
[How will we measure success? Specific targets tied to the user's ability to achieve their goal.]

## Users
[Who is affected? Context, expertise, mental models, behavioral patterns.]

## Risks and constraints
[How might this fail? Technical, organizational, adoption, communicative, and emotional risks.]

## Stakeholders
[Who holds authority, who must be consulted, who should be informed.]

## Approach and phases
[How will we proceed? What constitutes phase 1? What is deferred and why?]

## Open questions
[What remains unresolved? What assumptions are we carrying?]
```

Weight sections according to where the most significant unknowns reside.

## Tone and style

- Professional and precise. No filler, no equivocation.
- Lead with the problem, not the solution.
- Make assumptions explicit. If something is conjecture, name it.
- Quantify wherever possible. "Many users struggle" is vague. "42% abandon at step 3" is actionable.
- Write for a cross-functional audience. Product managers, engineers, and leadership should all be able to engage with this and understand the direction.

## What this skill does NOT do

- Design solutions. This skill frames the problem and charts the approach. Design follows.
- Conduct research. This skill identifies what is known and what remains unknown. Primary research is a distinct activity.
- Produce implementation specs. This yields a brief and a plan, not engineering documentation.
- Substitute for judgment. This skill surfaces the information needed to make sound decisions. The decisions themselves require your expertise and your team's input.

## Usage examples

**Starting a new project:**
- "I'm starting a new project. We need to redesign our onboarding flow."
- "Help me frame the problem for a new commenting feature."
- "We've been asked to improve activation. Where do I start?"

**Writing a brief:**
- "Help me write a brief for this initiative."
- "I need to define goals and success metrics for this project."
- "Help me articulate why this project warrants the investment."

**Planning an approach:**
- "How should we approach this redesign?"
- "Help me phase this project. What should ship first?"
- "What's the plan? We have 6 weeks and two designers."

**Scoping:**
- "Help me define what's in and out for v1."
- "We're trying to do too much. Help me prioritize."

**Systemic framing:**
- "Looking across our product, what's the most significant unsolved problem?"
- "How does this project connect to our long-term product direction?"
- "Is this the highest-leverage thing we could be working on?"
