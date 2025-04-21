# .dotcommands - Enhanced AI Workflow System

## What are .dotcommands?

.dotcommands are a streamlined pattern for AI interactions that combine command-line efficiency with natural language. They're concise instructions prefixed with a period (`.`) that trigger specific, predictable behaviors from AI assistants.

```
.refactor my_messy_function()
```

## Why use .dotcommands?

- **Reduce typing effort**: Execute complex prompts with minimal keystrokes
- **Maintain workflow momentum**: Chain commands for continuous progress
- **Standardize outputs**: Get consistent formatting across interactions
- **Enhance mobile/tablet usage**: Ideal for limited keyboards and touch interfaces

## Real-world Usage

Users report these common workflow patterns:

- **Sequential task execution**: `.checklist` followed by multiple `.next` commands
- **Context recovery**: `.status` to re-orient after stepping away
- **Troubleshooting**: `.think` to analyze issues when bugs arise
- **Command chaining**: Combining commands like `.status .think` for comprehensive responses

## Configuration

For aider users, add to your config:
```yaml
# ~/.aider.conf.yml
read: ["~/.aider.dotcommands.md"]
```

Or load at runtime:
```bash
/read ~/.aider.dotcommands.md
```

## Core Commands

These essential commands form the foundation of the .dotcommands system:

### Meta Commands
- `.help`: Display contextually relevant commands based on current conversation
- `.status`: Generate a status report of the chat history context and next tasks
- `.think`: Analyze problems, identify root causes, and propose prioritized solutions

### Project Commands
- `.checklist`: Create a tasks.md file containing a checklist based on chat context
- `.next`: Identify and implement the next incomplete task from tasks.md
- `.plan`: Generate a step-by-step plan for completing specified task
- `.overview`: Generate a high-level summary of the project purpose and components

### Development Commands
- `.work`: Make it work first - focus on core functionality with minimal implementation
- `.right`: Make it right - refactor working code to improve structure
- `.fast`: Make it fast - optimize performance while maintaining clean architecture
- `.scaffold`: Generate boilerplate code structure with ASCII tree visualization
- `.interface`: Design clean API interfaces with minimal parameter requirements

## Command Categories

The complete .dotcommands system is organized into specialized modules:

- **`.dotcommands.md`** - Essential commands for everyday use
- **`.dotcommands-code.md`** - Programming and development commands
- **`.dotcommands-writing.md`** - Content creation and structuring commands
- **`.dotcommands-system.md`** - Project management and workflow commands
- **`.dotcommands-research.md`** - Analysis and knowledge exploration commands
- **`.dotcommands-roleplay.md`** - Character and persona-based commands

## Advanced Workflows

### Multi-Model Collaboration
Run multiple AI instances with different specializations:
- **Tab 1**: Fast, economical model for initial code generation
- **Tab 2**: Powerful model for review, refinement, and bug fixing

### Mobile/Remote Development
The .dotcommands system is particularly valuable for:
- iPad/tablet development via SSH
- Minimal keyboard environments
- Situations requiring quick context recovery

## Customization

Create personal commands with:

```
.define [name] [description] [template]
```

Example:
```
.define arch "Design high-level architecture" "# Architecture Overview\n\n## Components\n\n## Interfaces\n\n## Data Flow"
```

## Command Structure

Commands follow consistent syntax patterns:

- Basic: `.command` - Executes default behavior
- With positional parameters: `.command arg1 arg2`
- With named parameters: `.command --option=value`

## Design Philosophy

The .dotcommands system follows principles from software design leaders:

- **Simplicity** (Rob Pike): Clear, unambiguous actions that do one thing well
- **Elegance** (Armin Ronacher): Powerful abstractions with minimal syntax
- **Developer Experience** (Taylor Otwell): Intuitive, expressive patterns that feel natural

## Golden Rule Priority

For development tasks, follow this sequence:
1. First, `.work` - Focus on core functionality with minimal viable implementation
2. Then, `.right` - Refactor working code to remove technical debt and improve structure
3. Finally, `.fast` - Optimize performance while maintaining clean architecture

## License

This project is available under the MIT License.