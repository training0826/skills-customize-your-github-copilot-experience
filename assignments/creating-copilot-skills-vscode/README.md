# 📘 Assignment: Creating Skills for Copilot in VS Code

## 🎯 Objective

Create a custom Copilot skill for VS Code that gives the agent a reliable workflow for a repeated development task. Practice writing discovery metadata, organizing progressive-disclosure references, and using scripts for deterministic operations.

## 📝 Tasks

### 🛠️ Define the Skill Workflow

#### Description

Choose a repeatable development task and create a skill directory with a main `SKILL.md` file. Describe when Copilot should use the skill and provide clear steps for completing the task.

#### Requirements

Completed skill should:

- Use a descriptive kebab-case directory name under `.github/skills/`.
- Include YAML frontmatter with a `name` matching the directory name.
- Include a specific `description` that explains when Copilot should activate the skill.
- Document a clear, ordered workflow in the body of `SKILL.md`.

### 🛠️ Add Progressive-Disclosure Resources

#### Description

Separate supporting knowledge from the main workflow so Copilot can load it only when needed. Add a reference document that provides domain guidance relevant to the selected task.

#### Requirements

Completed skill should:

- Include a `references/` directory.
- Add at least one Markdown reference file with relevant domain guidance.
- Link to the reference file from `SKILL.md` using a working relative path.
- Keep the main workflow focused by placing background explanations in the reference file.

### 🛠️ Bundle and Verify a Deterministic Script

#### Description

Add a script for an operation that should produce consistent results every time, such as generating a file, updating structured data, or validating the skill. Document how Copilot should run the script and verify the completed skill structure.

#### Requirements

Completed skill should:

- Include a `scripts/` directory containing at least one executable script.
- Validate required inputs and report clear errors when input is invalid.
- Avoid requiring Copilot to perform a fragile manual text or configuration edit.
- Document the script command and expected arguments in `SKILL.md`.
- Verify that the skill file, references, and scripts exist and that the frontmatter is valid.
