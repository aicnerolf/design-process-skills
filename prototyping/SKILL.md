---
name: prototyping
description: >
  Build interactive prototypes that embody design principles, not just functional
  requirements. Covers: establishing project context before building, selecting
  appropriate technology and fidelity, ensuring all states are accounted for,
  applying accessibility standards, and constructing artifacts that reflect
  deliberate design thinking rather than default developer conventions. Trigger on:
  "build a prototype," "build this," "code this," "create a prototype," "make this
  interactive," "build a page," "implement this design," "make this responsive,"
  "turn this into code," or any moment where a design needs to become a functional
  artifact. Also trigger when someone shares a Figma file, screenshot, wireframe,
  moodboard, or design reference and asks to build from it. Use this skill broadly;
  any time design work needs to be constructed as a working artifact, this skill applies.
---

# Prototyping

## What this skill does

This skill guides the construction of interactive prototypes and functional artifacts. It ensures that what gets built reflects deliberate design thinking; that the principles, frameworks, and decisions from problem framing, research, design, and validation are carried into the actual artifact, not abandoned the moment code is written.

This skill is fundamentally adaptive. The context, technology, inputs, and fidelity change with every project. What remains constant is the standard: every prototype should feel like it was built by someone who understands design principles, not merely someone who can write code.

## Core principle

A prototype is not a demonstration of technical capability; it is a design artifact that communicates, tests, and embodies a hypothesis. Every decision in its construction; layout, spacing, hierarchy, typography, interaction behavior, state handling; should reflect the same intentionality that informed the design thinking behind it. If the prototype does not carry the design principles forward, it undermines the work that preceded it.

## Before building anything

Read the context. Infer what you can from the inputs provided, the conversation history, and the design work that preceded this moment. Then build.

Ask only when something genuinely critical is missing or ambiguous. If a Figma file is shared with "build this," start building. If a vague request arrives with no inputs, ask. The threshold is: **would building without this information produce something fundamentally wrong, or merely imperfect?** If imperfect, build and refine. If fundamentally wrong, ask first.

When context is unclear, these are the questions that matter:

- **What inputs exist?** Figma file, wireframe, screenshot, moodboard, design system, existing codebase, or nothing. The inputs determine the starting point.
- **What fidelity and why?** Match the artifact to the hypothesis. Low fidelity for flow validation, mid-to-high for interaction and affordance validation, high fidelity for visceral experience. Do not default to high fidelity without reason.
- **What technology?** HTML/CSS/JS, React, a specific framework, or aligned with an existing codebase. If unspecified, choose what best serves the prototype's purpose and state the choice.
- **What constraints?** Device targets, responsive requirements, existing brand guidelines or tokens.

Bias toward building. A prototype that exists and needs refinement is more valuable than a conversation about what the prototype should eventually be.

## Construction standards

These apply to every prototype regardless of technology, fidelity, or context.

### Design principles in code

The prototype must embody the same design principles that informed the design thinking:

- **Visual hierarchy must be deliberate.** Size, weight, color, contrast, and position should guide the user's attention in the intended order. If every element carries equal visual weight, the hierarchy has failed.
- **Spacing must be systematic.** Use a consistent spacing scale. Whitespace communicates grouping and separation; tight spacing signals relatedness, generous spacing signals boundaries. Do not use arbitrary values.
- **Typography must establish rhythm.** A clear type scale with intentional size, weight, and line-height relationships. Body text optimized for readability (appropriate measure, adequate line-height). Headings that create scannable structure.
- **Interfaces have meaning.** Every element communicates something. A button's color, size, and position assert its importance. An icon's placement signals its function. Empty space around an element elevates it. Build with awareness that users read the interface as a system of signs.
- **Interaction patterns must match user expectations.** Respect the conventions established by the interfaces ecosystem. When deviating from convention, ensure the deviation is clearly communicated through the interface itself.

### States are non-negotiable

No prototype is complete until these states are addressed. Not all apply to every component, but each must be consciously considered:

- **Default.** The baseline state.
- **Loading.** What does the user see while data is being retrieved or processed?
- **Empty.** What appears when there is no content? Empty states are a communication opportunity, not an afterthought.
- **Error.** What happens when something fails? How is the failure communicated? How does the user recover?
- **Success.** What confirms that an action was completed?
- **Hover / Focus / Active.** Interactive elements must respond to user engagement. Focus states are both a usability and accessibility requirement.
- **Disabled.** When an action is unavailable, communicate why and what would enable it.
- **Partial / In-progress.** What does a form look like half-completed? What does a list look like with one item versus fifty?
- **Edge cases.** Very long text, very short text, missing images, unusual data, no permissions.

