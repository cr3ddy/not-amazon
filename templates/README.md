# Controlled Template Pack

Version: v1.0.0

This folder contains controlled templates used by the agent orchestrator.

## Freeze / Change Rules
- Templates are treated as controlled assets.
- Changes are allowed only via PR review.
- Update `templates/manifest.json` version + checksums in the same PR.
- Do not modify templates ad hoc during a story run.

## Usage
- The orchestrator may read and instantiate these templates into story-specific artifacts.
- Generated artifacts should live under `docs/artifacts/` or another run-specific path.
