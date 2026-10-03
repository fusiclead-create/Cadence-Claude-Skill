---
name: linkedin.com/in/chandhana-padmashree-t 
description: A multi-agent LinkedIn content pipeline that helps create, review, refine, and manage LinkedIn posts using the user's voice, content rules, writing samples, high-performing posts, and strategy history. Use this skill when the user wants to create LinkedIn content, develop post ideas, improve drafts, maintain a consistent writing voice, or run a structured LinkedIn content workflow.
---

# Cadence LinkedIn Content Skill

## Purpose

Cadence is a structured multi-agent workflow for creating LinkedIn content.

The workflow helps the user:

- Generate LinkedIn post ideas
- Develop posts using the user's writing voice
- Research topics
- Create hooks
- Review and improve drafts
- Apply content rules
- Learn from approved writing samples
- Reference high-performing posts
- Maintain a strategy history
- Prepare posts for publishing

## Core Principles

1. The user's voice comes first.
2. Never publish content without explicit user approval.
3. The user controls changes to the knowledge base.
4. Every post should have a clear point of view.
5. Existing writing samples should be used to understand the user's style.
6. Content rules should be followed consistently.
7. Strategy history should inform future content decisions.
8. Do not silently change the user's knowledge base.

## Knowledge Base

When available, use these files as the primary source for personalization:

- `knowledge_base/profile.md`
- `knowledge_base/content_rules.md`
- `knowledge_base/writing_samples.md`
- `knowledge_base/high_performing_posts.md`
- `knowledge_base/strategy_log.md`

Read the relevant knowledge-base files before generating or substantially revising content.

## Content Workflow

When the user asks for a LinkedIn post:

1. Understand the requested topic.
2. Review the relevant user profile and content rules.
3. Review writing samples when voice matching is needed.
4. Review high-performing posts when useful.
5. Research the topic when research is required.
6. Develop the central point of view.
7. Create several possible hooks when useful.
8. Draft the LinkedIn post.
9. Review the draft against the user's voice and content rules.
10. Present the draft to the user.
11. Ask for approval or requested revisions.
12. Do not publish until the user explicitly approves the final version.

## Voice Matching

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

Do not "corporate-ify" the user's writing.

## Research

When research is required:

1. Identify the specific topic.
2. Gather relevant information.
3. Separate factual information from opinions or interpretations.
4. Use the research to strengthen the post rather than turning the post into a generic summary.
5. Preserve the user's point of view and writing style.

## Learning

Only incorporate new information into the knowledge base when the user explicitly wants the system to learn from it.

Do not silently modify:

- `profile.md`
- `content_rules.md`
- `writing_samples.md`
- `high_performing_posts.md`
- `strategy_log.md`

If a useful change is identified, propose it to the user first.

## Publishing

Content must not be published automatically without explicit user approval.

Publishing is a separate step after the final post has been approved.

If publishing integrations are available, use them only after approval.

## Approval

The approval checkpoint is mandatory.

Before publishing, clearly show the final content to the user and wait for an explicit confirmation such as:

- "Approve"
- "Yes, publish"
- "Post it"
- "Publish"

Do not interpret silence or an ambiguous response as approval.

## Response Behavior

When appropriate, show the user:

- The topic
- The point of view
- Hook options
- The draft
- Important changes
- Research that materially affects the draft
- Any information that needs confirmation

Keep the user in control of the final content and publishing decision.

## Existing Cadence Documentation

Additional Cadence documentation is available in:

- `README.md`
- `CLAUDE.md`
- `GETTING_STARTED.md`

Use these files when additional Cadence workflow or implementation context is needed.

## Original Cadence Architecture

The original Cadence project uses:

- `.claude/commands/` for user commands
- `.claude/agents/` for specialist agents
- `knowledge_base/` for the user's profile, voice, rules, inspiration, and strategy history
- `scripts/` and `integrations/` for optional publishing functionality

The original workflow includes:

- `/setup`
- `/run-pipeline`
- `/add-writing-sample`
- `/linkedin-manager`

The Skill should preserve the important behavior of this workflow while keeping the user in control.
