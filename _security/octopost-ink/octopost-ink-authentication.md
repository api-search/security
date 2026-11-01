---
anonymous_access: false
api_key_in: []
api_specs:
- filename: octopost-ink-accounts-api-openapi.yml
  format: yaml
  label: octopost-ink Accounts API
  slug: octopost-ink-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octopost-ink/openapi/octopost-ink-accounts-api-openapi.yml
- filename: octopost-ink-posts-api-openapi.yml
  format: yaml
  label: octopost-ink Posts API
  slug: octopost-ink-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octopost-ink/openapi/octopost-ink-posts-api-openapi.yml
- filename: octopost-ink-queue-settings-api-openapi.yml
  format: yaml
  label: octopost-ink Queue Settings API
  slug: octopost-ink-queue-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octopost-ink/openapi/octopost-ink-queue-settings-api-openapi.yml
auth_types: []
description: Authentication uses an API key passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Octopost Ink Authentication
name_suffix: Authentication
oauth_flows: []
overview: octopost-ink declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: octopost-ink
provider_slug: octopost-ink
scheme_count: 1
schemes:
- evidence: All API requests must be authenticated using an API key passed as a Bearer token.
  header: Authorization
  how_to_obtain: Generate an API key in the Octopost Dashboard under Settings > API Keys and copy the key (starts with op_).
  location: header
  name: Bearer
  type: http-bearer
slug: octopost-ink-authentication
source_filename: octopost-ink-authentication.yml
source_heading: Authentication Profile
source_url: https://octopost.ink/docs/api/authentication
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://octopost.ink/docs/api/authentication\nsources:\n- https://octopost.ink/docs/api/authentication\n- https://octopost.ink/docs/api/authentication.md\n- https://octopost.ink/docs/mcp.md\n- https://octopost.ink/docs/getting-started.md\ndescription: Authentication uses an API key passed as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: All API requests must be authenticated using an API key passed as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the Octopost Dashboard under Settings > API Keys and copy the key (starts with op_).\ndocs: https://octopost.ink/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/octopost-ink/authentication/octopost-ink-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Social Media
- Automation
- Marketing
- API
---
