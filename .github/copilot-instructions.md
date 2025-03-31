# PowerShell Guidelines

## Code Structure

- Use advanced functions with `[CmdletBinding()]` and comment-based help
- Follow Verb-Noun naming with approved PowerShell verbs
- Use camelCase for variables, PascalCase for parameters
- Return objects directly without using return keyword
- Document parameters with detailed descriptions

## Code Formatting

- Do not split ScriptBlock expressions across multiple indentation levels
- If a code block uses multiple indentation levels within a single expression, preserve that exact formatting
- Keep related code blocks visually cohesive
- Keep single commands on a single line without using backticks
- Maintain code line integrity, especially for multi-condition statements
- Maintain consistent indentation using 4 spaces (not tabs)
- Maintain opening and closing braces at the same indentation level as their parent construct
- Never split existing single expression statements across multiple lines

## Best Practices

- Return structured objects with Status property, not formatted text
- Support -WhatIf for state-changing functions
- Use [OutputType()] attribute on functions
- Use parameter splatting for complex cmdlet calls
- Use try/catch blocks for error handling

## Security

- Clear sensitive information from memory when no longer needed
