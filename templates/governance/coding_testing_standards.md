# Coding & Testing Standards

## Code
- Keep changes scoped to the story
- Prefer small, composable functions
- Explicit error handling for external/tool calls
- No secrets in code, logs, or test fixtures

## Testing
- Unit tests for core logic
- Integration tests for API behavior, auth, validation, DB interactions
- E2E only for critical user smoke paths (keep suite small/stable)
- Cover negative paths (401/403/400/404 where relevant)

## Security (Priority)
- Validate inputs on all boundaries
- Enforce authorization server-side
- Sanitize/escape output as applicable
- Log security-relevant events without sensitive payload leakage
