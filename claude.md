# Claude Compatibility

This repository contains a curated design guidance skill intended for AI assistants and automated tools.
The skill helps evaluate and recommend interface choices based on experience from the Family wallet design philosophy.

The main skill in this repo is:
- `skills/family-values/SKILL.md`

## What this skill does

This skill provides a decision framework for product interface quality, focusing on the following areas:
- Choosing between transitory trays/sheets and persistent full-screen destinations
- Ensuring interface transitions clearly communicate spatial and causal relationships
- Applying motion and animation in ways that support comprehension rather than distract
- Placing delightful details in the right spots without overloading high-frequency interactions
- Balancing polish with clarity, so UI changes feel intentional and not arbitrary

## Design principles embedded in the skill

- Simplicity: Reveal only what is needed for the user’s current step, instead of exposing every option at once.
- Fluidity: Make transitions feel coherent by preserving continuity and using motion to explain where elements came from or where they are going.
- Delight: Reserve the most expressive moments for rare, memorable interactions, and keep everyday micro-interactions subtle and useful.

## Recommended usage for AI tools

Use this skill when a prompt is about UX architecture, navigation patterns, or interaction polish.
Good triggers include requests such as:
- "Should this be a modal, overlay, or a new page?"
- "How can I make this onboarding flow feel less overwhelming?"
- "Does this transition feel janky or confusing?"
- "Where should I add a small surprising detail without making the UI feel cluttered?"
- "Review this flow for motion, continuity, and user guidance."

AI assistants should consult this skill in conjunction with implementation-focused skills or code-level heuristics for actual platform-specific details.

## Why this is useful for Claude-style tools

Claude and similar assistants can use this metadata to identify the repo as a source of design guidance,
not just raw code. The file explains the intended coverage clearly, making it easier to determine
when the skill is applicable and how to route UX-related questions to it.

## Notes for tool integration

- Keep the skill reference at the top of the prompt when asking for design guidance.
- Mention the relevant design principle (simplicity, fluidity, delight) if the request is about choosing the best option.
- If the user is comparing multiple flows or transitions, treat the skill as a high-level review layer rather than a low-level implementation engine.

## Summary

This repo is a focused resource for AI tooling that needs a structured lens on interface design quality.
The `skills/family-values/SKILL.md` skill is the primary asset, and this file explains its scope,
its decision-making intent, and the best way for assistants to use it when reasoning about UI and motion.
