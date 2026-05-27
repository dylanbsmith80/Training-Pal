---
name: program-pal-intake-questions
description: Use when Program Pal is missing required client or program information before creating a Program Blueprint, exercise selections, or final workout workbook. This skill checks required inputs and asks focused follow-up questions instead of guessing.
---

# Program Pal Intake Questions Skill

Use this skill before Program Pal designs a program, selects exercises, or creates a final workout workbook. Program Pal may still summarize an assessment before this gate, but it must pass this gate before creating the actual program.

This skill is a readiness gate. Its job is to confirm Program Pal has the minimum required information to build a safe, specific, client-centered program.

## Required Knowledge

Program Pal must know these five items before creating a program:

1. How many sessions per week
2. Session length: 30 minutes or 60 minutes
3. Difficulty rating on a 1-10 scale, with 10 being the most challenging
4. Client goals
5. Client limitations

If any of these are missing, unclear, or contradictory, ask before moving on.

## Question Rules

Ask focused questions instead of guessing.

Use these rules:

- Ask only for missing or unclear required information.
- Group questions together when multiple required items are missing.
- Keep questions plain and easy for the trainer to answer quickly.
- Do not ask for information that is already clearly stated.
- Do not treat vague answers as complete if they could materially change the program.
- When limitations are unclear, ask about pain, injuries, medical constraints, movement restrictions, and exercises to avoid.
- When goals are broad, ask for the primary goal and any secondary goals.

## Required Question Prompts

Use or adapt these prompts:

### Sessions Per Week

"How many training sessions per week should this program include?"

### Session Length

"Are the sessions 30 minutes or 60 minutes?"

### Difficulty Rating

"What difficulty level should this program target on a 1-10 scale, with 10 being the most challenging?"

### Client Goals

"What are the client's main goals for this program? If there are multiple goals, which one is the top priority?"

### Client Limitations

"What limitations should Program Pal account for? Include pain, injuries, medical considerations, movement restrictions, exercises to avoid, or anything the client cannot or should not do."

## Readiness Output

When checking readiness, output one of these:

### Ready For Program Design

Use when all five required items are known.

Include:

- Sessions per week
- Session length
- Difficulty rating
- Client goals
- Client limitations

### Missing Required Information

Use when one or more required items are missing.

Include:

- Known information
- Missing information
- Focused questions for the missing items

## Handoff

Once all five required items are known, hand off to `program-pal-program-design` to create the Program Blueprint.

If exercise choices are needed, use `program-pal-exercise-selection` after the Program Blueprint has enough structure.

Do not create the final Excel workbook until this readiness gate has passed.
