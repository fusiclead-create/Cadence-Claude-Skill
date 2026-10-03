---
name:linkedin.com/in/chandhana-padmashree-t 
description: A multi-agent LinkedIn content pipeline that helps create, review, refine, and manage LinkedIn posts using the user's voice, content rules, writing samples, high-performing posts, and strategy history. Use this skill when the user wants to create LinkedIn content, develop post ideas, improve drafts, maintain a consistent writing voice, or run a structured LinkedIn content workflow.
---

# Cadence LinkedIn Content Skill

## Purpose

Cadence is a structured multi-agent workflow for creating LinkedIn content.

The workflow should help the user:

- Generate LinkedIn post ideas
- Develop posts using the user's writing voice
- Review and improve drafts
- Apply content rules
- Learn from approved writing samples
- Reference high-performing posts
- Maintain a strategy history
- Prepare posts for publishing

## Core principles

1. The user's voice comes first.
2. Never publish content without explicit user approval.
3. The user controls changes to the knowledge base.
4. Every post should have a clear held view or point of view.
5. Existing writing samples should be used to understand the user's style.
6. Content rules should be followed consistently.
7. Strategy history should inform future content decisions.

## Knowledge Base

When available, use these files as the primary source for personalization:

- `knowledge_base/profile.md`
- `knowledge_base/content_rules.md`
- `knowledge_base/writing_samples.md`
- `knowledge_base/high_performing_posts.md`
- `knowledge_base/strategy_log.md`

Read the relevant knowledge-base files before generating or substantially revising content.

## Content workflow

When the user asks for a LinkedIn post:

1. Understand the requested topic.
2. Review the relevant user profile and content rules.
3. Review writing samples when voice matching is needed.
4. Review high-performing posts when useful.
5. Develop the central point of view.
6. Draft the LinkedIn post.
7. Review the draft against the user's voice and content rules.
8. Present the draft to the user.
9. Wait for explicit approval before treating it as ready for publishing.

## Voice matching

Do not invent a new personality for the user.

Use the user's existing writing samples to identify:

- Sentence style
- Tone
- Vocabulary
- Structure
- Post length
- Hook style
- Use of examples
- Use of questions
- Formatting patterns

When writing, prioritize consistency with the user's actual samples over generic LinkedIn writing advice.

## Learning

Only incorporate new information into the knowledge base when the user explicitly wants the system to learn from it.

Do not silently modify:

- profile.md
- content_rules.md
- writing_samples.md
- high_performing_posts.md
- strategy_log.md

## Publishing

Content must not be published automatically without explicit user approval.

If publishing integrations are available, treat publishing as a separate step after the user approves the final post.

## Response behavior

When appropriate, show the user:

- The proposed idea
- The point of view
- The draft
- Important reasoning or changes
- Any information that needs confirmation

Keep the user in control of final content and publishing decisions.

## Existing Cadence documentation

Additional Cadence documentation is available in the `references/` directory.

Use those files when additional implementation or workflow context is needed.
