# 📘 Assignment: Build a Production-Ready Copilot Skill System

## 🎯 Objective

Design and build a reusable Copilot customization that supports a complete development workflow in VS Code. Combine a focused skill, specialized custom agents, progressive-disclosure references, deterministic scripts, and guardrails so the workflow is reliable and easy to verify.

## 📝 Tasks

### 🛠️ Design the Agentic Workflow

#### Description

Choose a repeatable development task and design how different Copilot roles should collaborate. Create a primary custom agent for planning or review and document how it hands work to Agent Mode or another specialized agent for implementation.

#### Requirements

Completed workflow should:

- Define a clear development task with a specific expected outcome.
- Include at least two custom agents with distinct responsibilities.
- Give each agent only the tools it needs for its responsibility.
- Include at least one handoff with a clear label and prompt.
- Explain how the workflow moves from planning to implementation to verification.

### 🛠️ Build the Skill and Its Resources

#### Description

Implement the workflow as a reusable skill under `.github/skills/<skill-name>/`. Keep the main instructions concise, and move supporting domain knowledge into reference files that the agent can load when needed.

#### Requirements

Completed skill should:

- Include valid frontmatter with a descriptive `name` and activation-focused `description`.
- Document an ordered workflow in `SKILL.md`.
- Include a `references/` directory with at least one relevant guide.
- Include a `scripts/` directory with at least one deterministic helper script.
- Document when to read references and how to run each bundled script.

### 🛠️ Add Guardrails and Verify the System

#### Description

Make the customization dependable by validating inputs, protecting important files, and checking the complete workflow. Test the skill with a realistic request and record what each agent produced at every handoff.

#### Requirements

Completed system should:

- Validate required script inputs and report actionable errors.
- Prevent a script from silently overwriting or duplicating existing results.
- Include at least one guardrail that requires verification before completion.
- Confirm that all referenced files and script paths exist.
- Test the handoff workflow from the initial request through implementation and verification.
- Record at least one limitation, failure case, or improvement discovered during testing.