### Accessibility is foundational

Accessibility is not an enhancement applied after construction; it is a structural requirement integrated from the beginning. Every prototype must meet WCAG AA standards:

- **Keyboard navigation.** Every interactive element must be reachable and operable via keyboard. Tab order must be logical. Focus must be visible.
- **Screen reader support.** Semantic HTML as the default. ARIA labels where semantic elements are insufficient. Meaningful alt text for images. Live regions for dynamic content updates.
- **Contrast ratios.** Minimum 4.5:1 for body text, 3:1 for large text and UI components. Verify, do not estimate.
- **Focus indicators.** Visible, consistent focus styles on all interactive elements. Never remove focus outlines without providing an equivalent alternative.
- **Reduced motion.** Respect `prefers-reduced-motion` for animations and transitions.
- **Touch targets.** Minimum 44x44px for interactive elements on touch devices.

### Responsive considerations

Unless explicitly scoped to a single viewport, prototypes should account for how the design adapts across breakpoints. At minimum, consider mobile and desktop. Responsive design is not merely scaling down; it frequently requires rethinking layout, hierarchy, and interaction patterns.

## Working with different inputs

**From a Figma file or design system:** Extract tokens (colors, typography, spacing, radii) and apply them precisely. Follow the component structure and naming conventions. Do not substitute with generic alternatives.

**From a wireframe or rough sketch:** Interpret the structural intent. Apply systematic spacing, a coherent type scale, and clear visual hierarchy. Fill in the design details that the wireframe leaves implicit; this is where design judgment matters most.

**From a screenshot or reference image:** Analyze the design principles at work (hierarchy, spacing rhythm, color relationships, interaction patterns) and reconstruct them faithfully. Do not replicate pixels; replicate the underlying logic.

**From a moodboard:** Extract the aesthetic direction (color temperature, contrast style, typographic character, density, emotional tone) and translate it into interface decisions. A moodboard guides the visceral and reflective qualities of the prototype.

**From nothing:** Ask about the intended audience, the product's existing visual language (if any), and the emotional register. Then apply systematic defaults: a clear type scale, a spacing system, a restrained color palette, and a hierarchy that prioritizes the user's primary task.

## Output format

When delivering a prototype, include:

```
## What was built
[What this prototype is, what it covers, what fidelity level and why.]

## Technology and setup
[What was used to build it. How to run or view it.]

## Design decisions
[Key design choices made during construction and the reasoning behind them. What principles from the design direction were applied and how.]

## States covered
[Which states were implemented. Which were intentionally deferred and why.]

## Accessibility
[What accessibility measures were implemented. Any known gaps.]

## Limitations and next steps
[What this prototype does not cover. What would need to change for production. What feedback is being sought.]
```

## Tone and style

- Precise about implementation details. Vague code produces vague results.
- Explain design decisions embedded in the code, not just the code itself.
- Flag trade-offs. If a shortcut was taken for speed, name it.
- Treat the prototype as a design artifact, not a technical exercise.

## What this skill does NOT do

- Determine what to build. If the design direction is not established, return to the design and systems thinking skill.
- Validate the design. This skill constructs the artifact; the validation skill evaluates it.
- Produce production-ready code by default. Prototypes are hypotheses made tangible. Production readiness is a separate, explicit scope decision.
- Substitute for design judgment. When inputs are ambiguous or incomplete, ask rather than default to generic solutions.

## Usage examples

**Building from design artifacts:**
- "Here is the Figma file. Build a responsive prototype of the onboarding flow."
- "Build this screen from the wireframe I shared. Mid-fidelity; I need to test the interaction."
- "Implement the design system components from this token file."

**Building from references:**
- "Here is a screenshot of what I want. Recreate it as an interactive prototype."
- "I have this moodboard. Build a landing page that captures this aesthetic direction."

**Specifying fidelity:**
- "Build a low-fi clickthrough to test the user flow. Structure matters; visuals don't."
- "I need a high-fidelity prototype. We are testing how this experience feels."

**Adapting context:**
- "This needs to work on mobile. Build it mobile-first."
- "Use our existing React component library for this."
- "There is no design system. Use sensible defaults but keep it systematic."

**Ensuring completeness:**
- "What states are missing from this prototype?"
- "Add error handling and empty states to what we built."
- "Review this prototype for accessibility gaps."
