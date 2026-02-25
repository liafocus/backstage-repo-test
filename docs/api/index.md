# API Documentation

## Overview

This section documents internal and external APIs maintained by the team.

## API Catalog

| API | Type | Status | Description |
|-----|------|--------|-------------|
| _Example API_ | REST | Active | _Brief description_ |

## Conventions

- All REST APIs use JSON request/response bodies.
- Authentication is handled via Bearer tokens.
- API versioning follows the `/api/v1/` URL prefix pattern.

## Adding API Documentation

To document a new API:

1. Create a new Markdown file under `docs/api/` (e.g., `docs/api/users-api.md`).
2. Add it to the `nav` section in `mkdocs.yml`.
3. Include endpoints, request/response examples, and error codes.
