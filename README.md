# Thesis Assistant Skill

A comprehensive Claude skill to help graduate students complete their under Master thesis. This skill guides you through the entire thesis lifecycle from topic clarification to final submission.

## Features

- **7-Phase Workflow**: Structured approach covering assessment, topic clarification, planning, execution, integration, format verification, and submission
- **Smart Skill Discovery**: Intelligently detects available skills and recommends appropriate ones, with fallback options when skills are unavailable
- **Multiple Thesis Types Supported**:
  - Experimental/Empirical
  - Theoretical/Analysis
  - Implementation/Engineering
  - Literature Review/Meta-analysis
  - Mixed Methods

## Installation

### Option 1: Via Git Clone
```bash
cd ~/.claude/skills
git clone https://github.com/seal-at-sale/Treat-AI-As-Your-Partner.git thesis
```

### Option 2: Via Claude Plugin Manager
```
/plugin install thesis
```

### Option 3: Manual Download
1. Download the `SKILL.md` file from this repository
2. Place it in `~/.claude/skills/thesis/SKILL.md`

## Usage

Once installed, simply invoke the skill:

```
/thesis
```

The skill will guide you through:
1. **Initial Assessment** — Understanding your current stage and thesis type
2. **Topic Clarification** — Refining your research questions and scope
3. **Structure & Planning** — Creating chapter outlines and timelines
4. **Component Execution** — Working through each chapter with specialized agents
5. **Integration & Cross-Checking** — Ensuring coherence across your thesis
6. **Format Verification** — Checking against school requirements
7. **Final Review** — Pre-submission quality audit

## Skill Recommendations

This skill intelligently recommends other Claude skills when appropriate:

| For This Need | Recommended Skill | Fallback if Unavailable |
|--------------|-------------------|------------------------|
| Visual design for figures | `/design-review`, `/design-consultation` | Manual design guidelines |
| Research paper discovery | `/browse` | WebSearch tool |
| Code review | `/review` | Manual code review checklist |
| Brainstorming methodology | `/office-hours` | Structured questioning |
| QA testing | `/qa` | Manual testing checklist |
| Debugging | `/investigate` | Structured debugging questions |

## Repository Structure

```
thesis/
├── SKILL.md          # Main skill definition (required)
└── README.md         # This file
```

## Requirements

- Claude Code or Claude.ai with skills support
- Tools: Bash, Read, Write, Edit, AskUserQuestion, Agent, TaskCreate, TaskUpdate, TaskList, Glob, Grep

## Contributing

Contributions welcome! Please submit issues or pull requests.

## License

MIT License - See LICENSE file for details

## Acknowledgments

Created with the [skill-creator](https://github.com/anthropics/skill-creator) plugin for Claude.
