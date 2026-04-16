# Design principles reference

This file expands on the conceptual toolkit referenced in the main skill. Read this when you need deeper context on why a principle matters or how to apply it during problem framing.

## Jobs to be done

Source: Clayton Christensen, Tony Ulwick, Alan Klement; applied through goal-directed design (Alan Cooper, About Face).

People don't buy products; they hire them to make progress in their lives. A job to be done is the underlying motivation that causes someone to adopt a product.

**How to apply during problem framing:**

- Ask "what progress is the user trying to make?" before asking "what features do they need?"
- Identify the current solution the user is "hiring" (even if it's a spreadsheet, sticky notes, or doing nothing). Understand why it's falling short.
- Define the job at the right altitude. Too high ("be more productive") is useless. Too low ("check a box") misses the motivation. The right level: "feel confident nothing important falls through the cracks."
- Consider the four forces of switching: push (frustration with current solution), pull (attraction of new solution), anxiety (fear of switching), and habit (comfort with status quo). All four must be addressed.
- The job stays stable even as solutions change. "Stay informed about what my team is doing" has been the same job for decades.

## Mental models

Users don't approach your product with a blank slate. They carry expectations from every other product, tool, and experience they've used. These expectations form their mental model: an internal representation of how they think the system works.

**How to apply during problem framing:**

- When users are confused, check whether the product's behavior matches their mental model. Often the product works correctly but contradicts what users expect.
- Mental models are shaped by the interfaces ecosystem: all the tools users interact with alongside yours. If every other tool in the space uses drag-and-drop, your users expect drag-and-drop.
- Mental models vary by expertise. A power user's model is more detailed and accurate than a new user's. Frame problems by user segment when mental models diverge significantly.
- Changing a mental model is expensive. If your design requires users to unlearn something, that's a cost that should be explicitly weighed during framing.

## The interfaces ecosystem

Source: Applied from competitive analysis and semiotic thinking about the sign systems users inhabit.

Your product exists within an ecosystem of tools the user interacts with. This ecosystem shapes expectations about interaction patterns, terminology, information architecture, and visual conventions. Understanding the ecosystem is not optional benchmarking; it's understanding the language your users already speak.

**How to apply during problem framing:**

- Map the tools users interact with alongside yours. These shape expectations more than your own product's history does.
- Identify conventions that are so established they function as a shared language. Breaking these conventions has a cost; sometimes that cost is worth it, but it must be conscious.
- Look for patterns across the ecosystem, not just in direct competitors. Adjacent tools (communication, project management, documentation) all contribute to the user's mental model.
- When there is no established ecosystem (new product category), look at analogous ecosystems in other domains for structural patterns.

## Interface paradigm and metaphor

Source: Semiotic analysis; Garrett (The Elements of User Experience), specifically conceptual models in the structure plane.

Every product is built on a foundational metaphor. A shopping cart is a metaphor that implies "put things in, take things out." A canvas implies "infinite space, free arrangement." A feed implies "chronological, ephemeral, scroll to see more." These metaphors are not decoration; they are the deep structure that shapes what users expect the product to do.

**How to apply during problem framing:**

- Identify the foundational metaphor of the current product or feature. Is it a document? A canvas? A conversation? A dashboard?
- Evaluate whether the metaphor still serves the user's job. A metaphor that worked for a simple product may break when complexity increases. Slate's "magazine" metaphor for the web didn't survive because the medium's affordances contradicted the metaphor.
- When the metaphor breaks (users expect behaviors the product can't deliver because the metaphor implied them), the problem may be at the paradigm level, not the feature level. This is a more fundamental problem that requires a different kind of solution.
- Don't take metaphors too literally. The metaphor should guide expectations without constraining design to a real-world analog that doesn't fit the medium.

## Norman's three levels of design

Source: Don Norman, Emotional Design.

Products operate on three levels simultaneously:

- **Visceral:** Immediate sensory reaction. How does it look and feel at first glance? This is pre-conscious; users react before they think.
- **Behavioral:** The experience of use. Is it effective? Easy? Satisfying? This is where usability lives.
- **Reflective:** Meaning and identity. What does using this product say about me? How do I feel about it after the fact? This is where brand, trust, and long-term attachment live.

**How to apply during problem framing:**

- Identify which level matters most for this project. Most product design work focuses on behavioral, but visceral and reflective matter too.
- When users describe a product as "annoying," "stressful," or "confusing," those emotional responses point to failures at specific levels. "Confusing" is usually behavioral. "Cheap-feeling" is visceral. "Embarrassing to use in front of colleagues" is reflective.
- A product can succeed at one level and fail at another. A tool that's functionally excellent but feels ugly (visceral failure) or makes users feel incompetent (reflective failure) still has a real problem worth solving.
- For products where reflective experience matters (journaling, personal finance, health), framing must account for the emotional job, not just the functional job.

## Interfaces have meaning (semiotic perspective)

Source: Communication Design and semiotic studies; applied to interface design.

Every design element is a sign that communicates meaning. Color, position, size, typography, whitespace, motion, labels; these are all part of a sign system that users read and interpret. Good design isn't just usable; it communicates clearly. Bad design isn't just hard to use; it says the wrong thing.

**How to apply during problem framing:**

- When framing a usability problem, ask: is the issue that users can't do the action, or that the interface doesn't communicate that the action is possible? This is Norman's distinction between affordances (what's possible) and signifiers (what's communicated).
- Consider what the interface says about importance. Size, position, and contrast create a hierarchy that tells users what matters most. If users miss a critical action, the hierarchy may be saying "this isn't important."
- Terminology and labeling are acts of communication. If users misunderstand a feature, the label may be using the wrong sign. Internal jargon that makes sense to the team may mean nothing (or the wrong thing) to users.
- Consistency in sign systems builds trust. When the same visual treatment means different things in different parts of the product, users lose confidence in their ability to read the interface.

## Goal-directed design

Source: Alan Cooper, About Face.

Design for user goals, not features. A goal is the end state the user wants to reach. Features are means to that goal.

**How to apply during problem framing:**

- Define user goals before listing features. "I want to know my project is on track" is a goal. "View a Gantt chart" is a feature.
- Use personas grounded in goals, context, and behavior patterns. "Marketing manager, 35, NYC" is useless. "Needs to coordinate campaign launches across three time zones with no direct authority over contributors" is useful.
- Distinguish end goals (what the user wants to achieve), experience goals (how they want to feel), and life goals (who they want to be).
- Scenarios are more useful than use cases. A scenario tells a concrete story; a use case is abstract.

## Garrett's five layers (diagnostic use)

Source: Jesse James Garrett, The Elements of User Experience.

The five planes from abstract to concrete: strategy → scope → structure → skeleton → surface. Each plane depends on the ones below it. Decisions at lower planes ripple upward; choices at higher planes are constrained by what's below.

Within each plane, there's a dual nature: functionality-oriented (tasks, interaction) and information-oriented (content, architecture). Most products are a hybrid of both.

**Strategy:** Product objectives + user needs. The foundation.
**Scope:** Functional specifications + content requirements. What's in, what's out.
**Structure:** Interaction design + information architecture. How features fit together; how users navigate the content.
**Skeleton:** Interface design + navigation design + information design. The layout, the controls, the presentation of information.
**Surface:** Sensory design. What users see, hear, touch.

**How to use as a diagnostic during problem framing:**

- When a problem is unclear, identify which layer it lives in. "Users can't find things" might be a structure problem (bad IA), a skeleton problem (bad navigation), or a surface problem (bad visual hierarchy). The fix is different for each.
- Solving a problem at the wrong layer wastes time. A surface redesign won't fix a structural problem. New features (scope) won't fix a strategy problem.
- When a product feels "off" but nobody can explain why, walk the layers from bottom to top. Is the strategy clear? Does the scope match the strategy? Does the structure support the scope? Does the skeleton make the structure navigable? Does the surface communicate all of this clearly?
- Use this to communicate with cross-functional partners. Engineers often think in terms of scope and structure. Executives often think in terms of strategy. Visual designers think in terms of surface. Naming the layer helps everyone see the same problem.

## Evidence over intuition

Source: Jakob Nielsen and Hoa Loranger, Prioritizing Web Usability; applied broadly.

Ground every framing decision in evidence: data, research, observed behavior. When evidence is missing, name the gap explicitly and propose how to fill it.

**How to apply during problem framing:**

- Define success metrics before designing. If you can't measure it, you can't know whether you solved it.
- Prioritize problems by severity and frequency. A problem affecting 80% of users mildly may matter more than one affecting 5% severely; or not. Frame the trade-off explicitly.
- Don't confuse preference data with behavior data. What users say they want and what they do are often different. Frame around observed behavior when possible.
- Assumptions are acceptable when stated as assumptions, not disguised as facts.

## Design thinking as a process

Source: Tim Brown, Change by Design.

Design thinking is a methodology for approaching complex problems through empathy, ideation, prototyping, and iteration. It's not linear; it's a set of modes you move between as the problem demands.

**How to apply during problem framing:**

- Start with empathy. Understand the problem from the user's perspective before the business perspective. Both matter, but user understanding comes first.
- Frame problems as "how might we" questions: broad enough for creative solutions, specific enough to act on.
- Prototype early to learn, not to ship. When framing reveals big unknowns, plan for quick experiments before committing.
- Tailor the process to the project. Not every project needs every step. The process serves the problem, not the other way around.
