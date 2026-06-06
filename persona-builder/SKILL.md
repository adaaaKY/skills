---
name: persona-builder
description: >
  Build a rich, structured UX persona as a Markdown document that can be fed into design flow
  analysis, critique, or evaluation skills. Use this skill whenever the user wants to create a
  user persona, define a target user, describe a customer segment, or build a persona profile for
  UX analysis. Trigger on phrases like: "create a persona", "build a persona for", "define my
  target user", "who is my user", "make a persona", "I need a persona for", "create a user profile",
  "define the customer for this flow", or any time the user wants to characterize a user for UX,
  design, or product purposes. Also trigger when a user asks to analyze a design flow "for [type
  of user]" and no persona document already exists.
---

# Persona Builder

Generates a detailed, structured UX persona as a Markdown document. The persona is designed to
be reusable — it can be passed directly into design flow analysis, critique, or heuristic
evaluation skills.

---

## Step 1: Gather Context via Interview

Before writing anything, interview the user. Ask **one question at a time** to avoid overwhelming
them. Gather answers to the following — stop early if the user says they have enough or wants to
proceed.

### Required inputs (always ask these):
1. **Product / service context** — What product, feature, or service is this persona for?
2. **Persona archetype** — Do they have a name in mind, or a user type they're imagining
   (e.g., "busy parent", "first-time investor", "power user")?
3. **Primary user goal** — What is the #1 thing this persona is trying to accomplish?

### Optional enrichment (ask if not already clear from context):
4. **Known demographics** — Age range, location, occupation, life stage — or should Claude infer?
5. **Key pain point** — What is the biggest frustration or blocker this user faces today?
6. **Tech fluency level** — Novice, intermediate, or advanced? Mobile-first or desktop?
7. **Trust triggers** — What makes this user trust or distrust a product?
8. **Accessibility considerations** — Any known physical, cognitive, or situational constraints?
9. **AI usage** — Do they use AI tools (e.g., ChatGPT, Alexa, Copilot)? For what kinds of tasks?
10. **Social media behavior** — Are they a passive consumer, casual poster, or active content creator? Which platforms?

**Inference rule**: If the user has already provided context (e.g., a product description, design
brief, or prior conversation), extract answers from that context first and only ask about genuine
gaps. Never ask something already answered.

---

## Step 2: Generate the Persona Document

Once you have enough to proceed (at minimum: product context + archetype + primary goal), generate
the full persona as a Markdown document using the template below.

Be specific and concrete. Avoid generic filler like "wants a seamless experience" — instead write
things like "expects to complete checkout in under 3 taps without re-entering saved card details."

---

## Persona Template

