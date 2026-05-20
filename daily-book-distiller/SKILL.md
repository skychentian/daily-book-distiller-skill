---
name: daily-book-distiller
description: Daily book recommendation and distillation skill. Use when an AI agent needs to recommend exactly one high-quality book based on the user's memory, current priorities, interests, and recent context, then produce a concise, faithful, insight-dense reading card with the book's core argument, counterintuitive insight, practical relevance, and a simple structure map. Suitable for scheduled daily reading tasks, founder/creator learning systems, business strategy reading, AI-era productivity learning, sales/marketing learning, team collaboration learning, and personal cognitive upgrade.
---

# Daily Book Distiller

Purpose: Recommend exactly one book per run and compress its real intellectual value into a short, useful reading card.

This is not a generic book-summary skill. Act like a rigorous reader plus a private reading advisor: first understand the book on its own terms, then connect it to the user's current context.

Core correction: Do not use a book as an excuse to give generic advice. The book itself should carry about 70% of the output. Application to the user should stay around 30%.

## Inputs to Consider

Before choosing a book, use the available context:

- Long-term memory or user profile
- Recent conversations or project notes
- Current business priorities
- Recurring weaknesses or bottlenecks
- Existing reading history if available
- The user's preferred surprise ratio or topic mix if available

If memory is unavailable, choose from well-known classics with high confidence.

## Book Selection Principles

Choose exactly one book.

Prioritize:

1. Classic value: books that have survived time, not short-term hype
2. Context fit plus occasional surprise: mostly match the user's current needs, sometimes introduce a distant field that creates a new lens
3. Cognitive gain: the book must change how the user sees a problem
4. Transferability: it does not need to be directly practical, but must offer a useful frame
5. No repetition: avoid books recently recommended if history is available

Recommended categories:

- Business strategy: positioning, competition, growth, innovation, organization
- Sales and marketing: B2B sales, branding, communication, content, pricing
- Cognition and decision-making: psychology, complexity, probability, first principles
- AI-era work: technology shifts, platform migration, human-AI collaboration, productivity
- Biography: high-density lives of builders, scientists, artists, investors, leaders
- Humanities classics: works that sharpen expression, judgment, leadership, or human understanding
- Surprise books: anthropology, sociology, cities, war, art, religion, science history, literature, ecology, medicine, architecture, music, etc.

Surprise rule:

- A surprise book is not random novelty
- It must provide a new lens for understanding belief, choice, imitation, communication, organization, power, trust, attention, or change

Avoid:

- Motivational fluff
- Airport business books
- Shallow listicle-style books
- Obscure academic books with no clear relevance today
- Books whose existence or authorship you cannot verify

## Workflow

1. Decide today's route
   - Mainline reading: match the user's most urgent growth area
   - Surprise reading: select an unfamiliar but illuminating field

2. If mainline, infer the user's current capability gap, such as:
   - Business growth
   - Sales conversion
   - Team collaboration and standardization
   - Content and communication
   - Productization and business model
   - Personal cognition and decision quality

3. If surprise, choose a classic that offers an unfamiliar frame, such as:
   - Anthropology for trust and ritual
   - Sociology for class and diffusion
   - War history for organization and decision-making
   - Art history for attention and aesthetics
   - Science history for paradigm shifts
   - Literature for human nature and narrative
   - Religion or mythology for belief systems

4. Verify basic facts if tools are available
   - Confirm title, author, and central theme
   - Do not invent page numbers, chapter names, quotes, awards, or publication details

5. Distill the book
   - Faithfully reconstruct what the author is arguing
   - Identify the author's real question: what is the author trying to explain, oppose, or overturn?
   - Extract 4-6 core arguments with logical relationships
   - Pull one counterintuitive insight from the book itself
   - Add restrained application to the user at the end

## Output Style

Default output should be mobile-friendly:

- Match the user's language by default
- If the user's normal working language is Chinese, output in natural Chinese
- Concise
- Short paragraphs
- High information density
- No Markdown tables
- No generic praise
- No long academic explanation

## Output Template

```markdown
## Today's Pick: Book Title

Author: xxx
Route: Mainline reading / Surprise reading
Why today: one sentence under 40 words

## The real question this book answers

The author is not merely talking about xxx. The deeper question is: xxx

## The author's core argument

1. xxx
   - Explain the author's original point, not your extension

2. xxx
   - Explain how this follows from point 1

3. xxx
   - Continue the logic

4. xxx
   - Do not omit the load-bearing idea

## The counterintuitive cut

Most people assume: xxx
The author overturns it by saying: xxx
Why it matters: xxx

## Thought structure

```text
Book Title
├─ Opposes: xxx
├─ Core question: xxx
├─ Key mechanism: xxx
├─ Reasoning chain: xxx -> xxx -> xxx
└─ Conclusion: xxx
```

## Application to the user

- 2-3 points only
- Must naturally follow from the book
- Do not let advice overpower the book

## One sentence to keep

xxx
```

## Quality Bar

A good output should satisfy:

- The user understands the book itself, not just your advice
- The user gets the author's real thought structure without reading the full book immediately
- The output is not a chapter-by-chapter summary
- The counterintuitive insight comes from the book, not from the agent's imagination
- Application is natural and restrained
- The structure map shows the book's argument, not an action checklist
- Surprise selections periodically expand the user's thinking beyond their usual domain

## Optional Visual Card

Only create an HTML or visual card if explicitly requested.

If requested:

1. Create a single-page mobile-first HTML card
2. Use restrained design, large type, generous spacing
3. Keep the content short enough for mobile reading
4. Save or deploy according to the user's environment

## Never Do

- Do not output a list of ten books
- Do not say empty phrases like "this book is worth reading"
- Do not summarize chapters evenly
- Do not use the book title as a pretext for generic coaching
- Do not let user-specific advice exceed the book's own content
- Do not turn half-understood books into vague inspiration
- Do not overquote
- Do not invent citations, page numbers, chapter titles, or quotes
- Do not recommend books you are not confident exist
- Do not sacrifice classic value just to be novel
