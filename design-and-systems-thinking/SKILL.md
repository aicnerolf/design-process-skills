---
name: design-and-systems-thinking
description: >
  Design solutions after the problem is framed and research is done. Covers: divergent
  exploration, sketching and brainstorming, prototyping at the right fidelity, thinking
  in systems, and making design decisions at the intersection of user needs, business
  needs, and technical feasibility. Trigger on: "help me design this," "let's explore
  solutions," "brainstorm ideas for," "how should this work," "prototype this,"
  "what are the options," "let's sketch this out," "design this feature," "how should
  we approach the interaction," "build me a prototype," or any moment where the
  work shifts from understanding the problem to designing the solution. Also trigger
  when someone says "I need to explore ideas," "let's diverge," "what could this
  look like," or "help me think through the design." Use this skill broadly; any time
  design work is happening, this skill applies.
---

# Design and systems thinking

## What this skill does

This skill guides the design of solutions after the problem has been articulated and the landscape is understood. It supports divergent exploration, deliberate convergence, and design decisions that account for user needs, business constraints, and technical feasibility simultaneously.

This skill addresses the thinking; it does not produce prototypes or implementation artifacts. When the design direction is established and a prototype is needed, transition to the prototyping skill.

## Core principles

**Better done than perfect.** A testable prototype in front of users holds more value than a polished design on a screen nobody has seen. Resist the impulse to refine before validating. Ship something, observe what happens, iterate. Perfectionism that delays learning is a liability.

**Diverge before you converge.** In the early stages of design, pursue quantity over quality. Generate as many distinct approaches as possible. There are no bad ideas at this stage; the objective is to explore the space broadly before narrowing. Convergence is a subsequent, deliberate act.

**Fidelity serves the hypothesis.** The level of detail in any prototype or exploration should correspond precisely to what is being validated:

- **Validating a flow or user journey:** Low fidelity. Rough sketches, wireframes, simple clickthrough prototypes. The structure matters; the visual treatment does not.
- **Validating interactions or affordances:** Mid to high fidelity. The prototype must behave realistically enough that users can assess whether the interaction communicates what is possible and responds as expected.
- **Validating the visceral experience:** High fidelity exclusively. When the question is how something *feels*; the emotional quality, the polish, the sensation of use; only a high-fidelity prototype yields honest feedback.

Constructing at the wrong fidelity is a waste of effort. A pixel-perfect mockup to evaluate a flow is over-investment. A wireframe to assess emotional resonance is under-investment. Align the artifact to the question.

