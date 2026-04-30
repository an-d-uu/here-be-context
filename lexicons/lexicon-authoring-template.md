# Lexicon Authoring Template

Use this when determining where content belongs and how it should be structured within the lexicon system.

## Instructions

Your task is to review the wording I provide and decide whether it should:

1. be added to an existing lexicon, or
2. become the foundation of a new lexicon

Follow these rules:

- Preserve the repo’s theme and naming style
- Treat lexicons as expression-control artifacts, not general instructions
- Favor precise, reusable phrasing patterns over one-off rewrites
- Keep tone professional, clear, neutral, and scope-safe unless the wording explicitly calls for a different approved style
- Avoid implied commitments, unnecessary ownership, panic-inducing phrasing, or uncontrolled flair
- When useful, distill the example into a more reusable phrasing pattern
- Do not invent random personality
- Keep metadata limited to artifact-level information
- Do not place behavioral guidance, tone rules, examples, or usage instructions in metadata unless they describe how the file itself should be used

When responding, do the following:

## Step 1: Classification

State whether this should be:

- added to an existing lexicon, or
- created as a new lexicon

## Step 2: Recommendation

If it belongs in an existing lexicon:

- recommend the best lexicon name
- recommend the best section name
- explain why briefly

If it should be a new lexicon:

- propose the lexicon filename
- provide a 1 to 2 sentence purpose statement for the file
- propose the first section name
- explain why briefly

## Step 3: Entry Formatting

Format the content as a ready-to-paste lexicon entry using this structure:

- Instead of: <raw or undesired phrasing>
- Use: <preferred phrasing>
- Context: <when this phrasing should be used>
- Notes: <why this phrasing works, what it avoids, or what it signals>

## Step 4: Reusability Check

Then provide:

- a more specific version, if the original is situation-specific
- a more reusable generalized version, if possible

## Step 5: Metadata Guidance

If this content belongs in a new file, include suggested sidecar metadata for a `.meta.yaml` file.

Use this format:

```yaml
file: <proposed-lexicon-filename.md>
title: <lexicon title>
type: lexicon
tool: ChatGPT
version: v1.0
purpose: <1 sentence describing what this lexicon controls>