```markdown
# Persona: [Full Name], [Age]
**Archetype:** [Short label, e.g. "The Reluctant Upgrader" or "The Efficiency Maximizer"]
**Product Context:** [Product or service this persona is scoped to]

---

## At a Glance
> "[A one-sentence quote that captures this persona's core attitude toward the product or problem space.]"

| Field | Detail |
|---|---|
| Age | |
| Location | |
| Occupation | |
| Life Stage | |
| Income Range | |
| Education | |

---

## Psychographics
- **Values:** [What they care about deeply — e.g., efficiency, family, independence, status]
- **Personality:** [2–3 traits that shape how they interact with products]
- **Lifestyle:** [Relevant context about how they spend their time]

---

## Goals & Motivations
### Primary Goal
[The #1 thing they want to accomplish with this product. Be specific.]

### Secondary Goals
- [Goal 2]
- [Goal 3]

### Emotional Drivers
[What emotional need does this product fulfill? e.g., "Feels in control", "Avoids embarrassment", "Saves face with family"]

### Definition of Success
[What does "this worked perfectly" look like for them?]

---

## Pain Points & Frustrations
### Primary Pain Point
[The biggest blocker or frustration today. Be concrete.]

### Additional Frustrations
- [Frustration 2]
- [Frustration 3]

### Current Workarounds
[How do they cope today without an ideal solution?]

### Failure States
[What makes them abandon a flow, give up, or call support?]

---

## Tech Behavior & Device Usage
- **Primary Device:** [Mobile / Desktop / Tablet — and OS if relevant]
- **Usage Context:** [When and where do they typically use this product? e.g., "commuting on phone", "at desk during work hours"]
- **Digital Fluency:** [Novice / Intermediate / Advanced]
- **Apps & Tools They Already Use:** [Relevant comparables that shape their expectations]
- **Usage Frequency:** [How often do they engage with this type of product?]

---

## AI Usage
- **Comfort Level:** [Enthusiast / Pragmatic adopter / Skeptic / Unaware]
- **Tools They Use:** [e.g., ChatGPT for writing, Alexa for home control, Copilot at work, Google Gemini for search]
- **How They Use AI:**
  - Search replacement: [Yes / Sometimes / No — e.g., "asks ChatGPT instead of Googling"]
  - Creative tasks: [Yes / Sometimes / No — e.g., "uses AI to draft emails or captions"]
  - Work tasks: [Yes / Sometimes / No — e.g., "uses Copilot in Excel or Outlook"]
- **Expectations of AI in Products:** [What do they expect when a product uses AI? e.g., "Expects recommendations to feel personal, not robotic", "Distrusts AI-generated content labels", "Comfortable with AI chat support as first line"]
- **Trust in AI Recommendations:** [How much do they let AI drive decisions vs. just inform them?]

---

## Mental Models & Expectations
- **Prior Experience Analogy:** [What product or experience does this user compare yours to? e.g., "Expects it to work like Amazon checkout"]
- **Navigation Expectations:** [How do they expect to move through the product?]
- **Vocabulary:** [Terms they use vs. terms they don't recognize]
- **Assumptions They Bring In:** [What do they assume is true before even opening the product?]

---

## Trust & Decision Drivers
### What Builds Trust
- [Trust signal 1 — e.g., "Recognizable brand logos", "Clear return policy upfront"]
- [Trust signal 2]

### What Triggers Abandonment
- [Abandonment trigger 1 — e.g., "Asks for too much personal info too early"]
- [Abandonment trigger 2]

### How They Evaluate Options
[How do they compare or decide? e.g., "Reads reviews first", "Asks a friend", "Judges by visual quality of the app"]

---

## Social Media Behavior
- **Platforms:** [Which platforms they use and how often — e.g., "TikTok daily, Instagram weekly, LinkedIn occasionally"]
- **Engagement Mode:** [Passive consumer / Casual engager (likes, comments) / Active poster / Content creator]
- **Content They Create (if any):** [e.g., "Posts trip photos", "Shares book recs in Stories", "Produces YouTube reviews"]
- **How Social Proof Shapes Decisions:**
  - Do they check social media before trying a new product or service? [Yes / Sometimes / No]
  - Do they trust influencer recommendations, peer reviews, or neither?
  - Would a shareable moment (e.g., "I finished a book!") motivate engagement, or feel performative to them?
- **Sharing Triggers:** [What would make them organically share something from this product? e.g., "A satisfying completion screen", "A funny or surprising recommendation", "A stat about how many hours they've listened"]

---

## Accessibility & Situational Constraints
- **Physical/Sensory:** [Any known or likely physical constraints — e.g., low vision, motor impairment]
- **Cognitive:** [Attention, memory, literacy considerations]
- **Situational:** [Environmental constraints — e.g., "Often using one-handed while holding coffee", "Interrupted frequently", "Low-bandwidth connection"]
- **Language:** [Primary language, fluency in product's language]

---

## Design Implications
> Use this section to translate the persona into actionable design guidance.

- **Prioritize:** [What the design must nail for this persona]
- **Avoid:** [What will lose this persona immediately]
- **Open Questions:** [What we still don't know about this persona that would be worth researching]
```

---

## Step 3: Review & Edit

After generating the full persona, ask the user:

> "Does this look right? Is there anything you'd like to change, add, or adjust?"

Apply any edits the user requests — one round at a time — and re-ask until the user confirms they're
happy with the persona. When the user indicates no further edits are needed, proceed to Step 4.

---

## Step 4: Save to File

Once the user is satisfied, ask:

> "Would you like to save this persona as a Markdown file?"

If yes:
- Suggest a default filename based on the persona's name, e.g. `persona-marcus-webb.md`
- Let the user confirm or change the filename
- Save the file to the project root (or a `/personas` folder if one exists)
- Confirm the file path after saving

If no, skip saving and proceed to Step 5.

---

## Step 5: Offer Next Steps

After the persona is finalized (and optionally saved), offer the user two follow-up options:

1. **Use it for analysis** — Offer to pass this persona into a design flow analysis (if that skill
   is available) to evaluate a screen, flow, or prototype against it.
2. **Build another persona** — Offer to create a second persona if they want to compare user types.

---

## Quality Rules

- **No generic filler.** Every field should contain something that couldn't be copy-pasted into a
  different persona unchanged. If you catch yourself writing "wants an easy experience," rewrite it.
- **Stay grounded.** If the user gave you real context (a PRD, a product description, a job-to-be-done),
  anchor every section to that reality. Don't invent details that contradict the product.
- **Be opinionated about Design Implications.** This section should feel like a UX strategist wrote
  it, not a content generator. Make concrete calls.
- **Accessibility is not optional.** Even if the user didn't mention it, include at least one
  realistic situational constraint. All users encounter situational accessibility challenges.
- **AI usage should inform recommendation UX.** A persona's AI comfort level directly predicts
  how they'll respond to algorithmic recommendations, chatbot support, and "AI-curated" labels.
  Make this section specific enough to be actionable — "uses ChatGPT daily for search" is more
  useful than "comfortable with AI."
- **Social media is about social proof, not just platform.** The most design-relevant output from
  this section is whether social proof (reviews, shares, friend activity) influences their decisions,
  and whether shareability is a motivation or an annoyance for this persona.
- **The quote must feel human.** It should sound like something a real person would say in a
  user interview, not a marketing tagline.