**Three constraints, always.** Product design occurs at the intersection of feasibility (can this be built?), business viability (does this serve the organization's objectives?), and user desirability (does this enable the user to achieve their goal?). A solution that disregards any one of these will ultimately fail. Evaluate every idea against all three.

## Conceptual toolkit

These lenses should actively inform design decisions, not merely decorate the rationale.

**Interface paradigm and metaphor.** Every design rests on a foundational metaphor, and choosing or inheriting that metaphor is one of the most consequential decisions in the process. A shopping cart metaphor implies "put things in, take things out." A canvas metaphor implies "infinite space, free arrangement." These metaphors govern user expectations at a structural level. When designing, be deliberate about which metaphor you are employing. If the current paradigm no longer serves users, recognize that as a fundamental design problem, not a surface refinement.

**Mental models.** Design must account for what users already expect. A solution that is internally coherent but contradicts the mental models users carry from the interfaces ecosystem will generate friction. When extending or breaking an existing mental model, do so with clear intention and ensure the interface communicates the shift unambiguously.

**Interfaces have meaning.** Every design element communicates meaning. The position of a button asserts its importance. The color of a state indicator signals urgency or calm. Whitespace creates grouping and separation. Typography establishes hierarchy and tone. When evaluating design directions, interrogate not only whether users *can* accomplish the task but whether the interface *communicates* what is possible, what is important, and what will happen next. A design that functions correctly but communicates poorly is a design that will confuse.

**Norman's three levels.** Evaluate design explorations across all three levels. Does the visceral impression align with the product's identity? Does the behavioral experience (ease, effectiveness, satisfaction) meet the standard? Does the reflective meaning (what it says about the user, how they feel about it afterward) serve the product's emotional mandate? Most design work focuses exclusively on behavioral. The strongest work addresses all three.

**The context gap.** Remember that what you design in your specific context will be experienced by users in entirely different circumstances. A flow that feels obvious on a large monitor in a quiet office may be disorienting on a phone during a commute. Design with awareness that the conditions of use are never identical to the conditions of creation.

**Garrett's layers as diagnostic.** When a design direction is not working and the reason is unclear, identify which layer the problem inhabits. A layout that feels "off" might be a surface problem (visual hierarchy), a skeleton problem (element arrangement), or a structure problem (the underlying organization is flawed). Addressing the correct layer prevents wasted iterations.

## The design process

### Step 1: Diverge

Generate as many distinct approaches as possible. At this stage:

- Sketch by hand. Quick, rough, disposable. The objective is thinking, not presentation.
- Involve people from other disciplines when circumstances allow. Engineers, product managers, and support staff perceive problems differently. Their contributions during divergence produce solutions a designer working alone would not reach.
- Quantity over quality. Critical judgment is reserved for the subsequent step.
- Pursue non-obvious directions. The first idea is rarely the strongest. Push past the evident solutions to discover what lies beyond them.

When working with Claude: leverage this phase to rapidly generate multiple approaches. Request 3-5 fundamentally different ways to address the same problem. Do not settle on the first suggestion.

### Step 2: Evaluate and converge

Once a range of ideas exists, narrow them with deliberation. For each promising direction, interrogate:

- Does it address the user's actual job? (Refer to the problem frame.)
- Is it feasible within the technical constraints and timeline?
- Does it serve the business objectives?
- How does it integrate with the existing system? Does it introduce inconsistencies or fracture established patterns?
- What is the simplest version that would permit validation of the core hypothesis?

Avoid converging prematurely. Sustain 2-3 candidates long enough to compare them meaningfully. Eliminate ideas with evidence, not instinct.

Note: Claude makes it inexpensive to construct interactive prototypes. This may alter the traditional design calculus. Rather than selecting one direction and committing, it may be practical to prototype multiple directions and evaluate them all. Consider this when the cost of building is low and the cost of choosing incorrectly is high.

### Step 3: Think in systems

Before committing to any design direction, examine it within the context of the broader product.

- **Connections.** What other features, screens, or flows does this design touch? Modifications here may necessitate modifications elsewhere. Trace the ripple effects.
- **Scale.** If this feature serves 10 users, it may function adequately. What about 10,000? What about edge cases: empty states, error states, extremely long content, absent permissions, degraded connectivity?
- **States.** Default, loading, empty, error, success, partial, disabled. A feature is not designed until every state is accounted for.
- **Information architecture.** Where does this reside within the product? How do users discover it? How does it relate to adjacent elements? Does it respect or violate the product's existing organizational logic?
- **Existing patterns.** Does the product already have conventions this should follow? Where must it deviate, and is that deviation warranted? Unjustified deviation from internal conventions erodes coherence and user trust.
- **The foundational metaphor.** Does this design reinforce or contradict the product's underlying paradigm? If the product is built on a document metaphor and this feature introduces canvas-like behavior, that tension must be resolved deliberately.

Systems thinking is not a discrete phase; it operates throughout the design process. But an explicit assessment before committing to a direction prevents costly rework later.

## Strategic context and scalability

Design decisions that resolve one project are useful. Design decisions that establish patterns for the product are substantially more valuable.

- **Design for reuse.** When solving an interaction problem, consider whether the solution could generalize. A component, pattern, or convention established here might serve adjacent features or future work. Invest the additional thought to make solutions extensible when the cost of doing so is marginal.
- **Resolve design debt deliberately.** Complex products accumulate inconsistencies: patterns that evolved independently, conventions that diverge across features, interactions that contradict each other. When a project touches areas with existing design debt, evaluate whether to resolve it now or defer it consciously.
- **Influence the product's foundational systems.** At the most impactful level, design work shapes the product's core patterns: its navigation model, its information architecture, its interaction conventions, its visual language. When a project presents the opportunity to strengthen these foundations, recognize that as high-leverage work that extends well beyond the immediate deliverable.
- **Articulate the rationale.** Document not only what was designed but why. What alternatives were considered and rejected? What trade-offs were accepted? This reasoning becomes a resource for the entire team, preventing future designers from re-litigating settled decisions without context.

## Output format

Design output varies by project, but when presenting design explorations or recommendations, employ this structure:

```
## Design brief
[Concise summary: what we are designing, for whom, what hypothesis we are testing.]

## Explorations
[Multiple approaches considered. For each: what it is, how it works, what it optimizes for, what it sacrifices. Evaluate against the three constraints: user needs, business viability, technical feasibility.]

## Recommended direction
[Which approach and why. How it serves the user's job, the business objectives, and the technical reality. What trade-offs are accepted.]

## Fidelity and validation plan
[What fidelity is appropriate for the next step? What hypothesis does it test? What feedback are we seeking?]

## System considerations
[How this connects to the broader product. States, edge cases, scale, existing patterns affected, paradigm alignment.]

## Design rationale
[Key decisions and their reasoning. Alternatives considered and why they were set aside.]

## Open questions
[What is unresolved? What requires testing? What might alter this direction?]
```

## Tone and style

- Professional and precise. Present design rationale with clarity.
- Expose the reasoning, not merely the result. Articulate *why* this direction over the alternatives.
- Acknowledge trade-offs candidly. Every design decision gains something and relinquishes something. Name both.
- Resist preciousness. Designs are hypotheses to be validated, not artifacts to be defended.

## What this skill does NOT do

- Frame the problem. If the problem lacks clarity, return to the problem framing skill.
- Conduct research. If the landscape is not understood, address that first.
- Build prototypes. This skill produces design thinking and direction. Construction is handled by the prototyping skill.
- Write implementation specifications. This yields design explorations and rationale, not engineering documentation.
- Polish indefinitely. If the design is sufficient to validate the hypothesis, proceed.

## Usage examples

**Divergent exploration:**
- "I need to design a new onboarding flow. Generate five fundamentally different approaches."
- "Brainstorm ways to address this problem. I want breadth, not polish."
- "What are the distinct ways we could handle notifications in this product?"

**Evaluating directions:**
- "Here are three directions. Help me evaluate which best serves the user's job."
- "Is this design feasible given our constraints?"
- "What does this direction sacrifice? What are the trade-offs?"

**Systems thinking:**
- "What states am I overlooking in this design?"
- "How does this feature affect the rest of the product?"
- "What happens to this design at scale?"
- "Does this contradict any existing patterns in the product?"

**Systemic design:**
- "Can this solution generalize beyond this one feature?"
- "We have inconsistent patterns across three features. How should we reconcile them?"
- "What foundational pattern should we establish here that future work can build on?"
