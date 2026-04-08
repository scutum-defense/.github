# Contributing to Scutum

Thank you for your interest in contributing to Scutum's open-source defense infrastructure libraries.

## Before You Start

- Read the repository's README to understand its purpose and architecture
- Check existing issues and pull requests to avoid duplicate work
- For significant changes, open an issue first to discuss the approach

## Development Workflow

1. Fork the repository
2. Create a feature branch from `main`

```bash
git checkout -b feat/your-feature
# or
git checkout -b fix/your-fix
```

3. Make your changes with clear, focused commits
4. Ensure all checks pass locally

```bash
pnpm typecheck
pnpm lint
pnpm test
pnpm build
```

5. Submit a pull request against `main`

## Branch Naming

| Prefix | Purpose |
|:--|:--|
| `feat/` | New feature or capability |
| `fix/` | Bug fix |
| `docs/` | Documentation change |
| `test/` | Test addition or modification |
| `sec/` | Security-related change |
| `chore/` | Maintenance, CI, tooling |

## Commit Messages

Use clear, descriptive commit messages:

```
feat: add correlation matcher for multi-source threat detection
fix: correct haversine distance calculation for antipodal points
docs: add usage example for zone classification
test: add threshold matcher boundary condition tests
```

## Pull Request Requirements

- Clear description of what changed and why
- All CI checks passing
- Tests for new functionality
- Documentation updated if behavior changes
- CODEOWNERS review approval

## Code Standards

- TypeScript strict mode enabled
- No `any` types without justification
- Exported functions and types must be documented
- Tests for all public API surfaces
- No secrets, credentials, or sensitive data in code

## Security

- Report security vulnerabilities per [SECURITY.md](SECURITY.md)
- Do not open public issues for security findings
- Security-sensitive changes require security team review

## License

By contributing, you agree that your contributions will be licensed under the same license as the project (Apache-2.0 for open-source repositories).
