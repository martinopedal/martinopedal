This is a GitHub profile README repository.

## Security rules
- No secrets in code - use environment variables or GitHub Secrets
- SHA-pin all GitHub Actions to commit SHAs
- Use actions/checkout@v6 (Node.js 24 compatible)

## GitHub-first principle
Validate changes in GitHub Actions, not locally. Push, trigger workflow, check logs, iterate.