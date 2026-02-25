# Contributing to TNG Solution

Thank you for your interest in contributing to TNG Solution. This document provides guidelines and instructions for contributing to our projects.

---

## Getting Started

### Prerequisites

- Git knowledge
- GitHub account
- Relevant technical skills (Terraform, Kubernetes, Go, Shell, etc.)
- Familiarity with the specific repository's technology stack

### Setup

1. Fork the repository
2. Clone your fork locally
3. Create a new branch for your changes
4. Make your changes
5. Test your changes thoroughly
6. Submit a pull request

---

## Development Workflow

### Branch Naming

Use descriptive branch names:

```
feature/description-of-feature
bugfix/description-of-bug
docs/description-of-documentation
chore/description-of-task
```

### Commit Messages

Write clear, descriptive commit messages:

```
type: brief description

Longer explanation of the change if needed.
- Point 1
- Point 2
```

Commit types:

- `feat` - New feature
- `fix` - Bug fix
- `docs` - Documentation changes
- `style` - Code style changes (formatting, semicolons, etc.)
- `refactor` - Code refactoring
- `test` - Adding or updating tests
- `chore` - Build, dependencies, or other maintenance

### Pull Requests

When submitting a pull request:

1. **Provide a clear title** - Briefly describe the change
2. **Write a description** - Explain what changed and why
3. **Reference issues** - Link to related issues if applicable
4. **Keep it focused** - One feature or fix per PR when possible
5. **Test thoroughly** - Verify your changes work as expected

---

## Code Standards

### General Principles

- Write clean, readable code
- Follow the language's conventions
- Include comments for complex logic
- Remove debug code before submitting
- Keep files organized and well-structured

### Language-Specific Guidelines

**Terraform (HCL)**
- Use consistent indentation (2 spaces)
- Use descriptive variable and resource names
- Include variable descriptions and types
- Format with `terraform fmt`
- Validate with `terraform validate`

**Go**
- Run `go fmt` for formatting
- Use `go vet` to check for errors
- Follow Go naming conventions
- Include package documentation
- Write unit tests for new functions

**Kubernetes YAML**
- Use 2-space indentation
- Include resource metadata (labels, annotations)
- Use descriptive names
- Organize related resources logically
- Validate YAML syntax

**Shell Scripts**
- Use consistent style and indentation
- Include shebang (`#!/bin/bash`)
- Add error handling
- Include comments for non-obvious sections
- Make scripts executable

---

## Testing

### Before Submitting

- Test changes in your local environment
- Run any available test suites
- Verify no breaking changes
- Check for security issues
- Validate syntax and formatting

### Test Requirements

- Infrastructure changes should be tested in a non-production environment
- Code changes should include relevant tests
- Documentation changes should be reviewed for accuracy

---

## Documentation

### When to Update Documentation

- When adding new features
- When changing behavior
- When fixing bugs that affect users
- When updating dependencies
- When changing configuration options

### Documentation Standards

- Use clear, concise language
- Include examples where helpful
- Update relevant README files
- Include code comments for complex logic
- Keep documentation in sync with code

---

## Security

### Security Issues

Do not open public issues for security vulnerabilities. See [SECURITY.md](SECURITY.md) for responsible disclosure procedures.

### Security Checklist

- Do not commit secrets or credentials
- Do not include API keys or passwords
- Follow least-privilege principles
- Validate user input
- Use appropriate authentication mechanisms

---

## Review Process

### What to Expect

1. **Initial Review** - A maintainer will review your PR for completeness and scope
2. **Code Review** - Changes will be reviewed for quality and standards compliance
3. **Testing** - Automated tests will run on your changes
4. **Feedback** - You may receive requests for changes or clarifications
5. **Approval** - Once approved, your changes will be merged

### Responding to Feedback

- Address comments promptly
- Ask for clarification if needed
- Push additional commits to the same branch
- Update your PR description if scope changes
- Mark conversations as resolved when complete

---

## Common Issues

### My PR is out of date

```bash
git fetch upstream
git rebase upstream/main
git push -f origin your-branch
```

### I need to update my commits

```bash
git rebase -i HEAD~n  # where n is the number of commits to edit
git push -f origin your-branch
```

### How do I sync my fork?

```bash
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```

---

## Repository-Specific Guidelines

Refer to each repository's README for specific contribution guidelines, setup instructions, and technology-specific requirements.

---

## Questions?

If you have questions about contributing:

1. Check the repository's README
2. Review open issues and pull requests
3. Open a new discussion or issue for clarification

---

## Code of Conduct

All contributors are expected to follow our [Code of Conduct](CODE_OF_CONDUCT.md). Please report any violations through the appropriate channels.

---

Thank you for contributing to TNG Solution!