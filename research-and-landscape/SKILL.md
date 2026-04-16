---
name: research-and-landscape
description: >
  Understand the problem space through research, competitive analysis, and landscape
  mapping before designing solutions. Covers: gathering user feedback, analyzing
  data, benchmarking competitors and adjacent tools, mapping the ecosystem users
  operate in, and synthesizing findings into actionable insights. Trigger on:
  "what do users say about this," "what does the competition do," "research this,"
  "benchmark," "competitive analysis," "what's out there," "how do others solve this,"
  "what do we know about our users," "help me understand the landscape," "what data
  do we have," or any moment where understanding the problem space is needed before
  designing. Also trigger when someone says "I need to look into this before designing,"
  "let's see what exists," or "what can we learn from other products." Use this skill
  broadly; any time research or landscape understanding is needed to inform design
  decisions, this skill applies.
---

# Research and landscape

## What this skill does

This skill supports the gathering of evidence, the analysis of the competitive landscape, and the development of a grounded understanding of users before design work begins. It ensures that design decisions are rooted in what is actually happening, not in assumptions or inherited narratives.

The depth and focus of research adapts to the project. A micro-interaction refinement demands different investigation than a new product initiative. The underlying questions remain consistent; the scope shifts.

## Core principle

Users construct their mental models from the entire ecosystem of tools they interact with, not solely from yours. Understanding the landscape is not an exercise in cataloguing competitor features; it is an exercise in comprehending the expectations, conventions, and behavioral patterns users already carry when they encounter your product. Research the ecosystem, not merely the competition.

## Conceptual toolkit

These lenses shape how research is conducted and how findings are interpreted. They should be actively applied, not passively acknowledged.

**The interfaces ecosystem.** Map the constellation of tools users operate alongside yours. These adjacent products establish conventions for interaction patterns, terminology, information architecture, and visual language. Users do not evaluate your product in isolation; they evaluate it against everything else they use. A pattern that contradicts the dominant ecosystem carries inherent friction. If a departure from established convention is being considered, it must be rigorously justified; not merely "better in theory," but demonstrably superior in the specific context of the user's actual job.

**Mental models.** Research should reveal not just what users do, but what they expect. Mental models are the invisible architecture users bring to every interaction. When user behavior seems irrational, it is often perfectly rational within the context of their mental model. Understanding these models is essential to designing experiences that feel intuitive rather than merely functional.

**Interface paradigm and metaphor.** When studying the landscape, attend to the foundational metaphors competitors employ. A canvas metaphor implies different capabilities than a document metaphor. Users who are accustomed to one paradigm will resist or misinterpret another unless the new paradigm offers clearly superior alignment with their actual goals. Note which metaphors are so pervasive they have become invisible conventions.

**Norman's three levels.** Research should address all three levels of experience. Behavioral data (analytics, task completion, error rates) captures the functional layer. But visceral reactions (first impressions, aesthetic responses) and reflective meaning (what users feel about the product after the fact, whether it aligns with their identity) require different methods: qualitative interviews, observation, emotional response testing.

**Interfaces have meaning.** When studying competitor products or evaluating user feedback, read the interface as a system of signs. What does each product communicate through its hierarchy, terminology, and visual treatment? Where does the communication succeed, and where does it mislead? Users who report being "confused" are often experiencing a semiotic failure: the interface is saying something different from what the system actually does.

**Garrett's layers as diagnostic.** When research surfaces problems in your own product, use the five layers to locate them precisely. User complaints about "navigation" might indicate a skeleton problem (poor layout), a structure problem (flawed information architecture), or a scope problem (missing content). Research that identifies the correct layer saves the design team from solving the wrong problem.

**The context gap.** Every interface is designed within a specific context: the team's knowledge at the time, the business pressures, the technological constraints, the assumptions about who the user is and what they need. But every interaction with that interface occurs in an entirely different context: the user's device, environment, mental state, prior experiences, current goals, and the moment they happen to be in. There is always a gap between the context in which something was designed and the context in which it is actually experienced. This gap shifts constantly; the same interface is encountered differently by different users, and differently by the same user at different moments. Research must actively surface and account for this gap. Understanding what the team intended is not sufficient; understanding what the user actually encounters, in their actual circumstances, is what matters. When research reveals that users are not behaving as expected, the explanation often lies in this gap rather than in the design itself.

