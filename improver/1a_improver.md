
# Prompt Optimization and Modularization Task

## Number of files
Number of files to generate: 8

## Objective
Deconstruct and refine the provided prompt into a sequence of at least <number_of_files> optimized Markdown (.md) files. The goal is to modularize the logic to enhance LLM reasoning efficiency and processing accuracy.

## File Structure Requirements
Each generated file must be self-contained and include the following sections:
- **Persona**: The specific role the agent assumes for this sub-task.
- **Task**: A concise description of the objective.
- **Workflow**: A step-by-step execution plan.
- **Rules**: Explicit operational guidelines.
- **Skills**: Required capabilities or knowledge domains.
- **Constraints**: Critical boundaries and "what-not-to-do" instructions.

## Output Specifications
- **Directory**: Save results in `/improved/<original_filename>/`.
- **Naming Convention**: Use the original filename with a sequential suffix (e.g., `filename_1.md`, `filename_2.md`).
- **Optimization**: Use clear delimiters (e.g., Markdown headers, bullet points) to ensure the structure is easily parsable by an LLM.

## Execution Logic
- Generate a minimum of <number_of_files> files.
- Ensure files are **logically connected** for sequential execution while remaining **functionally independent**.
- Modularize the content such that each file focuses on a specific phase of the overall process to minimize context noise.
