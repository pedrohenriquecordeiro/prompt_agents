# Dynamic Prompt Optimization and Modularization Workflow

## Objective
To deconstruct a master prompt into $N$ optimized, modular Markdown files, where $N$ is a variable defined by the programmer based on the complexity of the task.

## Execution Logic (for $N$ Modules)
1.  **Define $N$**: The programmer specifies the total number of modules ($N$) required for the task.
2.  **Logical Segmentation**: Analyze the source prompt and divide its core logic into $N$ distinct, sequential phases (e.g., Phase 1, Phase 2 ... Phase $N$).
3.  **Modular Persona Assignment**: For each phase $i$ (where $1 \le i \le N$), assign a specialized persona tailored to that specific sub-task.
4.  **Contextual Hand-off**: Establish a "chain of thought" where each file $i$ requires the agent to review the output of file $i-1$ to ensure continuity.
5.  **Section Generation**: Populate each of the $N$ files with the mandatory sections: Context, Persona, Task, Workflow, Rules, Skills, and Constraints.
6.  **Directory Organization**: Save all results in `.prompts/improved/<original_filename>/`.
7.  **Sequential Naming**: Name files using the format `filename_i.md` to maintain the execution order.
8.  **Final Verification**: Ensure each module is functionally independent (can run on its own) but logically connected to the overall goal.

---

## Modular File Template (Dynamic)

# [Filename]_[i].md (Module $i$ of $N$)

## Context
[Describe the current state of the project at step $i$. Mention that this is part $i$ of a $N$-step modular sequence.]

## Persona
[Specific role for this phase, e.g., "Logic Architect" or "Quality Assurance Specialist".]

## Task
[A concise description of the objective for this specific module.]

## Workflow
1. **Analyze Project State**: Review the previous output and current project requirements.
2. **Execute Phase $i$**: [Insert specific step-by-step instructions for this module].
3. **Validate Output**: Ensure the result meets the specific rules of this module.

## Rules
- **Operational Guideline 1**: [Specific rule for this phase]
- **Operational Guideline 2**: [Formatting or logic constraint]

## Skills
- [Skill 1]
- [Skill 2]

## Constraints
- **Boundaries**: Do not address logic outside of Phase $i$.
- **Format**: Maintain strict Markdown compatibility.
