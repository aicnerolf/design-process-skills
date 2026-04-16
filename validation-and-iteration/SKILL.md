---
name: validation-and-iteration
description: >
  Validate design work against defined goals and iterate based on what you learn.
  Covers: choosing the right validation method, evaluating results against success
  metrics, handling ambiguous data, deciding what to iterate on, and knowing when
  to ship. Trigger on: "how should we test this," "validate this design," "is this
  working," "what should we measure," "the data is ambiguous," "should we iterate
  or ship," "analyze these results," "usability test," "A/B test," "what do the
  numbers say," or any moment where design work needs to be evaluated against goals.
  Also trigger when someone says "we launched and here are the results," "how do
  we know if this is good enough," "what's the testing plan," or "help me interpret
  these results." Use this skill broadly; any time design work needs validation,
  evaluation, or iteration decisions, this skill applies.
---

# Validation and iteration

## What this skill does

This skill supports the evaluation of design work against its stated goals and guides the decisions that follow: ship, iterate, rethink, or reframe. It connects back to the success metrics established during problem framing and provides structure for testing, interpreting results, and determining next steps.

## Core principle

Validation is always relative to the goals defined at the outset. If clear goals and success metrics do not exist, return to the problem frame and establish them before attempting to validate anything. Testing without criteria is performance, not evaluation; it generates impressions but not answers.

## Conceptual toolkit

These lenses should inform how validation is planned, how results are interpreted, and what conclusions are drawn.

**Norman's three levels.** Validation should account for all three levels of experience, not only the behavioral. Standard usability testing captures whether users can complete tasks (behavioral). But visceral responses (first impressions, aesthetic reactions, sense of quality) and reflective meaning (how users feel about the experience afterward, whether it aligns with their identity and expectations) require different methods: qualitative conversations, emotional response observation, longitudinal follow-up. A design that performs well behaviorally but fails viscerally or reflectively still has a genuine problem.

**Interfaces have meaning.** When validating, attend not only to whether users accomplished the task but to whether the interface communicated what was intended. Did users understand what was possible? Did visual hierarchy guide their attention appropriately? Did labels and terminology convey the correct meaning? A high task-completion rate can mask communication failures if users succeeded through effort rather than clarity.

**Mental models.** Validation often reveals collisions between the user's mental model and the system's actual behavior. When users express confusion or take unexpected paths, investigate whether the design contradicts expectations they carry from the interfaces ecosystem. The problem may not be the design itself but the gap between what it communicates and what users anticipated.

**The context gap.** What functions in a controlled testing environment may falter in the conditions where users actually operate. Device, connectivity, environmental distractions, emotional state, and time pressure all shape the interaction. When possible, validate in circumstances that approximate real conditions of use. When not possible, acknowledge the gap and account for it in your interpretation.

**Garrett's layers as diagnostic.** When validation reveals a problem, locate it precisely. Users saying "I couldn't find it" might indicate a surface issue (visual hierarchy), a skeleton issue (navigation placement), a structure issue (information architecture), or a scope issue (the feature is absent). Misidentifying the layer leads to iterations that address symptoms rather than causes.

## Choosing the validation method

The appropriate method depends on two factors: what is being validated, and where the design stands in its lifecycle.

**What are you validating?**

- **Overall direction.** Does this approach address the right problem? Does it resonate with users? Methods: stakeholder reviews, concept testing, early feedback sessions with representative users.
- **A specific flow.** Can users navigate the journey successfully? Where do they hesitate or abandon? Methods: usability testing (moderated or unmoderated), task completion analysis, clickthrough prototype testing.
- **An interaction or affordance.** Do users comprehend what an element does? Does the interaction behave as they expect? Methods: usability testing at mid-to-high fidelity, first-use observation, think-aloud protocols.
- **The visceral experience.** Does this feel the way we intended? Does the sensory quality match the product's identity? Methods: high-fidelity prototype testing, qualitative feedback on emotional response, preference testing.
- **Business impact.** Is this moving the metrics that matter? Methods: A/B testing, analytics, funnel analysis, cohort comparison.

**Where is the design in its lifecycle?**

- **Pre-release.** Focus on whether the design resolves the problem and whether users can succeed with it. Usability testing, prototype validation, stakeholder alignment.
- **Post-release.** Focus on whether the design is achieving its goals in actual conditions. Analytics, A/B tests, user feedback, support ticket analysis.

Align the method to the question. A usability test cannot answer whether the design moves a business metric. Analytics cannot explain *why* users struggle. Choose accordingly.

## Evaluating results

### When results are clear

Compare outcomes against the success metrics from the problem frame. If the indicators confirm that users are better able to achieve their goals, the design is working. Document what succeeded and the reasoning behind it.

If indicators reveal the goals are not being met, identify where the design falls short. Is it a specific step in the flow? A misunderstood interaction? An incorrect assumption about user behavior? Metrics identify *that* something is underperforming; further investigation identifies *why*.

### When results are ambiguous

Ambiguous data is common and should not be treated as failure. The numbers are inconclusive, user feedback is mixed, or results partially meet the goal. When this occurs, several approaches are available:

- **Revisit the success metrics.** The original metrics may not be capturing what genuinely matters. If "time on task" is unchanged but users report significantly greater confidence, the metric may be inadequate, not the design.
- **Revisit the goals.** Ambiguous results sometimes reveal that the goal itself was insufficiently precise or overly ambitious. Sharpen it.
- **Define percentage of achievement.** Not every evaluation is binary. If the goal was a 20% improvement and the result is 12%, that represents partial success. Determine whether partial success is sufficient to proceed or whether the remaining gap justifies further iteration.
- **Examine the data from a different angle.** Segment by user type, device, entry point, or cohort. Ambiguous aggregate data frequently conceals clear patterns within subgroups.
- **Supplement with a different type of evidence.** If quantitative data is inconclusive, introduce qualitative methods (or the reverse). Speak with users who struggled. Review session recordings. The combination typically clarifies what neither source could resolve independently.