## The research process

### Step 1: Define what you need to learn

Before gathering anything, establish with precision what questions this research should answer. Derive these from the problem frame (if one exists) or articulate them now.

Recurrent research questions include:

- What do users currently experience? Where do they encounter friction?
- What do they expect based on other tools they use?
- What has the organization already attempted? What was learned?
- What does the competitive and adjacent landscape look like?
- What existing data is relevant and available?

Calibrate the research scope to the project. A full competitive analysis for a button redesign is disproportionate. Omitting landscape research for a new product is negligent.

### Step 2: Gather user evidence

Draw from every available source. The most complete understanding emerges from triangulating multiple types of evidence:

- **Behavioral data.** Analytics, funnels, usage patterns, drop-off points. What are users actually doing? This reveals the what.
- **Direct feedback.** Support tickets, NPS responses, customer calls, internal communication channels. What are users articulating? This reveals the felt experience.
- **User conversations.** Interviews, usability tests, customer calls. What do users describe in their own language? What do they struggle to articulate? This reveals the why.
- **Internal knowledge.** What does the team already know? What have prior projects uncovered? What have sales, support, or customer success been consistently hearing?
- **Context of use.** Investigate the circumstances in which users actually encounter the product. The conditions under which an interface was designed are never identical to the conditions under which it is experienced. Device, environment, emotional state, competing demands, and the user's immediate goals all shape the interaction. When possible, observe or inquire about these contextual factors; they frequently explain behavior that otherwise appears irrational.

No single source provides a complete picture. Data reveals what happens; conversations reveal why. Support tickets surface pain points that analytics miss. Triangulate deliberately.

When direct user access is constrained (by timeline, resources, or organizational barriers), lean more heavily on existing data and internal knowledge. Acknowledge the gap transparently; do not pretend it does not exist.

### Step 3: Map the landscape

Investigate how others address this problem or analogous problems. The objective is not to compile feature inventories; it is to understand:

- **What can we adopt and build upon?** Patterns users already comprehend. Conventions that would be costly to violate without compelling justification.
- **What mistakes should we avoid?** Where have others attempted and failed? What approaches generate confusion or friction? Learning from others' failures is as valuable as learning from their successes.
- **What translates to our context?** Not every pattern is transferable. A convention that serves a consumer application may misfire in an enterprise context. Be specific about what is relevant and why.
- **What constitutes the ecosystem?** Map the tools users employ alongside yours. These shape expectations around navigation, terminology, interaction patterns, and information architecture. If every comparable tool in the space employs a certain convention, your users will anticipate the same.
- **Where is the gap?** What are others doing inadequately? Where does an opportunity exist to be meaningfully superior? This is where differentiation originates.

**Calibrate the lens to the problem:**

- Refining a micro-interaction → study micro-interactions in comparable products
- Redesigning information architecture → study how similar tools organize content and navigation
- Building a new product → study the complete experience of competitors and adjacent tools
- Improving a specific flow → study how others handle the equivalent flow

Align the depth of investigation with what you are actually designing. Analyzing everything when you need to understand only one layer is wasteful.

**When no reference exists:** If you are working in a space with no direct comparables, examine analogous problems in unrelated domains. How do structurally similar challenges get addressed elsewhere? If nothing meaningfully applies, acknowledge that the landscape step is less pertinent and proceed. Do not fabricate a competitive analysis where none is warranted.

### Step 4: Synthesize findings

Raw data is not insight. Synthesis means transforming evidence into understanding the team can act upon.

- **Identify patterns.** What themes recur across multiple sources? What do users consistently struggle with? Where do competitors consistently succeed or fail?
- **Separate observations from interpretations.** "42% of users abandon at step 3" is an observation. "Users are confused by the permission model" is an interpretation. Present both; distinguish clearly between them.
- **Prioritize by consequence.** Not all findings carry equal weight. Foreground what is most consequential to the problem being addressed.
- **Connect to design implications.** Every significant finding should indicate what it means for the work ahead. "Users expect drag-and-drop because every comparable tool in the space employs it" implies a design constraint worth respecting.
- **Acknowledge gaps.** What could not be determined? What assumptions are being carried? What would merit further investigation?

