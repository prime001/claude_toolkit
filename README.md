# Claude Toolkit

A structured toolkit for using Claude as an engineering assistant through **skills, prompts, context, templates, and workflows**.

This repository provides reusable components that turn Claude from a simple chat assistant into a **structured engineering workflow engine**.

The toolkit helps enforce consistent thinking patterns such as:

* architecture before implementation
* systematic debugging
* structured code reviews
* production-safe design decisions
* repeatable workflows

---

# Philosophy

Claude performs best when given **clear roles, context, and structure**.

This toolkit separates those concerns into layers:

| Layer     | Purpose                              |
| --------- | ------------------------------------ |
| Skills    | Define expertise (how Claude thinks) |
| Context   | Describe the project environment     |
| Prompts   | Define the task to perform           |
| Templates | Enforce consistent output structure  |
| Workflows | Define multi-step processes          |

This prevents common problems such as:

* inconsistent outputs
* shallow reasoning
* skipping design steps
* weak debugging or review processes

---

# Repository Structure

```
.claude/
├── skills/
├── prompts/
├── context/
├── templates/
├── workflows/
└── outputs/
```

## `skills/`

Reusable **expert roles** that define how Claude should reason.

Examples include:

* `systems_architect.md`
* `devops_engineer.md`
* `full_stack_engineer.md`
* `debugging_specialist.md`
* `staff_code_reviewer.md`
* `security_auditor.md`
* `performance_optimizer.md`
* `technical_writer.md`
* `product_strategist.md`
* `seo_marketing_strategist.md`
* `ai_agent_architect.md`
* `incident_responder.md`
* `network_architect.md`
* `startup_operator.md`
* `cisco_nso_expert.md`

These roles give Claude **domain expertise and decision frameworks**.

---

## `context/`

Project knowledge that Claude should understand before making recommendations.

Typical files:

```
context/
├── project_context.md
├── architecture.md
├── stack.md
├── constraints.md
├── coding_standards.md
├── glossary.md
└── review_focus.md
```

This prevents Claude from making generic assumptions about the system.

---

## `prompts/`

Reusable prompts that define **task types**.

Examples:

```
prompts/
├── build.md
├── task.md
├── review.md
├── fix.md
└── summary.md
```

Typical development flow:

```
build → task → review → fix → summary
```

Each prompt loads the appropriate skills and context.

---

## `templates/`

Output templates that enforce consistent structure.

Examples:

```
templates/
├── architecture_template.md
├── code_review_template.md
├── feature_design_template.md
├── documentation_template.md
└── incident_response_template.md
```

These ensure Claude responses are **organized and actionable**.

---

## `workflows/`

Multi-step procedures that guide Claude through complex tasks.

Examples:

```
workflows/
├── feature_development.md
├── bug_fix.md
├── architecture_design.md
├── code_review.md
├── incident_response.md
├── nso_service_development.md
├── nso_reconcile_review.md
└── startup_launch.md
```

Workflows combine:

* skills
* prompts
* templates
* context

to produce **repeatable engineering processes**.

---

## `outputs/`

Optional directory for storing:

* generated prompts
* Claude responses
* architecture drafts
* review reports

This can be useful when running automated pipelines.

---

# Example Usage

Inside a repository with the toolkit:

```
claude
```

Then run a task using the toolkit.

Example:

```
Use:
.claude/workflows/feature_development.md

Task:
Build a cyberdeck-style dashboard for my home network with system metrics, terminal interface, achievements, and a scoreboard.
```

Claude will follow the workflow:

1. design the architecture
2. implement the feature
3. review the implementation
4. fix issues
5. summarize results

---

# Example Code Review

```
Use:
.claude/workflows/code_review.md

Review:
src/services/reconcile.py
```

Claude will:

* analyze the code
* identify risks
* recommend improvements
* classify issues by severity

---

# Why This Toolkit Exists

Most AI usage fails because prompts are **ad-hoc and inconsistent**.

This toolkit provides:

* structured reasoning
* repeatable workflows
* reusable expertise modules
* consistent output formats

It effectively turns Claude into a **structured engineering assistant**.

---

# Recommended Workflow

A typical engineering task should follow this sequence:

```
Architecture Design
        ↓
Implementation
        ↓
Code Review
        ↓
Fixes
        ↓
Summary / Documentation
```

The toolkit provides prompts and workflows for each stage.

---

# Best Practices

* Keep skills **focused and specialized**
* Keep context files **accurate and updated**
* Use workflows for **complex tasks**
* Use templates to **standardize outputs**
* Prefer **incremental improvements over large rewrites**

---

# Future Enhancements

Potential improvements include:

* CLI tooling for prompt orchestration
* CI/CD integration for automated AI reviews
* local prompt rendering pipelines
* repository-specific agent commands

Example future structure:

```
.claude/agents/
├── architect.md
├── reviewer.md
├── debugger.md
└── nso.md
```

Allowing commands such as:

```
/architect
/review
/debug
```

---

# License

MIT License

---

# Author

Prime001

GitHub:
https://github.com/prime001