Do not manufacture certainty from weak evidence. It is more valuable to state "we do not yet have a clear answer; here is what we need to investigate further" than to extract conclusions the data does not support.

## Deciding what follows

After evaluating results, determine the appropriate next step:

- **Ship.** The design meets its goals. Proceed to release.
- **Iterate on specific issues.** The design is largely sound but has identifiable shortcomings. Address those shortcomings; revalidate if the changes are substantial.
- **Rethink the approach.** The design is not resolving the problem in a fundamental way. Return to the design phase with the knowledge acquired.
- **Reframe the problem.** The results suggest the problem was defined incorrectly or the goals were misaligned. Return to problem framing with fresh understanding.

Iteration should always be targeted. "Improve it" is not an actionable brief. "Users abandon at step 3 because the permission options are unclear; redesign that step to communicate the choices more effectively" is.

## When to stop iterating

There is no formula for this. Recognizing when a design is ready to ship is a judgment developed through experience, and it depends on the circumstances: the organization's priorities, the team's capacity, competitive pressure, and the severity of remaining issues.

Considerations that inform the decision:

- **Are the core goals met?** If the primary success metrics are being satisfied, remaining issues may be acceptable.
- **What is the cost of delay?** Additional iteration consumes time. If the market is shifting or users are enduring a poor current experience, shipping an imperfect improvement may be preferable to waiting for a flawless one.
- **What is the cost of shipping?** If remaining issues risk genuine harm (data loss, security vulnerabilities, erosion of trust), further iteration is warranted. If they are cosmetic or affect edge cases, the calculus shifts.
- **Can you iterate after release?** If the answer is yes and the outstanding issues are minor, ship and refine in production. If shipping is irreversible or the cost of post-release changes is prohibitive, exercise greater caution.

Better done than perfect. A design that ships at 80% and generates real-world learning is more valuable than a design that reaches 95% but never encounters an actual user.

## Strategic context and scalability

Validation that serves only one project is useful. Validation that builds organizational knowledge is substantially more valuable.

- **Identify systemic patterns.** When the same category of issue surfaces across multiple projects (unclear permissions, confusing empty states, inconsistent terminology), the problem is systemic. Escalate it beyond the immediate project and advocate for a systemic solution.
- **Build shared evaluation practices.** When a validation approach proves effective, document it so other teams can apply it. A well-structured testing protocol has value beyond the project that created it.
- **Contribute to collective understanding.** Validation frequently produces insights about users that extend beyond the specific feature being tested. Capture these broader findings and ensure they reach the teams and individuals who can benefit from them.
- **Challenge inherited assumptions.** Validation sometimes contradicts long-held beliefs about users or the product. When it does, treat this as valuable information rather than inconvenient noise. Circulate the finding; it may reshape other teams' work.

## Output format

When presenting validation findings and iteration recommendations, employ this structure:

```
## What we validated
[What design, what hypothesis, what method, what audience, what conditions.]

## Results
[What was observed. Data, user behavior, feedback. Observations separated clearly from interpretations.]

## Evaluation against goals
[How do results compare to the success metrics established in the problem frame? Met, partially met, not met, or ambiguous?]

## Interpretation
[What do the results signify? Why did we observe what we observed? What succeeded, what fell short, and why?]

## Recommendation
[Ship, iterate, rethink, or reframe. With specific reasoning anchored to the evidence.]

## If iterating: what to address
[Specific issues to resolve. What remains unchanged, what requires modification, and why.]

## Broader insights
[Findings that extend beyond this project. Patterns, user behaviors, or systemic issues that other teams should be aware of.]

## Open questions
[What remains unresolved? What would additional investigation clarify?]
```

## Tone and style

- Professional and precise. Present findings with candor; do not shape results to appear more favorable than they are.
- Distinguish observations from interpretations. "42% abandon at step 3" is an observation. "Users are confused by the permission model" is an interpretation. Present both; label each clearly.
- Acknowledge uncertainty. Ambiguous results are normal, not a failure. Do not impose clarity where none exists.
- Actionable. Every evaluation should conclude with a clear recommendation for what to do next.

## What this skill does NOT do

- Design solutions. If iteration is required, this skill identifies what to address; the design skill handles the redesign.
- Execute tests. This skill helps plan, interpret, and decide. Conducting usability tests, configuring A/B tests, or extracting analytics is a distinct activity.
- Guarantee answers. Some validation rounds produce more questions than answers. That is a legitimate and valuable outcome.

## Usage examples

**Planning validation:**
- "How should we test this prototype before launch?"
- "What is the appropriate validation method for this design?"
- "Help me construct a testing plan for this feature."

**Interpreting results:**
- "Here are the results from our usability test. Help me synthesize them."
- "We launched the new flow and here are the analytics. Is it achieving what we intended?"
- "The A/B test results are ambiguous. Help me determine what is actually happening."

**Making iteration decisions:**
- "Should we ship this or iterate further?"
- "The design partially met our goals. What should we do?"
- "Help me distinguish what to fix from what to accept."

**Revisiting goals:**
- "Our original metrics do not seem to capture what matters. Help me reconsider them."
- "The data is mixed. Should we redefine success criteria?"

**Systemic validation:**
- "We keep encountering the same usability issue across different projects. Is this a systemic problem?"
- "What did this round of testing reveal about our users beyond this specific feature?"