## Strategic context and scalability

Research that serves only one project is useful. Research that builds cumulative understanding is substantially more valuable.

- **Maintain a living understanding of the landscape.** The competitive environment evolves continuously. Research conducted six months ago may no longer reflect the current state. Revisit landscape understanding periodically, not only at project inception.
- **Surface cross-team insights.** Research for one project often reveals findings relevant to adjacent teams or initiatives. Capture and distribute these proactively rather than allowing them to remain siloed.
- **Identify systemic patterns.** Look for recurring themes across multiple research efforts. If user confusion around permissions surfaces in three separate projects, the problem is systemic and warrants systemic attention.
- **Build shared research assets.** When practical, structure research outputs so they can be referenced by other teams and future projects. A well-structured landscape map or ecosystem analysis has value beyond the immediate initiative.

## Output format

When presenting research and landscape findings, employ this structure. Adapt the weight of each section to the project; not all sections require equal depth.

```
## Research scope
[What questions were we seeking to answer? What is the scope of this research relative to the project?]

## Key findings
[The most significant discoveries, prioritized by relevance to the design problem. Each finding states what was observed and what it implies for the work ahead.]

## User evidence
[What do users experience today? Pain points, behaviors, feedback, and representative quotes organized by theme. Sources identified.]

## Landscape and ecosystem
[How do others address this? Map of competitors and adjacent tools. What patterns exist? What succeeds, what fails, what is absent? How do these products shape user expectations?]

## What we can adopt
[Patterns, conventions, and approaches from the landscape that are applicable to our context, with reasoning.]

## What we should avoid
[Missteps, anti-patterns, and approaches that have proven problematic elsewhere, with reasoning.]

## Opportunities for differentiation
[Where is the gap? What can we do meaningfully better? Where does the evidence indicate unmet needs?]

## Context of use
[In what circumstances do users actually encounter this product or feature? What contextual factors (device, environment, emotional state, competing demands) shape the interaction? Where is the gap between the conditions under which this was designed and the conditions under which it is experienced?]

## Open questions and gaps
[What remains unknown? What assumptions are we carrying? What further investigation would be valuable?]
```

## Tone and style

- Professional and precise. Lead with findings, not methodology.
- Specific over general. "Three of five competitors employ inline editing" rather than "most competitors have similar patterns."
- Evidence-anchored. Every claim should trace to a source: data, a user quote, an observed pattern.
- Transparent about limitations. If the evidence is thin, acknowledge it. Do not overstate weak signals.
- Actionable. The team should conclude the reading with a clear understanding of the implications for the design work ahead.

## What this skill does NOT do

- Design solutions. This skill produces evidence and insight. Solutions follow.
- Conduct primary research. This skill helps structure, analyze, and synthesize research. Running user studies, surveys, or interviews is a distinct activity.
- Replace the problem frame. If the problem has not been articulated, address that first. Research without a clear question generates noise.
- Produce exhaustive reports for their own sake. Calibrate the depth to what the project genuinely requires. A week of research for a two-day design sprint is disproportionate.

## Usage examples

**Before a project:**
- "What do we know about how users handle task management? Help me assemble the evidence."
- "Map the landscape of collaboration tools with commenting features."
- "Help me understand how competitors approach onboarding flows."

**During research:**
- "Here are 15 support tickets about our search feature. Identify the patterns."
- "I examined five competitors. Help me organize what I found and surface the gaps."
- "Here is data from our analytics dashboard. What does it reveal about where users struggle?"

**Synthesizing findings:**
- "I have user interview notes, analytics data, and a competitive analysis. Help me synthesize this into a coherent presentation."
- "What are the key insights from this research and what do they imply for the design?"

**Landscape analysis:**
- "How do other products handle empty states in dashboards?"
- "What patterns exist for onboarding flows in enterprise SaaS?"

**Systemic research:**
- "We keep seeing the same user confusion across multiple projects. Help me investigate whether this is a systemic issue."
- "Build a landscape overview that can serve as a reference for the whole team, not just this project."
